```
In this exercise, you will be working with Lord of the Rings data. The dataset can be found on Kaggle.
Download and obtain the following CSV file: lotr_scripts.csv.
```
```
Document and describe the different data fields.

char: Contains character names, may include special formatting like parentheses.
dialog: Contains the spoken lines, sometimes with punctuation or formatting issues.
movie: Specifies the movie title.
```
```
Identify "dirty" data fields and clean them up. Use regex replace, spreadsheets, OpenRefine or whatever you like.

Example:
value.replace(" *","")
macht das leerzeichen vor dem Wort weg 
 Gandalf?  -> Gandalf?

value.trim()
entfernt zusätzliche leerzeichen

value.replace(/\s+/, " ")
Das entfernt führende/nachfolgende Leerzeichen und reduziert alle mehrfachen Leerzeichen auf ein einziges

value.replace(/\s+,/, ",").replace(/,\s+/, ", ")
alle Leerzeichen-Probleme auf einmal lösen

value.replace(/,{2,}/, ",")
doppeltes komma zu einem ersetzten

value.replace(/,\s*$/, "")
hinteres komma weg

value.replace(")", "")
) entfernen

value.replace(/,\s*Caught/, " Caught")
komma vor caught entfernen

```
````
Document your working steps in a Markdown-formatted file. Export your dataset as a clean CSV file. Add both files to this repository (in this directory).
Analyze the data set using shell scripts and/or regex. Document the commands in an additional section in your Markdown-formatted file.
Find the total number of lines and unique words used in the dialogs.
What is the distribution on the three different films?
What are the top 5 characters in the char column?
What are the top 5 characters in the dialogues?
```
