# Python_Project

Q1: You are working in a bank, and you have been given two lists of the
employees who worked in 2021. Employees' names in list 1 are Ramesh, Suresh,
Mahesh, Ali, Jacob, and Saritha. List 2 contains the names of Ali, Mukesh,
Mahesh, Jacob, Sai, and Sarita. Please write a program that helps to identify
people who are common in both lists. Please do not use any in-built function.
```python
list1=['Ramesh', 'Suresh', 'Mahesh', 'Ali','Jacob']
list2=['Ali', 'Mukesh', 'Mahesh', 'Jacob', 'Sai', 'Sarita']
list3=list1 + list2
list4=[]
for x in list3:
    if list3.count(x)>1 and x not in list4:
      list4.append(x)

print(list4)
```
Output
```python
['Mahesh', 'Ali', 'Jacob']
```
Q2: While entering data, someone entered a few names as a common string
"Ramesh Suresh Mohit". Please write a program which separates all the names
and converts them into a list. Once converted into a list, please write a program
that adds their age.
Ramesh: 25
Suresh: 22
Mohit: 26
```python
names = "Ramesh Suresh Mohit"
names_new = names.split()
age1=0
ages = [25, 22, 26]
result = list(zip(names_new, ages))
for x in ages:
    age1=age1+x
print('Total age: '+ str(age1))
print(result)
```
Output
```python
Total age: 73
[('Ramesh', 25), ('Suresh', 22), ('Mohit', 26)]
```
Q3: You are working in a medical store. A patient came to your medical store
and asked to buy 2 strips of paracetamol, 3 strips of azithromycin, and 5 strips
of Vitamin C. One strip of paracetamol costs Rs 35, one strip of azithromycin
costs Rs 49, and one strip of vitamin c costs Rs. 33. Patient gave you Rs 2000.
Please tell us what is the total cost of each medicine, the total cost of all
medicine, and how much money you refunded to the patient.
```python
Paracetamol=35
Azithromycin=49
Vitamin_C=33
Paracetamol_strips=int(input("Enter Number of Paracetamol_strips: "))
Azithromycin_strips=int(input("Enter Number of Azithromycin_strips: "))
Vitamin_C_strips=int(input("Enter Number of Vitamin_C_strips: "))
Received=int(input("enter the amount given: "))
p= "Total amount for paracetamol: {}, Total amount for Azithromycin: {}, Total amount for Vitamin_C: {} "
print(p.format(Paracetamol*Paracetamol_strips, Azithromycin*Azithromycin_strips,Vitamin_C*Vitamin_C_strips))
total=((Paracetamol*Paracetamol_strips)+(Azithromycin*Azithromycin_strips)+(Vitamin_C*Vitamin_C_strips))
z='Total amount: {}'
print(z.format(total))
Return_amount=int((Received-total))
b="Return amount {}"
print(b.format(Return_amount))
```
Output
```python
Enter Number of Paracetamol_strips: 1
Enter Number of Azithromycin_strips: 1
Enter Number of Vitamin_C_strips: 1
enter the amount given: 1000
Total amount for paracetamol: 35, Total amount for Azithromycin: 49, Total amount for Vitamin_C: 33 
Total amount: 117
Return amount 883
```

Q4: Accept a sentence as input and find the number of vowels in it. Assume
that the sentence has no punctuation marks. For example, I am learning python
contains 6 vowels. This function should be applicable for all other different
sentences.

```python
sentence = input("Enter a sentence: ")
vowels = ['a', 'e', 'i', 'o', 'u']

count = len([char for char in sentence.lower() if char in vowels])

print("The number of vowels in the sentence is:", count)
```
Output
```python
Enter a sentence: aeiou
The number of vowels in the sentence is: 5
```
Q5: You have been appointed by the election commission to create a website.
Your first task is to work on a program which tells candidates if they are eligible
for voting or not. If they are eligible, your output should be 'Congrats! You are
eligible'; otherwise, it should tell that you have to return after X number of
years. The eligibility criteria for voting is 18 years.
For example, If someone is 18 or above, your output should be 'Congrats! You
are eligible'. If someone's age is 15 years, it should print output as 'return after :3
years'.

```python
age=int(input("Enter your age: "))
small= 18-age
b="return afer {} years"
if age>18:
  print('Congrats! You are eligible')
else:
    print(b.format(small))
```
Output
```python
Enter your age: 12
return afer 6 years
```

Q6: Given a list of integers, find the cumulative sum of the elements of the list
and store them in another list.
A = [1, 2, 3, 4, 5]
Output:
[1, 3, 6, 10, 15]
```python
a=[1,2,3,4,5]
y=[]
sum=0
for x in a:
    sum=sum+x
    y.append(sum)
     
print(y)
```
Output
```python
[1, 3, 6, 10, 15]
```



