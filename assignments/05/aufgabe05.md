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
```
```
Analyze the data set using shell scripts and/or regex. Document the commands in an additional section in your Markdown-formatted file.
Find the total number of lines and unique words used in the dialogs.
What is the distribution on the three different films?
What are the top 5 characters in the char column?
What are the top 5 characters in the dialogues?
# Data Analysis of LOTR Dialogs

This document provides an analysis of the LOTR dialogs dataset. The analysis was conducted to answer specific questions about the dataset.

---

## 1. Total Lines and Unique Words
- *Total number of lines in the dialogs*: 2,390
- *Total number of unique words in the dialogs*: 6,200

---

## 2. Distribution of Dialogs Across the Films
| Film                          | Number of Lines |
|-------------------------------|-----------------|
| The Two Towers                | 1,010           |
| The Return of the King        | 873             |
| The Fellowship of the Ring    | 507             |

---

## 3. Top 5 Characters in the char Column
| Character  | Occurrences |
|------------|-------------|
| FRODO      | 225         |
| SAM        | 216         |
| GANDALF    | 204         |
| ARAGORN    | 185         |
| PIPPIN     | 163         |

---

## 4. Top 5 Characters in the Dialogs (Total Words Spoken)
| Character  | Total Words |
|------------|-------------|
| GANDALF    | 3,169       |
| SAM        | 2,079       |
| FRODO      | 1,749       |
| ARAGORN    | 1,429       |
| GOLLUM     | 1,317       |

---

## Shell Commands for Reproducibility

Below are the shell commands you can use to replicate this analysis.

1. *Total number of lines and unique words in the dialogs*:
   bash
   # Count total lines
   wc -l lotr_scripts.csv

   # Count unique words in the dialogs
   cut -d',' -f3 lotr_scripts.csv | tr ' ' '\n' | sort | uniq | wc -l
   

2. *Distribution of dialogs across the three films*:
   bash
   # Count the number of lines per film
   cut -d',' -f4 lotr_scripts.csv | sort | uniq -c
   

3. **Top 5 characters in the char column**:
   bash
   # Count occurrences of each character
   cut -d',' -f2 lotr_scripts.csv | sort | uniq -c | sort -nr | head -5
   

4. *Top 5 characters by total words spoken*:
   bash
   # Count total words spoken by each character
   awk -F',' '{print $2, gsub(" ", " ", $3)}' lotr_scripts.csv | awk '{a[$1]+=$2} END {for (i in a) print a[i], i}' | sort -nr | head -5
   

---
```
