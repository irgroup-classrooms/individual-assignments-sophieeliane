```
# Frage 1 The Shell 

Exercises
$ date --> Wed Oct 30 11:41:48     2024
$ whoami --> selia

Quiz
What should be outputted to the display when you type echo Hello World?
Hello World
```
```
# Frage 2 pwd (Print Working Directory)
$ pwd --> /c/Users/selia

no exercises

Quiz 
How do I find what directory you are currently in?
pwd
```
```
# Frage 3 cd (Change Directory)

Exercises

Run the cd command without any flags, where does it take you?
selia@SLY-SBOOK3 MINGW64 ~
$ cd .

selia@SLY-SBOOK3 MINGW64 ~
$ cd ..

selia@SLY-SBOOK3 MINGW64 /c/Users
$ cd ~

selia@SLY-SBOOK3 MINGW64 ~
$ cd -
/c/Users

only the ~ and - is working in my gitbash 

Quiz

If you are in /home/pete/Pictures and wanted to go to /home/pete, what’s a good shortcut to use?

cd ..
```
```
# Frage 4

Exercises
Run ls with different flags and see the output you receive.

ls -R: recursively list directory contents --> opens every file 
ls -r: reverse order while sorting --> $ ls -r
 selia/    desktop.ini  'Default User'@  'All Users'@
 ladmin/   Public/       Default/

ls -t: sort by modification time, newest first --> $ ls -t
 ladmin/   Default/  'Default User'@   desktop.ini
 selia/    Public/   'All Users'@


Flags like -R, -r, and -t customize how ls shows the contents of a directory, making it easier to find what you need based on structure, order, or time. You can use one flag at a time or combine them for specific effects.

Quiz 
What command would you use to see hidden files? --> ls -a
```
```
# Frage 5 touch 
$ ls -l superduperfile
-rw-r--r-- 1 ladmin 197121 0 Oct 30 14:46 superduperfile

Quiz 

How do you create a file called myfile?
touch myfile
```
```
# Frage 6 file

Exercises

Run the file command on a few different directories and files and note the output.
$ file DIS08_WS24_01_Introduction.pdf
DIS08_WS24_01_Introduction.pdf: PDF document, version 1.3, 8 page(s)

Quiz

What command can you use to find the file type of a file? --> file
```
```
# Frage 7 cat
Excersice
Run cat on different files and directories. Then try to cat multiple files.
ladmin@SLY-SBOOK3 MINGW64 /c/Users/selia/OneDrive/th köln/3 Semester/DIS08 DatenmodellierungData Modelling
$ echo "hallo" > textfile.txt

ladmin@SLY-SBOOK3 MINGW64 /c/Users/selia/OneDrive/th köln/3 Semester/DIS08 DatenmodellierungData Modelling
$ cat textfile.txt
hallo

Quiz
What's a good way to see the contents of a file?
cat
```
```
# Frage 8 less
Exercises
Run less on a file, then page up and around the file. Try searching for a specific word. Quickly navigate to the beginning or the end of the file.
ladmin@SLY-SBOOK3 MINGW64 /c/Users/selia/OneDrive/th köln/3 Semester/DIS08 DatenmodellierungData Modelling
$ less textfile.txt

q - Used to quit out of less and go back to your shell.
Page up, Page down, Up and Down - Navigate using the arrow keys and page keys.
g - Moves to beginning of the text file.
G - Moves to the end of the text file.
/search - You can search for specific text inside the text document. Prefacing the words you want to search with /
h - If you need a little help about how to use less while you’re in less, use help.

Quiz
How do you quit out of a less command?
q
```
```
# Frage 9 history
Exercises
Navigate through your previous command history with the Up and Down keys. Play around with ctrl-R reverse search.

$ history
    1  pwd
    2  touch test.txt
    3  echo Hello World
    4  date
    5  whoami
    6  pwd
    7  cd .
    8  cd ..
    9  cd ~
   10  cd -
   11  cd
   12  ls -R
   13  clear
   14  ls -r
   15  touch superduperfile
   16  ls -l
   17  ls -l superduperfile
   18  cd /c/Users/selia/OneDrive/th\ köln/3\ Semester/DIS08\ DatenmodellierungData\ Modelling
   19  touch superduperfile
   20  cd /c/Users/selia/OneDrive/th\ köln/3\ Semester/DIS08\ DatenmodellierungData\ Modelling
   21  $ ls -l superduperfile
   22  ls -l superduperfile
   23  file banana,jpg
   24  file.jpg
   25  file banana.jpg
   26  cd ~
   27  cd /c/Users/selia/OneDrive/th\ köln/3\ Semester/DIS08\ DatenmodellierungData\ Modelling
   28  file DIS08_WS24_01_Introduction.pdf
   29  cat DIS08_WS24_01_Introduction.pdf
   30  64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c;1;120;120;1;0x64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c64;1;2;4;6;9;11;15;21;22;28;29c
   31  cd /c/Users/selia/OneDrive/th\ köln/3\ Semester/DIS08\ DatenmodellierungData\ Modelling
   32  cd -
   33  cd /c/Users/selia/OneDrive/th\ köln/3\ Semester/DIS08\ DatenmodellierungData\ Modelling
   34  cd .
   35  cd ..
   36  cat DIS13 Datenbanksysteme
   37  cat DIS13\Datenbanksysteme
   38  cd ~
   39  cd /c/Users/selia/OneDrive/th\ köln/3\ Semester/DIS08\ DatenmodellierungData\ Modelling
   40  less
   41  less /c/Users/selia/OneDrive/th köln/3 Semester/DIS08 DatenmodellierungData Modelling
   42  less OneDrive/th köln/3 Semester/DIS08 DatenmodellierungData Modelling
   43  q-
   44  q
   45  less q
   46  less g
   47  Page up
   48  less /c/Users/selia/OneDrive/th köln/3 Semester/DIS11 Informationssysteme - Content­- & Dokumentenmanagementsysteme
   49  less /c/Users/selia/OneDrive/th köln/3 Semester/DIS11 Informationssysteme - Content­- & Dokumentenmanagementsysteme/DIS 11 Informationssysteme 15.10.24
   50  less /C/Users/selia/OneDrive/th köln/2 Semester/Lepsky/Lepsky
   51  history
   52  clear
   53  history
   54  mv superduperfile elianefile
   55  mv elianefile /c/Users/selia/OneDrive/th köln/3 Semester
   56  cd /c/Users/selia/OneDrive/th\ köln/3\ Semester/DIS08\ DatenmodellierungData\ Modelling
   57  touch elianefile
   58  echo "hallo" > git bash pfad.txt
   59  cat git bash pfad.txt
   60  echo "hallo" > textfile.txt
   61  cat textfile.txt
   62  less textfile.txt
   63  q
   64  less textfile.txt
   65  less textfile.txt
   66  less textfile.txt
   67  history

Quiz
What is the command to clear the terminal?



