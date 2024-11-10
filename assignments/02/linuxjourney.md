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
clear
```
```
# Frage 10 cp (Copy)
Exercises
Copy over a couple of files, be careful not to overwrite anything important.
ladmin@SLY-SBOOK3 MINGW64 /c/Users/selia/OneDrive/th köln/3 Semester/DIS08 DatenmodellierungData Modelling
$ cp textfile.txt /c/Users/selia/OneDrive/th\ köln/3\ Semester


Quiz
What flag do you need to specify to copy over a directory?
-r
```
```
#Frage 11
Exercises
Rename a file, then move that file to a different directory.

ladmin@SLY-SBOOK3 MINGW64 /c/Users/selia/OneDrive/th köln/3 Semester/DIS08 DatenmodellierungData Modelling
$ mv textfile.txt textfile2.txt
ladmin@SLY-SBOOK3 MINGW64 /c/Users/selia/OneDrive/th köln/3 Semester/DIS08 DatenmodellierungData Modelling
$ mv textfile2.txt /c/Users/selia/OneDrive/th\ köln/3\ Semester
ladmin@SLY-SBOOK3 MINGW64 /c/Users/selia/OneDrive/th köln/3 Semester/DIS08 DatenmodellierungData Modelling
$ mv ../textfile2.txt /c/Users/selia/OneDrive/th\ köln/3\ Semester/DIS08\ DatenmodellierungData\ Modelling

Quiz
How do you rename a file called cat to dog?
mv cat dog
```
```
# Frage 12 mkdir (Make Directory)
Exercises
Make a couple of directories and move some files into that directory.

ladmin@SLY-SBOOK3 MINGW64 /c/Users/selia/OneDrive/th köln/3 Semester/DIS08 DatenmodellierungData Modelling
$ mkdir wichtig

Quiz
What command is use to make a directory?
mkdir
```
```
# Frage 13 rm (Remove)
Exercises
Create a file called -file (don't forget the dash!).
Remove that file.
ladmin@SLY-SBOOK3 MINGW64 /c/Users/selia/OneDrive/th köln/3 Semester/DIS08 DatenmodellierungData Modelling
$ touch eliane.txt

ladmin@SLY-SBOOK3 MINGW64 /c/Users/selia/OneDrive/th köln/3 Semester/DIS08 DatenmodellierungData Modelling
$ rm eliane.txt

Quiz
How do you remove a file called myfile?
rm myfile
```
```
# Frage 14 find
Exercises
Find a file from the root directory that has the word net in it.
ladmin@SLY-SBOOK3 MINGW64 /c/Users/selia/OneDrive/th köln/3 Semester/DIS08 DatenmodellierungData Modelling
$ find /d -name net
/d/phyton/Library/include/aws/core/net
/d/phyton/pkgs/aws-sdk-cpp-1.10.55-hd77b12b_0/Library/include/aws/core/net

Quiz
What option should I specify for find if I want to search by name?
-name
```
```
# frage 15 help
Exercises
Run help on the echo command, logout command and pwd command.

$ help echo
echo: echo [-neE] [arg ...]
    Write arguments to the standard output.

    Display the ARGs, separated by a single space character and followed by a
    newline, on the standard output.

    Options:
      -n        do not append a newline
      -e        enable interpretation of the following backslash escapes
      -E        explicitly suppress interpretation of backslash escapes

    `echo' interprets the following backslash-escaped characters:
      \a        alert (bell)
      \b        backspace
      \c        suppress further output
      \e        escape character
      \E        escape character
      \f        form feed
      \n        new line
      \r        carriage return
      \t        horizontal tab
      \v        vertical tab
      \\        backslash
      \0nnn     the character whose ASCII code is NNN (octal).  NNN can be
                0 to 3 octal digits
      \xHH      the eight-bit character whose value is HH (hexadecimal).  HH
                can be one or two hex digits
      \uHHHH    the Unicode character whose value is the hexadecimal value HHHH.
                HHHH can be one to four hex digits.
      \UHHHHHHHH the Unicode character whose value is the hexadecimal value
                HHHHHHHH. HHHHHHHH can be one to eight hex digits.

    Exit Status:
    Returns success unless a write error occurs.

$ help logout
logout: logout [n]
    Exit a login shell.

    Exits a login shell with exit status N.  Returns an error if not executed
    in a login shell.

$ help pwd
pwd: pwd [-LPW]
    Print the name of the current working directory.

    Options:
      -L        print the value of $PWD if it names the current working
                directory
      -P        print the physical directory, without any symbolic links
      -W        print the Win32 value of the physical directory

    By default, `pwd' behaves as if `-L' were specified.

    Exit Status:
    Returns 0 unless an invalid option is given or the current directory
    cannot be read.

Quiz
How do you get quick command line help for built-in bash commands?
help
```
```
# Frage 16 ls
Exercises
Run the man command on the ls command.

unfortionally the man ls command ist not working on windows, thats why i used th ls--help command and this is what came out oft that: $ ls --help
Usage: ls [OPTION]... [FILE]...
List information about the FILEs (the current directory by default).
Sort entries alphabetically if none of -cftuvSUX nor --sort is specified.

Mandatory arguments to long options are mandatory for short options too.
  -a, --all                  do not ignore entries starting with .
  -A, --almost-all           do not list implied . and ..
      --author               with -l, print the author of each file
  -b, --escape               print C-style escapes for nongraphic characters
      --block-size=SIZE      with -l, scale sizes by SIZE when printing them;
                               e.g., '--block-size=M'; see SIZE format below
  -B, --ignore-backups       do not list implied entries ending with ~
  -c                         with -lt: sort by, and show, ctime (time of last
                               modification of file status information);
                               with -l: show ctime and sort by name;
                               otherwise: sort by ctime, newest first
  -C                         list entries by columns
      --color[=WHEN]         colorize the output; WHEN can be 'always' (default
                               if omitted), 'auto', or 'never'; more info below
  -d, --directory            list directories themselves, not their contents
  -D, --dired                generate output designed for Emacs' dired mode
  -f                         do not sort, enable -aU, disable -ls --color
  -F, --classify             append indicator (one of */=>@|) to entries
      --file-type            likewise, except do not append '*'
      --format=WORD          across -x, commas -m, horizontal -x, long -l,
                               single-column -1, verbose -l, vertical -C
      --full-time            like -l --time-style=full-iso
  -g                         like -l, but do not list owner
      --group-directories-first
                             group directories before files;
                               can be augmented with a --sort option, but any
                               use of --sort=none (-U) disables grouping
  -G, --no-group             in a long listing, don't print group names
  -h, --human-readable       with -l and -s, print sizes like 1K 234M 2G etc.
      --si                   likewise, but use powers of 1000 not 1024
  -H, --dereference-command-line
                             follow symbolic links listed on the command line
      --dereference-command-line-symlink-to-dir
                             follow each command line symbolic link
                               that points to a directory
      --hide=PATTERN         do not list implied entries matching shell PATTERN
                               (overridden by -a or -A)
      --hyperlink[=WHEN]     hyperlink file names; WHEN can be 'always'
                               (default if omitted), 'auto', or 'never'
      --indicator-style=WORD  append indicator with style WORD to entry names:
                               none (default), slash (-p),
                               file-type (--file-type), classify (-F)
  -i, --inode                print the index number of each file
  -I, --ignore=PATTERN       do not list implied entries matching shell PATTERN
  -k, --kibibytes            default to 1024-byte blocks for disk usage;
                               used only with -s and per directory totals
  -l                         use a long listing format
  -L, --dereference          when showing file information for a symbolic
                               link, show information for the file the link
                               references rather than for the link itself
  -m                         fill width with a comma separated list of entries
  -n, --numeric-uid-gid      like -l, but list numeric user and group IDs
  -N, --literal              print entry names without quoting
  -o                         like -l, but do not list group information
  -p, --indicator-style=slash
                             append / indicator to directories
  -q, --hide-control-chars   print ? instead of nongraphic characters
      --show-control-chars   show nongraphic characters as-is (the default,
                               unless program is 'ls' and output is a terminal)
  -Q, --quote-name           enclose entry names in double quotes
      --quoting-style=WORD   use quoting style WORD for entry names:
                               literal, locale, shell, shell-always,
                               shell-escape, shell-escape-always, c, escape
                               (overrides QUOTING_STYLE environment variable)
  -r, --reverse              reverse order while sorting
  -R, --recursive            list subdirectories recursively
  -s, --size                 print the allocated size of each file, in blocks
  -S                         sort by file size, largest first
      --sort=WORD            sort by WORD instead of name: none (-U), size (-S),
                               time (-t), version (-v), extension (-X)
      --time=WORD            change the default of using modification times;
                               access time (-u): atime, access, use;
                               change time (-c): ctime, status;
                               birth time: birth, creation;
                             with -l, WORD determines which time to show;
                             with --sort=time, sort by WORD (newest first)
      --time-style=TIME_STYLE  time/date format with -l; see TIME_STYLE below
  -t                         sort by time, newest first; see --time
  -T, --tabsize=COLS         assume tab stops at each COLS instead of 8
  -u                         with -lt: sort by, and show, access time;
                               with -l: show access time and sort by name;
                               otherwise: sort by access time, newest first
  -U                         do not sort; list entries in directory order
  -v                         natural sort of (version) numbers within text
  -w, --width=COLS           set output width to COLS.  0 means no limit
  -x                         list entries by lines instead of by columns
  -X                         sort alphabetically by entry extension
  -Z, --context              print any security context of each file
  -1                         list one file per line.  Avoid '\n' with -q or -b
      --append-exe           append .exe if cygwin magic was needed
      --help     display this help and exit
      --version  output version information and exit

The SIZE argument is an integer and optional unit (example: 10K is 10*1024).
Units are K,M,G,T,P,E,Z,Y (powers of 1024) or KB,MB,... (powers of 1000).
Binary prefixes can be used, too: KiB=K, MiB=M, and so on.

The TIME_STYLE argument can be full-iso, long-iso, iso, locale, or +FORMAT.
FORMAT is interpreted like in date(1).  If FORMAT is FORMAT1<newline>FORMAT2,
then FORMAT1 applies to non-recent files and FORMAT2 to recent files.
TIME_STYLE prefixed with 'posix-' takes effect only outside the POSIX locale.
Also the TIME_STYLE environment variable sets the default style to use.

Using color to distinguish file types is disabled both by default and
with --color=never.  With --color=auto, ls emits color codes only when
standard output is connected to a terminal.  The LS_COLORS environment
variable can change the settings.  Use the dircolors command to set it.

Exit status:
 0  if OK,
 1  if minor problems (e.g., cannot access subdirectory),
 2  if serious trouble (e.g., cannot access command-line argument).

GNU coreutils online help: <https://www.gnu.org/software/coreutils/>
Report any translation bugs to <https://translationproject.org/team/>
Full documentation <https://www.gnu.org/software/coreutils/ls>
or available locally via: info '(coreutils) ls invocation'


and I also just ran the ls command by it self:
$ ls
 DIS08_WS24_01_Introduction.pdf   git                  textfile2.txt
 elianefile                      'git bash pfad.txt'   wichtig/



Quiz
How do you see the manuals for a command?
man
```
```
# Frage 17











