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

ncal -j -  מס היום בשנה (ספירה ג'ליאנית)
ncal -3 - חודש אחורה נוכחי וקדימה 
ניתן לשלב כמה אופציות לאחר פקודה מסויימת כך :  ncal -3 -j שיציג שלושה חודשים עוקבים בצורה גוליאנית 
אפשר גם לשלב אותם ןלכתוב בצורה הבאה :  ncal -3j (combine options)


<h4> long form option</h4> 
1.date -u
2.date --universal

ls- רשימה של כל התיקיות 
cd Desktop - get into folder
touch colors.txt -create file 

sort colors.txt -r או --revers  יציג לי את תוכן הרשימה מסודר בצורה אלפבתית הפוכה
sort colors.txt -r -u  רשימה מסודרת הפוך שמראה רק ערכים ייחודיים (--unique)
ncal -A2 או -A5 ידפיס לי מס חודשים לאחר חודש נוכחי בהתאם למס שארשום אחרי האות (After) 
ncal -B2 או -A5 ידפיס לי מס חודשים לפני חודש נוכחי בהתאם למס שארשום אחרי האות (Before)
ניתן גם לשלב כך : ncal -B2 -A1 יציג חודשיים לפני וחודש אחרי 
ncal -M -A1 -B1 july 1969  יציג חודש לפני ואחרי יולי בשנת 1969 






</pre>


<h3>   man - Manual מדריך לפקודות  : </h3>
<pre>
man ls יתן לי את כל האופציות בפקודה הזאת 
בדף שייפתח בקומנד ליין 
ננווט כך : 
g - יעלה אותנו הכי למעלה 
G - ייקח אותנו למטה בעמוד 
q - man חזרה לקומנדליין יצא מהעמוד של 

</pre>

<!-- https://poalim.udemy.com/course/the-linux-command-line-bootcamp/learn/lecture/26177178#overview -->
