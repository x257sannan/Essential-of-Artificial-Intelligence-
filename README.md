# Essential-of-Artificial-Intelligence-

## 📂 Lab 1 Code

### task1_table.py
```python
# Task 1: Multiplication table of a number
num = int(input("Enter a number: "))
for i in range(1, 11):
    print(f"{num} x {i} = {num * i}")
```

### task2_prime.py
```python
# Task 2: Check if a number is prime
num = int(input("Enter a number: "))
if num > 1:
    for i in range(2, num):
        if num % i == 0:
            print(f"{num} is not a prime number")
            break
    else:
        print(f"{num} is a prime number")
else:
    print(f"{num} is not a prime number")
```

### task3_loops.py
```python
# Task 3: Print numbers 1 to 10 using while loop
i = 1
while i <= 10:
    print(i)
    i += 1

# Modified: Print even numbers between 1 and 20
i = 2
while i <= 20:
    print(i)
    i += 2
```

### task4_harshad.py
```python
# Task 4: Check if a number is a Harshad Number
num = int(input("Enter a number: "))
digit_sum = sum(int(digit) for digit in str(num))

if num % digit_sum == 0:
    print(f"{num} is a Harshad Number")
else:
    print(f"{num} is not a Harshad Number")
```

---

## 📂 Lab 2 Code

### task1_string_check.py
```python
# Task 1: Count strings with same first and last character
strings = ['abc', 'xyz', 'aba', '1221', 'xyzzyx', 'aa', '122']
count = 0
for s in strings:
    if len(s) >= 2 and s[0] == s[-1]:
        count += 1
print("Result:", count)
```

### task2_tuple_math.py
```python
# Task 2: Sum and product of tuple elements
t = (1, 2, 4, 2, 6)
sum_t = sum(t)
product_t = 1
for num in t:
    product_t *= num
print("Sum:", sum_t)
print("Product:", product_t)
```

### task3_largest_list.py
```python
# Task 3: Largest number in a list
lst = [1, 2, 4, 2, 6]
print("Largest number:", max(lst))
```

### task4_remove_empty_tuple.py
```python
# Task 4: Remove empty tuples from list
L = [(), (), ('',), ('a', 'b'), (), ('a', 'b', 'c'), (), ('d')]
result = [t for t in L if t]
print("Result:", result)
```

### task5_square_dict.py
```python
# Task 5: Generate dictionary of squares
n = int(input("Enter a number: "))
square_dict = {str(x): x * x for x in range(1, n + 1)}
print(square_dict)
```

### task6_number_to_words.py
```python
# Task 6: Convert number to words
num = input("Enter a number: ")
digits_map = {
    '0': 'Zero', '1': 'One', '2': 'Two', '3': 'Three', '4': 'Four',
    '5': 'Five', '6': 'Six', '7': 'Seven', '8': 'Eight', '9': 'Nine'
}
output = " ".join(digits_map[d] for d in num if d in digits_map)
print(output)
