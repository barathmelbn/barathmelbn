1.
# Program to print prime numbers in the given range
n = int(input("Enter the value of n: "))
for i in range(2, n + 1):
    is_prime = True
    for j in range(2, i):          if i % j == 0:
            is_prime = False
            break
    if is_prime:
        print(i, end=' ')
2. while loop
i, j = 1, 3
n = int(input("Enter the value of n: "))
print("The generated series is:")
print(i, j, end=' ')
n
while j < n:
    k = j + 2 * (j - i)
print(k, end=' ')
    i, j = j, k
Nested while loop
n = int(input('Enter the value of n: '))
c1 = 1  
while c1 <= n:
    f = 1  
    c2 = 1  
    while c2 <= c1:
        f *= c2  
        c2 += 1  
    print("Factorial of", c1, "is", f)
    c1 += 1
for loop
for i in range(5):
    print("Python is interpreted object-oriented high level programming language")
print("The program executed successfully")

 Nested for loop
for i in range(1, 4):
    for j in range(1, 11):
        print(i, '*', j, '=', i * j)
 
3. Write a python program to print Armstrong numbers between the given range
for num in range(100, 2001):
 sum_of_powers = 0
 temp = num
 order = len(str(num)) 
while temp > 0:
 digit = temp % 10
 sum_of_powers += digit ** order
 temp //= 10
if num == sum_of_powers:
 print(num)

4. Python program to find minimum and maximum of a given range of numbers
data = [-2, 45, 0, 11, -9, 88, -97, -202, 747]
for i in range(len(data)):
    min_value = min(data[i:]); data[data.index(min_value)], data[i] = data[i], min_value
print('Sorted numbers:', data)

5. Fibonacci Series Program:
def recursive_fibonacci(n):
 if n <= 1:
 return n
 else:
 return recursive_fibonacci(n - 1) + recursive_fibonacci(n - 2)
n_terms = 10
if n_terms <= 0:
 print("Invalid input! Please input a positive value.")
else:
 print("Fibonacci series:")
 for i in range(n_terms):
 print(recursive_fibonacci(i))


6. 4. Leap Year Checker Program:
year = int(input("Enter a year: "))
if (year % 400 == 0) or (year % 4 == 0 and year % 100 != 0):
 print(year, "is a leap year")
else:
 print(year, "is not a leap year")


7. Python Program to sort a set of elements using Selection sort
def selectionSort(arr):
    for i in range(len(arr)):
        min_index = i
        for j in range(i + 1, len(arr)):
            if arr[j] < arr[min_index]:
                min_index = j
        arr[i], arr[min_index] = arr[min_index], arr[i]  
arr = [-2, 45, 0, 11, -9, 88, -97, -202, 747]
selectionSort(arr)  # Call the sorting function
print('Sorted array:', arr)

8. Matrix Multiplication Program:
# Program to multiply two matrices using nested loops
# 3x3 matrix
X = [[12,7,3],
    [4 ,5,6],
    [7 ,8,9]]
# 3x4 matrix
Y = [[5,8,1,2],
    [6,7,3,0],
    [4,5,9,1]]
# result is 3x4
result = [[0,0,0,0],
         [0,0,0,0],
         [0,0,0,0]]
# iterate through rows of X
for i in range(len(X)):
   # iterate through columns of Y
   for j in range(len(Y[0])):
       # iterate through rows of Y
       for k in range(len(Y)):
           result[i][j] += X[i][k] * Y[k][j]
for r in result:
   print(r)
9. string to iterate
string_to_iterate = "Python Data Science"
for char in string_to_iterate:
    print(char)  # Print each character on a new line
