# Linux-server
<h3>linux basic command </h3>
<pre>
clear - clean the command line
ctrl+C (^C) -to get out of process

pwd - מראה את כתובת העבודה הנוכחית 
cd - cd Desktop למשל ייכנס לתוך תקייה בנתיב 

date -תאריך
cal - ידפיס את לוח השנה בטרמינל
ncal - ידפיס את לוח השנה בטרמינל בצורה אנכית 
אפשריות נוספות לתאריך : 
ncal 2022 - יצי לי לוח שנה מלא של אותה שנה 
cal july 1969 -חודש יולי באותה שנה 

## commands & arguments
sort :
sort color.txt - יסדר בסדר אלפבתי את התוכן שבקובץ
rm:
rm color.txt - מוחק קובץ
rm -r - מוחק תקייה 
mv - in Linux stands for move, mv <file/folder we want to move> <destination>

ncal -j -  מס היום בשנה (ספירה ג'ליאנית)
ncal -3 - חודש אחורה נוכחי וקדימה 
ניתן לשלב כמה אופציות לאחר פקודה מסויימת כך :  ncal -3 -j שיציג שלושה חודשים עוקבים בצורה גוליאנית 
אפשר גם לשלב אותם ןלכתוב בצורה הבאה :  ncal -3j (combine options)


<h4> long form option</h4> 
1.date -u
2.date --universal

ls- רשימה של כל התיקיות 
ls -la  רשימה של כל הקבצים כולל המוסתרים שמתחילים בנקודה
cd Desktop - get into folder
touch colors.txt -create file 

vi fileName.txt  הכנסת תוכן לקובץ דרך הטרמינל  
will open the empty file after that
in the terminal you press i to start INSERT text to it through terminal
in order to exit insert mood just press esc and than enter ":wq" to save the file changes.(w-write :q- just quit no save)

Command "cp" - allows you to copy a file or a folder (or multiples) from one location to another one example:
cp <file we want to copy> <name of the new file/folder>
cp -r <folder we want to copy> <name of the new file/folder> //use -r option to copy folders


sort colors.txt -r או --revers  יציג לי את תוכן הרשימה מסודר בצורה אלפבתית הפוכה
sort colors.txt -r -u  רשימה מסודרת הפוך שמראה רק ערכים ייחודיים (--unique)
ncal -A2 או -A5 ידפיס לי מס חודשים לאחר חודש נוכחי בהתאם למס שארשום אחרי האות (After) 
ncal -B2 או -A5 ידפיס לי מס חודשים לפני חודש נוכחי בהתאם למס שארשום אחרי האות (Before)
ניתן גם לשלב כך : ncal -B2 -A1 יציג חודשיים לפני וחודש אחרי 
ncal -M -A1 -B1 july 1969  יציג חודש לפני ואחרי יולי בשנת 1969 






</pre>


<h3>   man - Manual מדריך לפקודות  : </h3>
<h4> man commnd will give me descriptions of all the availible options of the command    </h4>
<pre>
man ls יתן לי את כל האופציות בפקודה הזאת 
בדף שייפתח בקומנד ליין 
ננווט כך : 
g - יעלה אותנו הכי למעלה 
G - ייקח אותנו למטה בעמוד 
q - man חזרה לקומנדליין יצא מהעמוד של 
press "space" / f to see manual next page that fit the terminal view
press b to see manual back page that fit the terminal view
h - find all the moving in manual shortcuts 
To search spesifice command opption in the manual (like cntrl + f) use /-theOption

</pre>

<h3>  type/which for command that dont have manual page entries  </h3>
<pre>
man command
type command - tell me if the command is shell/binaty/alias
which command - to see path of the command location
help command
</pre>

<h3> Navigation </h3>
<pre>
xdg-open /  -to open the root directory (like c driver in windows)
/home -contain ahome folderfor each user on the system
xdg-open ~  -to open home directory shortcut
pwd   -Print Working Directory (current path)
ls    -show list of folders and files in the current directory 
ls folderName  -it will show me all the files and folders in spesific folder name 

</pre>
![image](https://user-images.githubusercontent.com/86184072/193459753-5cd7b92f-7471-415a-9dc1-4b03fb7f3cef.png)


<pre></pre>
<!-- https://poalim.udemy.com/course/the-linux-command-line-bootcamp/learn/lecture/26177178#overview -->


<h3> Permissions </h3>
<pre>
ls -la   -la flag allows us to see some basic data related to the files or folders, like the permissions of the files/folders, their creation date/time, etc

read: The Read permission refers to a user's ability to read the contents of the file. It is stated with the character r.
write: The Write permission refers to a user's ability to write or modify a file or directory. It is stated with the character w.
execute: The Execute permission affects a user's ability to execute a file or view the contents of a directory. It is stated with the character x.

user-based permission groups:

owner: The Owner permissions apply only to the owner of the file or directory, and will not impact the actions of other users. They are represented in the first 3 characters.
group: The Group permissions apply only to the group that has been assigned to the file or directory, and will not affect the actions of other users. They are represented in the middle 3 characters.
all users: The All Users permissions apply to all other users on the system, and this is the permission group that you want to watch the most. They are represented in the last 3 characters.

So, applying all this to our file, we can say that the owner of the file (in this case, it's us) has read (r) and write (w) permissions, and the group and the rest of users have only read (r) permissions.
example:
rw-/r--/r--


</pre>
