# Java Grep App 

## Introduction 
The purpose for this application is to search all the files in a root directory recursively, then output all the lines that have matched given regex pattern and collect them to a specific file. This project was made to practice java development by using popular tools like IntelliJ IDE and Maven. It also help to gain knowledge of using Java I/O and Java 8 features like Stream API and Lambda Expression.

## Usage 
This app take three arguments:
  - regex pattern: the regex pattern that need to be searched for
  
  - path of root directory: the path to the directory that will be searched recursively
  
  - output file directory: the file that stores all the matched lines 
  
 ### Format of arguments: 
    <regex pattern> <path of root directory> <output file directory>
 ### Example of Usage: 
     .*IllegalArgumentException.* ./grep/src /tmp/javaGrep.out

## Pseudocode
The basic pseudocode show below :
```
matchedLines = []
for file in listFilesRecursively(rootDir)
  for line in readLines(file)
      if containsPattern(line)
        matchedLines.add(line)
writeToFile(matchedLines)
```
Methods in JavaGrep.java interface are implemented by JavaGrepImp.java and JavaGrepLambda.java. Methods and fuctionalities show below :
  - listFiles: Traverse a given directory and return all files
  
  - readLines: Read a file and return all the lines

  - containsPattern: Check if a line contains the regex pattern

  - writeToFiles: Write lines to a file
  
  - getters and setters : Save CLI arguments into private member variables (encapsulation)

## Performance Issues

## Improvement 
 1. 
