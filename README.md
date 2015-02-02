# Hadoop-Projects

This is a simple Hadoop Word Count program, which illustrates Hadoop MapReduce programming model.
Input is a text file. And output is a file containing the number of occurences of each word in the file.
Mapper takes each line from the file as its input and then using String Tokenizer, the input line is split into words and fed to the Combiner.
The combiner then performs aggregation of data and gives the count of each word. 
This output is given to the Reducer which collects data from all combiner instances on nodes of the cluster and gives the output in the desired form.
