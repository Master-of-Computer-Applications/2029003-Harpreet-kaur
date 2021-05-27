## *Python program to create an array of 5 elements and Display the array items.  Access each individual element through indexes.*

First of all in first line we define the values [10,20,30,40,50] to the array varible 'a'. Then we display them using the "print" command.
  To access each elemnet individully we display each element through indexes individually by print command again.


..*CODE*
```python
a=[10,20,30,40,50]
```
```python
print a
print"1st element:",a[0]
print"2nd element:",a[1]
print"3rd element:",a[2]
print"4th element:",a[3]
print"5th element:",a[4]
````

..*OUTPUT*

![Screenshot from 2021-04-27 23-28-05](https://user-images.githubusercontent.com/79329465/116290342-fddaf500-a7b0-11eb-8e2e-d381d076fad4.png)



## *Write a Python program to reverse the order of the items in the array*.

_Code_
```python
arr=[1,2,3,4,5]
```
```python
result=list(reversed(arr))
print"Reversed array using reversed() method : ",result
```
```python
res=arr[::-1]
print"Reversed array using list slicing is : ",res
```
```python
arr.reverse()
print"Reversed array using reverse() method : ",arr
```

*Output*

![reverse of array list](https://user-images.githubusercontent.com/79329465/119646070-5f3bc580-be3c-11eb-8c83-6fa4506607d0.png)



## *Write a Python program to append a new item to the end of the array.*

_code_
```python
A=['mango','orange','banana']
```
```python
B=['pear','grapes','apple']
```
```python
A.append(B)
print A
```

_Output_

![append item into the array](https://user-images.githubusercontent.com/79329465/119653321-d2e1d080-be44-11eb-8bea-8362881a3556.png)



## *Write a Python program to remove a specified item using the index from an array.*

_Code_
```python
A=[1,2,3,4]
```
```python
A.pop(1)
print" remove a specified item using the index from an array by POP operation: ",A
```
_Output_

![remove item from array list](https://user-images.githubusercontent.com/79329465/119653922-834fd480-be45-11eb-8890-379e31fdd749.png)


## *Write a Python program to get the length of an array.*

_Code_
```python
A=[1,2,3,4,'hello']
```
```python
print"Display all elements: ",A
print"Length of all elements: ",len(A)
```

_Output_

![length of array ](https://user-images.githubusercontent.com/79329465/119654962-a2029b00-be46-11eb-9afc-63f57d606a04.png)
