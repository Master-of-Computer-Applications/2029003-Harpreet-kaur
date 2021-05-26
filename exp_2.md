__Write a Python program to reverse the order of the items in the array__.

_Code_
```python
arr=[1,2,3,4,5]

result=list(reversed(arr))
print"Reversed array using reversed() method : ",result


res=arr[::-1]
print"Reversed array using list slicing is : ",res


arr.reverse()
print"Reversed array using reverse() method : ",arr
```

*Output*

![reverse of array list](https://user-images.githubusercontent.com/79329465/119646070-5f3bc580-be3c-11eb-8c83-6fa4506607d0.png)


