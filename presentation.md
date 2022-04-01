# Timestamp


## Что такое timestamp?

```python
import time

print(time.time())
```


# Timestamp


## Что такое timestamp?

```python
import time

print(time.time())
```

    1648836725.796722


# Timestamp


## Что такое timestamp?

```python
import time
from datetime import datetime

t = time.time()
print(
  datetime.utcfromtimestamp(t)
)
```

    2022-04-01 18:12:05.841410


# Timestamp


## Что такое timestamp?

А что будет если вызвать такой код?

```python
from datetime import datetime

print(
  datetime.utcfromtimestamp(0)
)
```


# Timestamp


## Что такое timestamp?

```python
from datetime import datetime

print(
  datetime.utcfromtimestamp(0)
)
```

    1970-01-01 00:00:00


# UNIX


## 1970.1.1

**Дата отсчёта UNIX-эпохи**

![img](/home/pimiento/yap/thompson_n_ritchi.jpeg)


# UNIX

<span class="underline">Главные принципы UNIX</span>:

-   Всё есть файл (ну или почти всё)
-   Каждая программа должна уметь делать ****только одно**** и делать это хорошо!

****UNIX-way****


# Shell

-   *sh*
-   *bash*
-   *zsh*
-   csh
-   fish
-   ksh
-   tcsh


# Основные команды Bash (sh, zsh)


## ls

```sh
ls ~/workdir/generate-password/
```

    gen_pass
    README


# Основные команды Bash (sh, zsh)


## ls -l

```sh
ls -l ~/workdir/generate-password/
```

    total 8
    drwxr-xr-x 3 pimiento pimiento 4096 Jun 12  2021
    gen_pass
    -rw-r--r-- 1 pimiento pimiento  420 Apr 13  2021
    README


# Основные команды Bash (sh, zsh)


## ls -a

```sh
ls -a ~/workdir/generate-password/
```

    .
    ..
    gen_pass
    .git
    README


# Основные команды Bash (sh, zsh)


## which

```sh
which python3
```

    /usr/bin/python3


# Основные команды Bash (sh, zsh)


## mkdir

```sh
mkdir /tmp/notexist
```


# Основные команды Bash (sh, zsh)


## rm

```sh
rm -r /tmp/notexist
```


# Основные команды Bash (sh, zsh)


## grep

```sh
grep pimiento /etc/passwd
```

    pimiento:x:1000:1000:Pavel
    Vavilin,,,:/home/pimiento:/bin/zsh


# Основные команды Bash (sh, zsh)


## cat

```sh
cat /etc/lsb-release
```

    DISTRIB_ID=LinuxMint
    DISTRIB_RELEASE=20.3
    DISTRIB_CODENAME=una
    DISTRIB_DESCRIPTION="Linux Mint 20.3 Una"


# Основные команды Bash (sh, zsh)


## перенаправление

-   0 => stdin
-   1 => stdout
-   2 => stderr


# Основные команды Bash (sh, zsh)


## перенаправление

```sh
rm -r /tmp/notexist 2> /tmp/rm.log
cat /tmp/rm.log
```

    rm: cannot remove '/tmp/notexist': No such file
    or directory


# Основные команды Bash (sh, zsh)


## pipe

Выход одной команды мы можем подать на вход другой команде!

```sh
echo "Привет Яндекс Практикум" | wc -c
```

    45

```sh
cat /etc/lsb-release | grep RELEASE \
    |cut -d '=' -f 2|cut -d '.' -f 1
```

    20


# Основные команды Bash (sh, zsh)

```sh
cat /dev/urandom | hexdump -c
```


## Время стать крутыми хакерами!

![img](/home/pimiento/yap/matrix.png)


# UNIX это интересно!

![img](/home/pimiento/yap/unix.jpg)


# #!/usr/bin/env python

Шебэнг? Шебанг? Shebang.


## hello.py

```sh
#!/usr/bin/env python3

print("Hello World!")
```


## $>

```sh
chmod +x hello.py
```


# Что почитать?


## Про UNIX идеологию в целом

Брайн Керниган, Роб Пайк «Программное окружение UNIX»


## Bash

<span class="underline"><span class="underline">«[Advanced Bash-Scripting Guide](https://tldp.org/LDP/abs/html/)»</span></span>. На OpenNet можно найти <span class="underline"><span class="underline">[перевод](https://www.opennet.ru/docs/RUS/bash_scripting_guide/index.html)</span></span>


# SSH

( *В MS Windows чаще всего используют **PuTTY*** )

```sh
ssh user@ya.ru
```



```sh
scp user@ya.ru:/answers.txt ./
```


# VI

Редактор де-факто на всех UNIX-like системах
![img](/home/pimiento/yap/vim.jpg)


# VI

<div class="org-center">
<span class="underline"><span class="underline">[МЕМАСИКИ](https://yandex.ru/images/search?text=vim%20%D0%BC%D0%B5%D0%BC%D1%8B&from=tabbar)</span></span>
</div>


*шпаргалку по Vi/Vim пришлю после вебинара*


# Linux. При чём тут GIT?

![img](/home/pimiento/yap/linux.png)


# GIT

-   [GitHub](https://github.com)
-   [BitBucket](https://bitbucket.org)
-   [GitLab](https://about.gitlab.com/)
-   …


# GIT


## Время приключений!

![img](/home/pimiento/yap/adventure_time.jpg)


# .gitignore


## glob

```sh
mkdir /tmp/yap
cd /tmp/yap
python3 -m venv venv
cd /tmp/yap/venv
ls lib/*/*/*/*.py | head -n 5
```

    lib/python3.8/site-packages/pip/__init__.py
    lib/python3.8/site-packages/pip/__main__.py
    lib/python3.8/site-packages/pkg_resources/__init__.py
    lib/python3.8/site-packages/pkg_resources/py31compat.py
    lib/python3.8/site-packages/setuptools/archive_util.py


# .gitignore


## bash>     :B_block:

```sh
man 7 glob |head -n5
```


##       :B_ignoreheading:

    GLOB(7)                    Linux Programmer's Manual                   GLOB(7)

    NAME
           glob - globbing pathnames


## python>     :B_block:

```python
import glob
```


# Что внутри .git

![img](/home/pimiento/yap/dot_git_1.png)


# Что внутри .git

![img](/home/pimiento/yap/dot_git_2.png)


# Что внутри .git

![img](/home/pimiento/yap/dot_git_3.png)


# diff

![img](/home/pimiento/yap/dot_git_4.png)


# Commits

![img](/home/pimiento/yap/commits_1.png)


# Commits

![img](/home/pimiento/yap/commits_2.png)


# Commits

![img](//home/pimiento/yap/commits_3.png)


# Совместная разработка

![img](/home/pimiento/yap/centralized_workflow.png)


# Совместная разработка

![img](/home/pimiento/yap/small-team-flow.png)


# Branches

![img](/home/pimiento/yap/branch_1.png)


# Merge

![img](/home/pimiento/yap/merge_1.png)


# Merge

![img](/home/pimiento/yap/merge_2.png)


# Merge

![img](/home/pimiento/yap/workflow.png)


# Кто виноват?


## git blame

![img](/home/pimiento/yap/who.jpg)


# Кто виноват?


## git blame

```sh
git blame
```


# Откат изменений файла

\small{}

| HEAD                           | Снимок последнего коммита,    |
|                                | родитель следующего           |
| Индекс (Index)                 | Снимок следующего намеченного |
|                                | коммита                       |
| Рабочий каталог (Working tree) | Песочница                     |


# git reset

![img](/home/pimiento/yap/reset-soft.png)


# git reset

![img](/home/pimiento/yap/reset-mixed.png)


# git reset

![img](/home/pimiento/yap/reset-hard.png)


# git checkout


## git reset

<div class="org-center">
git reset &#x2013;hard [branch] file
</div>

Так не может быть, потому что *git reset* перемещает указатель HEAD, а он не может
указывать на несколько мест одновременно.


# git checkout


## git checkout

    git checkout [ --patch ] <hash> -- file

Замещает содержимое файла в текущем HEAD на содержимое из коммита <hash>.


# GIT. что почитать?


## Классика

<div class="org-center">
[GIT](https://git-scm.com/book/en/v2)
</div>


## Советую (english)

<div class="org-center">
[GIT Concepts and Workflows](https://vk.com/doc269223643_507620347?hash=f0724cb386dcc4da4a&dl=62be737793f7e270db)
</div>


# Спасибо!


## Задавайте ваши вопросы

![img](/home/pimiento/yap/questions.jpg)
