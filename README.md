# Phanivardhan spark project

## About Me and the objective of the project
I am phanivardhan Gurram from Hyderabad,India <br>
I completed my undergraduation from mallareddy college in the year 2106<br>
I worked as a .net developer for 1 year<br>

The objective of this project is to find the word count

## dataset
 I choose Maheshbabu wikipedia page.I choose this data set as he is my favourite actor.<br>
 link to the data : https://en.wikipedia.org/wiki/Mahesh_Babu
 
 ## commands used:
 
 val inputFile = sc.textFile("C:/44564/scala_sample/winemag_data.txt")<br>
 This command is used to load the input txt file<br><br>
 
 val counts = inputFile.flatMap(line => line.split(",")).map(word => (word,1)).reduceByKey(_ + _);<br>
 This command is used to count the words<br><br>
 
 
 
counts.saveAsTextFile("c:/tmp/show-spark/output")<br>
This command is used to save the result in a output file<br><br>

## result <br> 

| Word    | Count|
|---------|------|
| a      | 4 |
| and     | 10  |
|  as    | 9   |
| he     | 4  |
| his     | 5  |
| in    | 8  |
| is    | 5  |
| mahesh     | 7  |
| of    | 9   |
| telugu      | 6  |
| the | 13   |

Through the above table we conclude that the word "the " has highest count in the input data.

## screenshot of  result graph


 
 
 
