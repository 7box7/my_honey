# ЛР №5
#### Сбудышева Людмила А-18-22
<br><br>



<p style="color: pink; font-weight: bold; font-size: 20px;">Часть 1</p>

---

#### 2. Изменить пароль (раsswd). Выполнить просмотр информации о работающих пользователях (who). 

```                                                                                                            
┌──(kali㉿kali)-[~]
└─$ passwd
Changing password for kali.
Current password: 
New password: 
Retype new password: 
The password has not been changed.
New password: 
Retype new password: 
You must choose a longer password.
New password: 
Retype new password: 
passwd: password updated successfully
```

```
┌──(kali㉿kali)-[~]
└─$ who
kali     tty7         2024-12-03 11:52 (:0)
```

---

#### 3. Познакомиться со справочным руководством (man). 

```
┌──(kali㉿kali)-[~]
└─$ man man
MAN(1)                                            Manual pager utils                                           MAN(1)

NAME
       man - an interface to the system reference manuals

SYNOPSIS
       man [man options] [[section] page ...] ...
       man -k [apropos options] regexp ...
       man -K [man options] [section] term ...
       man -f [whatis options] page ...
       man -l [man options] file ...
       man -w|-W [man options] page ...

DESCRIPTION
       man  is the system's manual pager.  Each page argument given to man is normally the name of a program, utility
       or function.  The manual page associated with each of these arguments is then found and displayed.  A section,
       if provided, will direct man to look only in that section of the manual.  The default action is to  search  in
       all  of  the  available sections following a pre-defined order (see DEFAULTS), and to show only the first page
       found, even if page exists in several sections.
```

> Описание команды - очень большое, чтобы полностью его вставить в отчет, поэтому вот маленький кусочек.

---

#### 4. В своем домашнем каталоге создать иерархическую 3-х уровневую структуру из 6-ти каталогов (например, каталог А с подкаталогами А1 и А2; в подкаталоге А1 создать подкаталоги А11 и А21; в подкаталоге А11 создать текстовые файлы file1.tхt и fіlе2.tхt и т.п.). 

```
┌──(kali㉿kali)-[~]
└─$ cd Desktop 
                                                                                                                      
┌──(kali㉿kali)-[~/Desktop]
└─$ mkdir -p A/A1/A11 A/A1/A21 A/A2                                                                                                                    
                                                                                                                      
┌──(kali㉿kali)-[~/Desktop]
└─$ echo "Hello World"             
Hello World
                                                                                                                      
┌──(kali㉿kali)-[~/Desktop]
└─$ echo "Hello World1" > A/A1/A11/file1.txt 
                                                                                                                      
┌──(kali㉿kali)-[~/Desktop]
└─$ echo "Hello World2" > A/A1/A11/file2.txt 
```

---

#### 5. Осуществить просмотр содержимого созданных файлов (саt, more). 

```
┌──(kali㉿kali)-[~/Desktop]
└─$ cat A/A1/A11/file1.txt 
Hello World1
```

> для того, чтобы увидеть различия в работе cat more, добавим в file2.txt побольше строчек Hello World2

```
┌──(kali㉿kali)-[~/Desktop]
└─$ echo "Hello World2" >> A/A1/A11/file2.txt 
```

```
┌──(kali㉿kali)-[~/Desktop]
└─$ cat A/A1/A11/file2.txt 
Hello World2
Hello World2
Hello World2
Hello World2
Hello World2
Hello World2
Hello World2
Hello World2
```

```
┌──(kali㉿kali)-[~/Desktop]
└─$ more A/A1/A11/file2.txt 
Hello World2
Hello World2
Hello World2
Hello World2
Hello World2
Hello World2
Hello World2
Hello World2
--More--(89%)
```

> cat выводит весь файл сразу, а more позволяет постранично просматривать большие файлы

---

#### 6. Создать файлы различных типов (саt, mкdіr, mknоd, ln). 

```
```

---

#### 7. Выполнить копирование, перемещение и удаление файлов и кaтaлoгов (cp, mv, rm, rmdir).

```
```

---

#### 8. Освоить команды: mкdіг, сhdіr, Іs, rm, рwd, раsswd в различных режимах (в частности, Іs в «коротком» (“‘Іs) и «длинном» (“‘Іs -аl') вариантах). 

```
```

---

#### 9. Изучить способ определения типов файлов в UNІХ и ознакомиться с командой filе. Изучить специальные типы файлов (файлы устройств). 

```
```

---

#### 10.Изучить средства создания ссылок в файловой системе (команда In). 

```
```

---

#### 11. Выполнить просмотр информации о файлах, изменение прав доступа и владельца файлов (Іs, сhmоd, сhоwn, сhgrр, umаsk).

```
```

---

#### 12. Назначить одному из файлов права. Убрать право “х", назначить "w". 

```
```

---

#### 13. Выполнить поиск файлов по различным критериям (fіnd).

```
```

---

#### 14. Отработать совместное использование каталогов: одному из пользователей зайти в домашний каталог другого, просмотреть созданную им структуру. Отредактировать файлы. 

```
```

---

#### 15. Удалить созданную структуру. 

```
```

---

#### 16. Просмотреть список процессов и информацию о процессах, установить поправки приоритета (рs, nісе). 

```
```

---

#### 17. Выполнить посылку сигналов процессам (kіll).

```
```

---

#### 18. Изучить средства переадресации ввода-вывода и конвейеризации команд интерпретатора. Записать в файл с именем текущей даты информацию о процессах, запущенных от имени пользователя.

```
```

---

#### 19. Получить справку по командам Іs, сhmоd.

```
```

---

#### 20. Изучить основные стандартные интерпретаторы (bаsh, сsh, ksh) и главные различия между ними.

```
```

---

#### 21. С помощью команды Windows ipconfig (используется из  командной строки windows) узнать IP-адреса локальных машин. Проверить, используя команду ping, проходят ли пакеты между  ними. С помощью traceroute (в версии Windows команда  называется tracert, используется таким же образом, как и в UNIX)  определить, каким образом – с участием сервера или без него – ходят пакеты между машинами. 

```
```

---

#### 22. Обменяться сообщениями электронной почты, используя  почтовую программу mail. 

```
```

---

#### 23. Завершить сеанс работы.
---
