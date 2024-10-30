# Frage 1 The Shell 

Exercises
$ date --> Wed Oct 30 11:41:48     2024
$ whoami --> selia

Quiz
What should be outputted to the display when you type echo Hello World?
Hello World

# Frage 2 pwd (Print Working Directory)
$ pwd --> /c/Users/selia

no exercises

Quiz 
How do I find what directory you are currently in?
pwd

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

# Frage 5 touch 
$ ls -l superduperfile
-rw-r--r-- 1 ladmin 197121 0 Oct 30 14:46 superduperfile

Quiz 

How do you create a file called myfile?
touch myfile

# Frage 6 file

Exercises

Run the file command on a few different directories and files and note the output.
$ file DIS08_WS24_01_Introduction.pdf
DIS08_WS24_01_Introduction.pdf: PDF document, version 1.3, 8 page(s)

Quiz

What command can you use to find the file type of a file? --> file

# Frage 7 cat 


