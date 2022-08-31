# Python-Challenge
# DAY-3 TEN CODING SOLUTIONS

#### 1. PRINTING SIMPLE NUMBER TRIANGLE PATTERN

n = int(input("Enter number of rows: "))
for i in range(n):
    for j in range(i+1):
        print(i+1,end = " ")
    print()

#### 2. PRINTING SIMPLE INVERTED NUMBER TRIANGLE

n = int(input("Enter number of rows: "))
for i in range(n):
    for j in range(i,n+1):
        print(i+1,end = " ")
    print()

#### 3.PRINTING INVERTED HALF PYRAMID PATTERN WITH NUMBERS:

rows = int(input("enter number of rows: "))
for i in range(rows, 0, -1):
    for j in range(0, i+1):
        print(j, end=' ')
    print("")


#### 4. PRINTING REVERSE PYRAMID PATTERN WITH NUMBERS

n = int(input("Enter number of rows: "))
for i in range(1,n):
    for j in range(i ,0 , -1):
        print(j,end = " ")
    print()

#### 5. PASCALS TRIANGLE USING NUMBERS

from math import factorial
n = int(input("Enter number of rows: "))
for i in range(n):
    for j in range(n-i-1):#6-0-1=5
        print(end=" ")#left spacing 
    for j in range(i+1):#at i=0 i.e,0 row we want 1 number
        print(factorial(i)//(factorial(j)*factorial(i-j)), end=" ")#nCr = n!/((n-r)!*r!)
    print()
         
        
          #0C0
       #1C0   #1C1
    #2C0   #2C1   #2C2
#3C0   #3C1   #3C2    #3C3

from math import factorial
n = int(input("Enter number of rows: "))
for i in range(n):
    for j in range(i+1):#at i=0 i.e,0 row we want 1 number
        print(factorial(i)//(factorial(j)*factorial(i-j)), end=" ")#nCr = n!/((n-r)!*r!)
    print()

#### 6.EQUILATERAL TRIANGLE OF STARS PATTERN

n = int(input("Enter number of rows: "))
for i in range(n):
    for j in range(n-i-1):
        print(end=" ")
    for j in range(i+1):
        print('*',end = " ")
    print()

#### 7. INVERTED PYRAMID PATTERN OF STARS 

n = int(input("Enter number of rows: "))
for i in range(n-1,-1,-1): #6,5,4,3,2,1,0
    for j in range(n-i-1-1,-1,-1):
        print(end=" ")
    for j in range(0,i+1):
        print("* ",end="")
    print()

#### 8.DIAMOND SHAPED PATTERN OF STARS

n=int(input("Enter number of rows:")) 
for i in range(0,n): 
    for j in range(0,n-i-1):#left spacing
        print(end=" ")
    for j in range(0,i+1):
        print("* ",end="")# *_ indicates *is preceded by a whitespace
    print()

for i in range(n-1,-1,-1): #6,5,4,3,2,1,0
    for j in range(n-i-1-1,-1,-1):
        print(end=" ")
    for j in range(0,i+1):
        print("* ",end="")
    print()

#### 9. PRINT PYTHON WORD AS PYRAMID PATTERN

str="python"
x=""
for i in str:
    x=x+i
    print(x)

####  10. PRINT SQUARE AND HOLLOW SQUARE PATTERNS USING STARS

#SQUARE PATTERN
n = int(input("enter number of rows and columns to be printed : "))
for i in range(n):#i reps no of rows
    for j in range(n):#no of columns
        print("* ",end="")
    print()

n=int(input("Enter number of rows: "))
for i in range(1,n+1):
    for j in range(1,n+1):
        if i==1 or i==n or j==1 or j==n:
            print("*",end="")
        else:
            print(" ",end="")
    print()

DONE FOR THE DAY!
