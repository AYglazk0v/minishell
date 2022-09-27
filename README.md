
<h1 align="center">
💻 Minishell
</h1>

## 💡 О проекте:

> _Этот проект посвящен созданию простой оболочки. Да, мы владеем маленьким bash.
Вы узнаете много нового о процессах и файловых дескрипторах._

	Этот проект состоит в написании собственного командного интерпретатора.
	Этот интерпретатор должен:
	- Отображать приглашение при ожидании новой команды
	- Иметь историю работы.
	- Находить и запускать исполняемые файды на основе переменной `PATH` в env, а так же
	при указании абсолютного пути.
	- Содержать не более одной глобальной перемеенной.
	- Корректно обрабатывать одинарные и двойные кавычки.
	- Корректно перенаправлять ввод и вывод ('<' и '>').
	- Выполнять дозапись в файл и воспроизводить поведение heredoc ('>>'  и '<<').
	- Выполнять команды связанные пайпами ('|') [Выход команды1 поступает на вход команды2].
	- Обрабатывать переменные окружения при помощи '$' (пример: echo $PATH).
	- Повторять поведение shell при команде `$ $?` [расшираться до состояния выхода
	последнего конвейера].
	- Обрабатывать сигналы 'Ctrl-C', 'Ctrl-D', 'Ctrl-\'
	- Не должен воспроизводить поведения shell при '\' и ';'.

	Так же нобходимо реализовать следующие встроенные функции:
	- `echo` с опцией `-n`.
	- `cd` -- только с относительным и абсолютным путем.
	- `pwd` без опций
	- `export` без опций
    - `unset` без опций
    - `env` без опций или аргументов
    - `exit` без опций
    
    Бонусная часть:
    - `&&` и `||` со скобками для приоритетов.
	- Подстановочные знаки `*` должны работать для текущего рабочего каталога.

Более подробно о проекте и нюансах можно посмотреть в  [**subject**](https://github.com/AYglazk0v/minishell/blob/main/Subject.pdf).

## 🛠 Тестирование и использование:

	# Клонируйте проект и получите доступ к папке
	git clone git@github.com:AYglazk0v/minishell.git && cd minishell/
	# Выполните make для сборки проекта
	make
	# Для запуска программы выполните команду
	./minishell
	# Для выхода из программы напишите exit, либо нажмите 'Ctrl-D'
	# Очистите выходные файлы с помощью
	make fclean

Для провекри корректности реализации проекта можно пройтись по [чеклисту](https://github.com/AYglazk0v/minishell/blob/main/checklist(old).pdf).

## 🎬 Демонстрация:
![exec](https://github.com/AYglazk0v/minishell/blob/main/exec.gif)
## P.S.:
Этот проект является групповым, репозиторий в котором велась работа над проектом: [link](https://github.com/MKKurbandibirov/Minishell).

Благодарю [напарника](https://github.com/MKKurbandibirov) за слаженную работу над проектом!

