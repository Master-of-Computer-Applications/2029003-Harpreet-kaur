|  Sr no |  Experiment Name |  Remarks|   
|---|---|---|
|  1| Write a Python program to create an array of 5 elements and display the array items Access each individual items through indexes.  |   |   
|  2|Write a Python program to reverse the order of items in the array.   |   |   
|  3|Write a Python program to append a new item to the end of the array.  |   |   
|  4|Write a Python program to remove a specified item using the index from an array.  |  |
|  5|Write a Python program to get the length of an array.  |  |
|  6|Write a Python program for binary Search.   |  |
|  7|Write a Python program for sequential or linear search.   |  |
|  8|Write a Python program to sort a list of elements using the bubble sort algorithm.   |  |
|  9|Write a Python program to sort a list of elements using the selection sort algorithm.   |  |
|  10|Write a Python program to sort a list of elements using the insertion sort algorithm.   |  |
|  11|Write a Python program to sort a list of elements using the quick sort algorithm.   |  |
|  12|Write a Python program to create a singly linked list and append some items iterate through the list.   |  |
|  13|Write a Python program to find the size of singly linked list.   |  |
|  14|Write a python program to search a specific item in singly linked list and return true if the item was found otherwise return false.   |  |
|  15|Write a Python program to delete the first item from singly linked list.   |  |
|  16|Write a Python program to create a circular linked list.   |  |
|  17|Write a Python program to implement stack operation using list.   |  |
|  18|Write a Python program to implement queue and its operations using list.   |  |
|  19|Write a Python program to find kth smallest element in a given binary tree.   |  |
|  20|Write a Python program to count the number of nodes in binary search tree.   |  |



## 1._Write a Python program to create an array of 5 elements and display the array items Access each individual items through indexe._

_Code_

```python
a=[10,20,30,40,50]
print a
print"1st element:",a[0]
print"2nd element:",a[1]
print"3rd element:",a[2]
print"4th element:",a[3]
print"5th element:",a[4]
```
_Output_
![Screenshot from 2021-06-07 13-18-08](https://user-images.githubusercontent.com/79329465/120979093-d9504080-c792-11eb-893b-dc8990909e1d.png)


## 2._Write a Python program to reverse the order of the items in the array._

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
_Output_

![Screenshot from 2021-06-07 13-34-50](https://user-images.githubusercontent.com/79329465/120981324-32b96f00-c795-11eb-8782-8902af86619c.png)


## 3._Write a Python program for sequential or linear search._

_Code_

```python


## _Write a Python program to append a new item to the end of the array._

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

![Screenshot from 2021-06-07 13-49-14](https://user-images.githubusercontent.com/79329465/120983432-51206a00-c797-11eb-8afe-c3dd187cd77d.png)


## 4._Write a Python program to remove a specified item using the index from an array_

_code_

```python
A=[1,2,3,4]
```
```python
A.pop(1)
print" remove a specified item using the index from an array by POP operation: ",A
```
_Output_

![Screenshot from 2021-06-07 13-53-15](https://user-images.githubusercontent.com/79329465/120984769-942f0d00-c798-11eb-9dc8-75b13f33c804.png)


## 5._Write a Python program to get the length of an array._

_Code_

```python
A=[1,2,3,4,'hello']
```
```python
print"Display all elements: ",A
print"Length of all elements: ",len(A)
```
_Output_

![Screenshot from 2021-06-07 14-09-10](https://user-images.githubusercontent.com/79329465/120986461-3f8c9180-c79a-11eb-9db4-7788d3acbcde.png)


## 6._Write a Python program for binary search._
_Code_

```python
def binarySearch (arr, l, r, x):

    if r >= l:
 
        mid = l + (r - l) // 2
 
       
        if arr[mid] == x:
            return mid
         
       
        elif arr[mid] > x:
            return binarySearch(arr, l, mid-1, x)
        else:
            return binarySearch(arr, mid + 1, r, x)
 
    else:
        return -1
        
arr = [ 2, 3, 4, 10, 40 ]
x = 10

result = binarySearch(arr, 0, len(arr)-1, x)
 
if result != -1:
    print ("Element is present at index % d" % result)
else:
    print ("Element is not present in array")
```

_Output_

![Screenshot from 2021-06-07 14-14-03](https://user-images.githubusercontent.com/79329465/120987398-2d5f2300-c79b-11eb-9c2e-88d033a1c1b8.png)


## 7._Write a Python program for sequential or linear search._

_Code_

```python
def linearsearch(arr, x):
   for i in range(len(arr)):
      if arr[i] == x:
         return i
   return -1
arr = ['t','u','t','o','r','i','a','l']
x = 'a'
print("element found at index "+str(linearsearch(arr,x)))
```

_Output_

![Screenshot from 2021-06-07 14-25-44](https://user-images.githubusercontent.com/79329465/120988543-4caa8000-c79c-11eb-89dd-528ae8b4c51e.png)


## 8_Write a Python program to sort a list of elements using the bubble sort algorithm._

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

_Output_

![Screenshot from 2021-06-07 14-36-57](https://user-images.githubusercontent.com/79329465/120990176-e6bef800-c79d-11eb-880b-5317c13114ca.png)


## 9._Write a Python program to sort a list of elements using the selection sort algorithm._

_Code_

```python
def selectionSort(array):
  n = len(array)
  for i in range(n):
    
    minimum = i

    for j in range(i+1, n):
      if (array[j] < array[minimum]):
        
        minimum = j
    
    temp = array[i]
    array[i] = array[minimum]
    array[minimum] = temp
    
  return array
  
array = [13, 4, 9, 5, 3, 16, 12]
print(selectionSort(array))
```

_Output_

![Screenshot from 2021-06-07 14-52-39](https://user-images.githubusercontent.com/79329465/120992309-1a9b1d00-c7a0-11eb-9a32-27ac80ceeb17.png)


## 10._Write a Python program to sort a list of elements using the insertion sort algorithm._

_Code_

```python
def insertionSort(arr):

     for i in range(1, len(arr)):

		key = arr[i]

		j = i-1
		while j >=0 and key < arr[j] :
				arr[j+1] = arr[j]
				j -= 1
		arr[j+1] = key


arr = [12, 11, 13, 5, 6]
insertionSort(arr)
print ("Sorted array is:")
for i in range(len(arr)):
	print ("%d" %arr[i])
```

_Output_

![Screenshot from 2021-06-07 15-01-25](https://user-images.githubusercontent.com/79329465/120993833-8c279b00-c7a1-11eb-8acb-18e45d6adf44.png)


## 11._Write a Python program to sort a list of elements using the quick sort algorithm._

_code_

```python
def partition(arr, low, high):
    i = (low-1)         
    pivot = arr[high]     
  
    for j in range(low, high):
  
        if arr[j] <= pivot:
  
            i = i+1
            arr[i], arr[j] = arr[j], arr[i]
  
    arr[i+1], arr[high] = arr[high], arr[i+1]
    return (i+1)
  
def quickSort(arr, low, high):
    if len(arr) == 1:
        return arr
    if low < high:

        pi = partition(arr, low, high)

        quickSort(arr, low, pi-1)
        quickSort(arr, pi+1, high)
  
arr = [10, 7, 8, 9, 1, 5]
n = len(arr)
quickSort(arr, 0, n-1)
print("Sorted array is:")
for i in range(n):
    print("%d" % arr[i])
```
_Output_

![Screenshot from 2021-06-07 15-38-26](https://user-images.githubusercontent.com/79329465/120999275-90a28280-c7a6-11eb-8fa6-f03eca54dd0b.png)


## 12._

_Code_

```python
class Node:
    # Singly linked node
    def __init__(self, data=None):
        self.data = data
        self.next = None
class singly_linked_list:
    def __init__(self):
        # Createe an empty list
        self.head = None
        self.tail = None
        self.count = 0
    def iterate_item(self):
        # Iterate the list.
        current_item = self.head
        while current_item:
            val = current_item.data
            current_item = current_item.next
            yield val
    def append_item(self, data):
        #Append items on the list
        node = Node(data)
        if self.tail:
            self.tail.next = node
            self.tail = node
        else:
            self.head = node
            self.tail = node
        self.count += 1
items = singly_linked_list()
items.append_item('PHP')
items.append_item('Python')
items.append_item('C#')
items.append_item('C++')
items.append_item('Java')
for val in items.iterate_item():
    print(val)
print"\nhead.data: ",items.head.data
print"tail.data: ",items.tail.data
```
_Output_

![Screenshot from 2021-06-07 15-54-40](https://user-images.githubusercontent.com/79329465/121001411-e5df9380-c7a8-11eb-9a0d-c8759f3dad49.png)


## 13._Write a Python program to find the size of a singly linked list._

_Code_

```python
class Node:
    # Singly linked node
    def __init__(self, data=None):
        self.data = data
        self.next = None
class singly_linked_list:
    def __init__(self):
        # Createe an empty list
        self.tail = None
        self.head = None
        self.count = 0
	
    def append_item(self, data):
        #Append items on the list
        node = Node(data)
        if self.head:
            self.head.next = node
            self.head = node
        else:
            self.tail = node
            self.head = node
        self.count += 1
    
    def iterate_item(self):
        # Iterate the list.
        current_item = self.tail
        while current_item:
            val = current_item.data
            current_item = current_item.next
            yield val

items = singly_linked_list()
items.append_item('PHP')
items.append_item('Python')
items.append_item('C#')
items.append_item('C++')
items.append_item('Java')

print"Original list:"
for val in items.iterate_item():
    print(val)

print"\nSize of the list:",items.count
```

_Output_

![Screenshot from 2021-06-07 16-06-47](https://user-images.githubusercontent.com/79329465/121002850-6bb00e80-c7aa-11eb-8257-fd4b34f29ac1.png)


## 14._Write a Python program to delete the first item from a singly linked list._

_Code_

```python
class Node:
    # Singly linked node
    def __init__(self, data=None):
        self.data = data
        self.next = None
class singly_linked_list:
    def __init__(self):
        # Createe an empty list
        self.tail = None
        self.head = None
        self.count = 0

    def append_item(self, data):
        #Append items on the list
        node = Node(data)
        if self.head:
            self.head.next = node
            self.head = node
        else:
            self.tail = node
            self.head = node
        self.count += 1
    
    def delete_item(self, data):
        # Delete an item from the list
        current = self.tail
        prev = self.tail
        while current:
            if current.data == data:
                if current == self.tail:
                    self.tail = current.next
                else:
                    prev.next = current.next
                self.count -= 1
                return
            prev = current
            current = current.next
    def iterate_item(self):
        # Iterate the list.
        current_item = self.tail
        while current_item:
            val = current_item.data
            current_item = current_item.next
            yield val

items = singly_linked_list()
items.append_item('PHP')
items.append_item('Python')
items.append_item('C#')
items.append_item('C++')
items.append_item('Java')

print("Original list:")
for val in items.iterate_item():
    print(val)

print("\nAfter removing the first item from the list:")
items.delete_item('PHP')
for val in items.iterate_item():
    print(val)
```

_Output_

![Screenshot from 2021-06-07 16-21-44](https://user-images.githubusercontent.com/79329465/121004658-93a07180-c7ac-11eb-86de-4113fa986f93.png)


## 15._Write a Python program to create circular single linked lists._

_Code_

```python
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
class CircularLinkedList:
    def __init__(self):
        self.head = None
    def push(self, data):
        ptr1 = Node(data)
        temp = self.head
        ptr1.next = self.head
        if self.head is not None:
            while(temp.next != self.head):
                temp = temp.next
            temp.next = ptr1 
        else:
            ptr1.next = ptr1 # For the first node
        self.head = ptr1
    def printList(self):
        temp = self.head
        if self.head is not None:
            while(True):
                print "%d" %(temp.data),
                temp = temp.next
                if (temp == self.head):
                    break
cllist = CircularLinkedList()
cllist.push(12)
cllist.push(56)
cllist.push(2)
cllist.push(11)
 
print "Contents of circular Linked List"
cllist.printList()
```
_Output_

![Screenshot from 2021-06-07 17-47-18](https://user-images.githubusercontent.com/79329465/121015345-85f0e900-c7b8-11eb-8dee-60c1d5c8ce42.png)


## 16._Write Python programs to implement stack and its operations using list._

_Code_

```python
stack = []
 
# append() function to push
# element in the stack
stack.append('a')
stack.append('b')
stack.append('c')
 
print "Initial stack"
print(stack)
 
# pop() fucntion to pop
# element from stack in
# LIFO order
print "Elements poped from stack:"
print(stack.pop())
print(stack.pop())
print(stack.pop())
 
print "nStack after elements are poped:"
print stack
```
_Output:_

![output](https://user-images.githubusercontent.com/82715927/120991445-45d13c80-c79f-11eb-87e6-8db467c48642.png)

## *18. Write a Python program to implement queue and its operations using list.*
_Code:_

```python
queue = []
queue.append('a')
queue.append('b')
queue.append('c')
print "Initial queue"
print queue
print "Elements dequeued from queue"
print(queue.pop(0))
print(queue.pop(0))
print(queue.pop(0)) 
print"Queue after removing elements"
print queue
```
_Output_

![Screenshot from 2021-06-07 17-53-53](https://user-images.githubusercontent.com/79329465/121016136-66a68b80-c7b9-11eb-8d59-3e34659fa7b5.png)


## *19. Write a Python program to find kth smallest element in a given binary tree.*
_Code:_

```python
class TreeNode(object):
    def __init__(self, x):
        self.val = x
        self.left = None
        self.right = None

def kth_smallest(root, k):
    stack = []
    while root or stack:
        while root:
            stack.append(root)
            root = root.left
        root = stack.pop()
        k -= 1
        if k == 0:
            break
        root = root.right
    return root.val

root = TreeNode(8)  
root.left = TreeNode(5)  
root.right = TreeNode(14) 
root.left.left = TreeNode(4)  
root.left.right = TreeNode(6) 
root.left.right.left = TreeNode(8)  
root.left.right.right = TreeNode(7)  
root.right.right = TreeNode(24) 
root.right.right.left = TreeNode(22)  

print(kth_smallest(root, 2))
print(kth_smallest(root, 3))
```
_Output_

![Screenshot from 2021-06-07 17-56-51](https://user-images.githubusercontent.com/79329465/121016447-c3a24180-c7b9-11eb-8a77-d011900c9822.png)


## *20. Write a Python program to count the number of nodes in binary search tree.*
_Code:_

```python
class Node:
    def __init__(self ,key):
        self.data = key
        self.left = None
        self.right = None
def getfullCount(root):
    if root is None:
        return 0
    queue = []
    queue.append(root)       
    count = 0 #initialize count for full nodes
    while(len(queue) > 0):
        node = queue.pop(0)
        if node.left is not None and node.right is not None:
            count = count+1
        if node.left is not None:
            queue.append(node.left)
        if node.right is not None:
            queue.append(node.right)     
    return count
root = Node(2)
root.left = Node(7)
root.right = Node(5)
root.left.right = Node(6)
root.left.right.left = Node(1)
root.left.right.right = Node(11)
root.right.right = Node(9)
root.right.right.left = Node(4) 
print "%d" %(getfullCount(root))
```
_Output_

![Screenshot from 2021-06-07 17-59-16](https://user-images.githubusercontent.com/79329465/121016759-272c6f00-c7ba-11eb-89c2-c055f11617e4.png)



