
# Shell-odessy-Processing 
---
## Content Info
- LINK= [The Odysse](http://classics.mit.edu/Homer/odyssey.mb.txt) is a book on greek mythiology where a war hero, Odysses takes 10 years to come back home from the Trojan war.

---
### Commands

  

-  **curl** : retrieves all the contents of a web page. 
 ```curl http://classics.mit.edu/Homer/odyssey.mb.txt``` will get all the contents of this page.

  

-  **-O flag** : will save to a file. 
 ```curl http://classics.mit.edu/Homer/odyssey.mb.txt -O odessy.txt``` will save text received from ```curl http://classics.mit.edu/Homer/odyssey.mb.txt``` to odessy.txt.

  

-  **tr command** : will transform one text to other.
 ```tr ' ' '\12'``` will transform space " " into ascii code \12 which is new line.

  

-  **Redirection (<)** : will take input from a file.
 ```tr ' ' '\12' < odessy.txt``` will take input from the file odessy.txt and will feed to ```tr ' ' '\12'```.

  

-  **Pipe ( | )** : will send the results of one command as input into another command. 
 ```tr ' ' '\12' < odessy.txt | sort``` will take input from ```tr ' ' '\12' < odessy.txt``` and pass it to sort command.

  

-  **Sort** : will sort the values in increasing order.
 ```tr ' ' '\12' < odessy.txt | sort``` will take input from ```tr ' ' '\12' < odessy.txt``` and sort them in increasing order.

  

-  **uniq** : will filter out the repeated lines in a file.
 ```tr ' ' '\12' < odessy.txt | sort | uniq``` will filter the repeated lines from the input passed from ```tr ' ' '\12' < odessy.txt | sort```.

  

-  **-c flag** : is for counting. 
 ```tr ' ' '\12' < odessy.txt | sort | uniq - c``` will count all the repeated words that came from ```tr ' ' '\12' < odessy.txt | sort | uniq```.

  

-  **-n flag** : is used with sort and is used to compare according to string numerical value.

  

-  **-r flag** :  is also used with sort and is used to denote sorting in reverse order. i.e. if the sort is done in ascending order, using -r will do the sorting in decending order.

  

-  **Redirect Standard Output (>)** : is used to write/ redirect output to a new file. For example, ```tr ' ' '\12' < odessy.txt | sort | uniq -c | sort -nr > report.txt``` will redirect the output to a new file called report.txt.

  

---
### Suggestion
- In both Git Bash and Powershell, use up and down arrow to navigate through previously written comands and use left and right arrow to navigate through the words in the line.
- Use right click then click pate to paste anything from your clip board in Git Bash.(short cuts dosen't work)