# command-line-arguments-to-count-word
## AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.
## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7
## ALGORITHM: 
### Step 1:
import sys module to use the command line arguments 
### Step 2: 
Use the open() function to get the file name from the command line arguments.

sys.argv[1] refers to the first command line argument (file name).
### Step 3: 
Iterate through the content of the file using a for loop.
### Step 4:  
Split the contents into each line using .split() function.
### Step 5: 
Iterate the list of lines and increment the value of variable (word) each time.

### Step 6: 
Run the program to determine the number of words in the file created.

## PROGRAM:
```python
'''Program for getting the word count from the contents of a file using command line arguments
Developed by: Santhan Kumar
Reference number: 23004568
''''
import sys
count = {}
total_count = 0
with open(sys.argv[1], 'r') as f:
    for line in f:
        for word in line.split():
            if word not in count:
                count[word] = 1
            else:
                count[word] += 1
            total_count += 1
print(count)
print(f"\nTotal word count: {total_count}")

```
### OUTPUT:
![Screenshot 2023-12-27 173957](https://github.com/AkilaMohan/command-line-arguments-to-count-word/assets/145742508/c8972b5d-4341-4712-8632-9fee002a1acc)

## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.
