- [Timestamp](#orgc4916a2)
  - [Что такое timestamp?](#org04bd766)
- [Timestamp](#orgd24d26e)
  - [Что такое timestamp?](#org9dfaa80)
- [Timestamp](#orgc8921f2)
  - [Что такое timestamp?](#orgd420669)
- [Timestamp](#orgccdc86a)
  - [Что такое timestamp?](#orgdbe7ca9)
- [Timestamp](#org1f9985a)
  - [Что такое timestamp?](#org60d0b26)
- [UNIX](#org2f22521)
  - [1970.1.1](#org64e1041)
- [UNIX](#org6b19dc6)
- [Shell](#org8430f32)
- [Основные команды Bash (sh, zsh)](#orgbe1345c)
  - [ls](#org87159b9)
- [Основные команды Bash (sh, zsh)](#org1b75e7f)
  - [ls -l](#orgc95d646)
- [Основные команды Bash (sh, zsh)](#org0ea596d)
  - [ls -a](#orgbc355c3)
- [Основные команды Bash (sh, zsh)](#orgc1bb388)
  - [which](#orgbc2e119)
- [Основные команды Bash (sh, zsh)](#org0a57049)
  - [mkdir](#org5777720)
- [Основные команды Bash (sh, zsh)](#org08a1ec0)
  - [rm](#org78461de)
- [Основные команды Bash (sh, zsh)](#org2763db5)
  - [grep](#orgb4d14f5)
- [Основные команды Bash (sh, zsh)](#org27269cd)
  - [cat](#orga1a470b)
- [Основные команды Bash (sh, zsh)](#orgb050b4c)
  - [перенаправление](#orgb4631e4)
- [Основные команды Bash (sh, zsh)](#org40b2eab)
  - [перенаправление](#org465c171)
- [Основные команды Bash (sh, zsh)](#orgf6aa581)
  - [pipe](#org29c1101)
- [Основные команды Bash (sh, zsh)](#orgb7575f6)
  - [Время стать крутыми хакерами!](#org6483470)
- [UNIX это интересно!](#org3ac0afb)
- [#!/usr/bin/env python](#org575d47b)
  - [hello.py](#org3eec78d)
  - [$>](#orga450d30)
- [Что почитать?](#org8545c3e)
  - [Про UNIX идеологию в целом](#orgf58da7b)
  - [Bash](#orgb2fe5b5)
- [SSH](#org2670d84)
- [VI](#org4f701a1)
- [VI](#orge4503af)
- [Linux. При чём тут GIT?](#org10c55c1)
- [GIT](#orge3f7cc4)
- [GIT](#orgf4e7edb)
  - [Время приключений!](#org13530c0)
- [.gitignore](#org3a83580)
  - [glob](#orgccdb85a)
- [.gitignore](#org63a4a1c)
  - [bash>](#org59de4db)
  - [ ](#orgc702f70)
  - [python>](#orgd39705d)
- [Что внутри .git](#org32bba30)
- [Что внутри .git](#org497fadb)
- [Что внутри .git](#orga4de8fe)
- [diff](#orgfbf36d1)
- [Commits](#orgeedabe3)
- [Commits](#org2f926da)
- [Commits](#org9141e65)
- [Совместная разработка](#orgfc2e463)
- [Совместная разработка](#org6ee13d0)
- [Branches](#orgad2121e)
- [Merge](#org29a5e23)
- [Merge](#orgcd71f9e)
- [Merge](#orgfe0bde4)
- [Кто виноват?](#org37981c3)
  - [git blame](#org2a53ea1)
- [Кто виноват?](#org509d12e)
  - [git blame](#orgaf8c733)
- [Откат изменений файла](#orgb2e039d)
- [git reset](#org16abf07)
- [git reset](#orgba0a5da)
- [git reset](#org443eae1)
- [git checkout](#orgb4c2b42)
  - [git reset](#orgc19bc0f)
- [git checkout](#org14a0f10)
  - [git checkout](#orgf4a16ed)
- [GIT. что почитать?](#orgb8f3299)
  - [Классика](#org87d82b5)
  - [Советую (english)](#orga0e7578)
- [Спасибо!](#org8926bdd)
  - [Задавайте ваши вопросы](#org4bd9277)



<a id="orgc4916a2"></a>

# Timestamp


<a id="org04bd766"></a>

## Что такое timestamp?

```python
import time

print(time.time())
```


<a id="orgd24d26e"></a>

# Timestamp


<a id="org9dfaa80"></a>

## Что такое timestamp?

```python
import time

print(time.time())
```

    1648836033.276411


<a id="orgc8921f2"></a>

# Timestamp


<a id="orgd420669"></a>

## Что такое timestamp?

```python
import time
from datetime import datetime

t = time.time()
print(
  datetime.utcfromtimestamp(t)
)
```

    2022-04-01 18:00:33.320419


<a id="orgccdc86a"></a>

# Timestamp


<a id="orgdbe7ca9"></a>

## Что такое timestamp?

А что будет если вызвать такой код?

```python
from datetime import datetime

print(
  datetime.utcfromtimestamp(0)
)
```


<a id="org1f9985a"></a>

# Timestamp


<a id="org60d0b26"></a>

## Что такое timestamp?

```python
from datetime import datetime

print(
  datetime.utcfromtimestamp(0)
)
```

    1970-01-01 00:00:00


<a id="org2f22521"></a>

# UNIX


<a id="org64e1041"></a>

## 1970.1.1

**Дата отсчёта UNIX-эпохи**

![img](/home/pimiento/yap/thompson_n_ritchi.jpeg)


<a id="org6b19dc6"></a>

# UNIX

<span class="underline">Главные принципы UNIX</span>:

-   Всё есть файл (ну или почти всё)
-   Каждая программа должна уметь делать ****только одно**** и делать это хорошо!

****UNIX-way****


<a id="org8430f32"></a>

# Shell

-   *sh*
-   *bash*
-   *zsh*
-   csh
-   fish
-   ksh
-   tcsh


<a id="orgbe1345c"></a>

# Основные команды Bash (sh, zsh)


<a id="org87159b9"></a>

## ls

```sh
ls ~/workdir/generate-password/
```

    gen_pass
    README


<a id="org1b75e7f"></a>

# Основные команды Bash (sh, zsh)


<a id="orgc95d646"></a>

## ls -l

```sh
ls -l ~/workdir/generate-password/
```

    total 8
    drwxr-xr-x 3 pimiento pimiento 4096 Jun 12  2021
    gen_pass
    -rw-r--r-- 1 pimiento pimiento  420 Apr 13  2021
    README


<a id="org0ea596d"></a>

# Основные команды Bash (sh, zsh)


<a id="orgbc355c3"></a>

## ls -a

```sh
ls -a ~/workdir/generate-password/
```

    .
    ..
    gen_pass
    .git
    README


<a id="orgc1bb388"></a>

# Основные команды Bash (sh, zsh)


<a id="orgbc2e119"></a>

## which

```sh
which python3
```

    /usr/bin/python3


<a id="org0a57049"></a>

# Основные команды Bash (sh, zsh)


<a id="org5777720"></a>

## mkdir

```sh
mkdir /tmp/notexist
```


<a id="org08a1ec0"></a>

# Основные команды Bash (sh, zsh)


<a id="org78461de"></a>

## rm

```sh
rm -r /tmp/notexist
```


<a id="org2763db5"></a>

# Основные команды Bash (sh, zsh)


<a id="orgb4d14f5"></a>

## grep

```sh
grep pimiento /etc/passwd
```

    pimiento:x:1000:1000:Pavel
    Vavilin,,,:/home/pimiento:/bin/zsh


<a id="org27269cd"></a>

# Основные команды Bash (sh, zsh)


<a id="orga1a470b"></a>

## cat

```sh
cat /etc/lsb-release
```

    DISTRIB_ID=LinuxMint
    DISTRIB_RELEASE=20.3
    DISTRIB_CODENAME=una
    DISTRIB_DESCRIPTION="Linux Mint 20.3 Una"


<a id="orgb050b4c"></a>

# Основные команды Bash (sh, zsh)


<a id="orgb4631e4"></a>

## перенаправление

-   0 => stdin
-   1 => stdout
-   2 => stderr


<a id="org40b2eab"></a>

# Основные команды Bash (sh, zsh)


<a id="org465c171"></a>

## перенаправление

```sh
rm -r /tmp/notexist 2> /tmp/rm.log
cat /tmp/rm.log
```

    rm: cannot remove '/tmp/notexist': No such file
    or directory


<a id="orgf6aa581"></a>

# Основные команды Bash (sh, zsh)


<a id="org29c1101"></a>

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


<a id="orgb7575f6"></a>

# Основные команды Bash (sh, zsh)

```sh
cat /dev/urandom | hexdump -c
```


<a id="org6483470"></a>

## Время стать крутыми хакерами!

![img](/home/pimiento/yap/matrix.png)


<a id="org3ac0afb"></a>

# UNIX это интересно!

![img](/home/pimiento/yap/unix.jpg)


<a id="org575d47b"></a>

# #!/usr/bin/env python

Шебэнг? Шебанг? Shebang.


<a id="org3eec78d"></a>

## hello.py

```sh
#!/usr/bin/env python3

print("Hello World!")
```


<a id="orga450d30"></a>

## $>

```sh
chmod +x hello.py
```


<a id="org8545c3e"></a>

# Что почитать?


<a id="orgf58da7b"></a>

## Про UNIX идеологию в целом

Брайн Керниган, Роб Пайк «Программное окружение UNIX»


<a id="orgb2fe5b5"></a>

## Bash

<span class="underline"><span class="underline">«[Advanced Bash-Scripting Guide](https://tldp.org/LDP/abs/html/)»</span></span>. На OpenNet можно найти <span class="underline"><span class="underline">[перевод](https://www.opennet.ru/docs/RUS/bash_scripting_guide/index.html)</span></span>


<a id="org2670d84"></a>

# SSH

( *В MS Windows чаще всего используют **PuTTY*** )

```sh
ssh user@ya.ru
```



```sh
scp user@ya.ru:/answers.txt ./
```


<a id="org4f701a1"></a>

# VI

Редактор де-факто на всех UNIX-like системах
![img](/home/pimiento/yap/vim.jpg)


<a id="orge4503af"></a>

# VI

<div class="org-center">
<span class="underline"><span class="underline">[МЕМАСИКИ](https://yandex.ru/images/search?text=vim%20%D0%BC%D0%B5%D0%BC%D1%8B&from=tabbar)</span></span>
</div>


*шпаргалку по Vi/Vim пришлю после вебинара*


<a id="org10c55c1"></a>

# Linux. При чём тут GIT?

![img](/home/pimiento/yap/linux.png)


<a id="orge3f7cc4"></a>

# GIT

-   [GitHub](https://github.com)
-   [BitBucket](https://bitbucket.org)
-   [GitLab](https://about.gitlab.com/)
-   …


<a id="orgf4e7edb"></a>

# GIT


<a id="org13530c0"></a>

## Время приключений!

![img](/home/pimiento/yap/adventure_time.jpg)


<a id="org3a83580"></a>

# .gitignore


<a id="orgccdb85a"></a>

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


<a id="org63a4a1c"></a>

# .gitignore


<a id="org59de4db"></a>

## bash>     :B_block:

```sh
man 7 glob |head -n5
```


<a id="orgc702f70"></a>

##       :B_ignoreheading:

    GLOB(7)                    Linux Programmer's Manual                   GLOB(7)

    NAME
           glob - globbing pathnames


<a id="orgd39705d"></a>

## python>     :B_block:

```python
import glob
```


<a id="org32bba30"></a>

# Что внутри .git

![img](/home/pimiento/yap/dot_git_1.png)


<a id="org497fadb"></a>

# Что внутри .git

![img](/home/pimiento/yap/dot_git_2.png)


<a id="orga4de8fe"></a>

# Что внутри .git

![img](/home/pimiento/yap/dot_git_3.png)


<a id="orgfbf36d1"></a>

# diff

![img](/home/pimiento/yap/dot_git_4.png)


<a id="orgeedabe3"></a>

# Commits

![img](/home/pimiento/yap/commits_1.png)


<a id="org2f926da"></a>

# Commits

![img](/home/pimiento/yap/commits_2.png)


<a id="org9141e65"></a>

# Commits

![img](//home/pimiento/yap/commits_3.png)


<a id="orgfc2e463"></a>

# Совместная разработка

![img](/home/pimiento/yap/centralized_workflow.png)


<a id="org6ee13d0"></a>

# Совместная разработка

![img](/home/pimiento/yap/small-team-flow.png)


<a id="orgad2121e"></a>

# Branches

![img](/home/pimiento/yap/branch_1.png)


<a id="org29a5e23"></a>

# Merge

![img](/home/pimiento/yap/merge_1.png)


<a id="orgcd71f9e"></a>

# Merge

![img](/home/pimiento/yap/merge_2.png)


<a id="orgfe0bde4"></a>

# Merge

![img](/home/pimiento/yap/workflow.png)


<a id="org37981c3"></a>

# Кто виноват?


<a id="org2a53ea1"></a>

## git blame

![img](/home/pimiento/yap/who.jpg)


<a id="org509d12e"></a>

# Кто виноват?


<a id="orgaf8c733"></a>

## git blame

```sh
git blame
```


<a id="orgb2e039d"></a>

# Откат изменений файла

\small{}

| HEAD                           | Снимок последнего коммита,    |
|                                | родитель следующего           |
| Индекс (Index)                 | Снимок следующего намеченного |
|                                | коммита                       |
| Рабочий каталог (Working tree) | Песочница                     |


<a id="org16abf07"></a>

# git reset

![img](/home/pimiento/yap/reset-soft.png)


<a id="orgba0a5da"></a>

# git reset

![img](/home/pimiento/yap/reset-mixed.png)


<a id="org443eae1"></a>

# git reset

![img](/home/pimiento/yap/reset-hard.png)


<a id="orgb4c2b42"></a>

# git checkout


<a id="orgc19bc0f"></a>

## git reset

<div class="org-center">
git reset &#x2013;hard [branch] file
</div>

Так не может быть, потому что *git reset* перемещает указатель HEAD, а он не может
указывать на несколько мест одновременно.


<a id="org14a0f10"></a>

# git checkout


<a id="orgf4a16ed"></a>

## git checkout

    git checkout [ --patch ] <hash> -- file

Замещает содержимое файла в текущем HEAD на содержимое из коммита <hash>.


<a id="orgb8f3299"></a>

# GIT. что почитать?


<a id="org87d82b5"></a>

## Классика

<div class="org-center">
[GIT](https://git-scm.com/book/en/v2)
</div>


<a id="orga0e7578"></a>

## Советую (english)

<div class="org-center">
[GIT Concepts and Workflows](https://vk.com/doc269223643_507620347?hash=f0724cb386dcc4da4a&dl=62be737793f7e270db)
</div>


<a id="org8926bdd"></a>

# Спасибо!


<a id="org4bd9277"></a>

## Задавайте ваши вопросы

![img](/home/pimiento/yap/questions.jpg)
