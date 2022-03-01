# Intro to Programming - Python

## Introduction Python Pickling, Python Exception Handling & Git Hub Pages 
In this assignment I will explain the steps I used to create several scripts to show the use of pickling, exception handling and git hub pages. I did research pickling first to better understand how this is used and for what purpose. 

I started with a site from [Univeristy of Pittsburgh](https://sites.pitt.edu/~naraehan/python3/pickling.html)
I felt that site gave some very simplified examples, which helped greatly in my understanding of the process and broke it out in an easy way to understand. 

For the error handling I used this URL from [Python Basicis](https://pythonbasics.org/try-except/). I felt again that this presented the basic information in an easy-to-understand presentation. 

## Variables
For the first script, pickling, I created a basic script with variables named globally for the file name, objFile and a dictionary. These would enable me to do a very basic script to show how pickling works. 

For the error handling, try/except, again, I really wanted a basic example of how the code worked. For variables I used integers and wanted to determine if the integers that an end user would enter would in fact be integers. 

## Starting the Code 
I decided to break up the assignment into two different scripts in order to make it more understandable for myself. I have to admit, in starting the pickling script, WK7_P.Everett_Pickling.py, I found it very straight forward in writing the code and it actually worked. I was quite surprised as it did not throw any error messages on the first try. 

I then went on to research the try/except error handling in Python. I do have to say I found one issue, which was in regards to using int in front of the variables for numbers. At one point I did enter a string for one of them and it actually added the first number plus the string. Definitely not what I really wanted. Once I resolved that, it was good to go. 

## Script
Once I was able to get both scripts working correctly, I added comments to the lines in order for it to be easier to read. I placed both scripts within my Git Hub account [here](https://github.com/pme636/ITFnd100-Mod07). 


## Pickling
```
# ------------------------------------------------- #
# Title: Pickling - example
# Description: An example of pickling in Python
# ChangeLog: (Who, When, What)
# P.Everett 02/21/2022,Created Script
# ------------------------------------------------- #

# Data -------------------------------------------- #
strFile = "MyScores.dat"  #file needs to be a binary file
objFile = None
myDict = {} #empty dictionary object
dicScores = {'Ralph': 89, "Lisa": 99, "Jack": 56}  #score dictionary

# Processing -------------------------------------- #
import pickle
objFile = open(strFile, 'ab') #file is to be opened with a binary append vs regular append
pickle.dump(dicScores, objFile) # dumps the dictonary data into the non text file
objFile.close()


# Presentation ------------------------------------ #
objFile =open(strFile, 'rb') #open the file, again in binary mode for read only
myDict = pickle.load(objFile)  #loads the data from the binary file into the variable dictionary
print(myDict) #prints the data from the file so the end user can see the data
```

## Error Handling - Try/Except
```
# ------------------------------------------------- #
# Title: Try Except Error Handling - example
# Description: An example of error handling in Python
# ChangeLog: (Who, When, What)
# P.Everett 02/22/2022,Created Script
# ------------------------------------------------- #

try:
   intV1 = input("Enter a value to add: ") #asks user to enter a number to add
   intV2 = input("Enter a second value to add: ") #asks user to enter a second number to perform addition
   intAnswer = int(intV1) + int(intV2) #adds the two values if they are integers
   print(intAnswer)

except:
    print("Please be sure to enter a number value! <<< Custom Message\n")#Error message if one of the values is not a number

```
## Screen Prints of Results

![Pickling](/github.com/pme636/ITFnd100-Mod07/tree/main/docs/assets/PythonPickling.png)




## Script Saved
The script was saved in the week 7 folder along with several screen shots. I placed those into a folder I saved on git hub. 

## Git Hub Pages
I read thru the provided information for creating the git hub pages and was able to finally create my page with the data from this document. I included the links of the pages I used as a reference and saved the screen prints into a separate folder. It seems to be working also!



Summary
Using the provided information from this week’s assignment I was able to create one script to show the example of pickling in Python. In addition, I was also able to create a script for try/except error handling in Python. They do actually work too! 

