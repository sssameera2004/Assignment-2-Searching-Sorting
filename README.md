QUESTION 4:-

# Insertion sort in Python


def insertionSort(array):

    for step in range(1, len(array)):
        key = array[step]
        j = step - 1
        
        # Compare key with each element on the left of it until an element smaller than it is found
        # For descending order, change key<array[j] to key>array[j].        
        while j >= 0 and key < array[j]:
            array[j + 1] = array[j]
            j = j - 1
        
        # Place key at after the element just smaller than it.
        array[j + 1] = key


data = [9, 5, 1, 4, 3]
insertionSort(data)
print('Sorted Array in Ascending Order:')
print(data)



def insertionSort(a): # Function to implement insertion sort  
    for i in range(1, len(a)):  
        temp = a[i]  
  
        # Move the elements greater than temp to one position   
        #ahead from their current position  
        j = i-1  
        while j >= 0 and temp < a[j] :  
                a[j + 1] = a[j]  
                j = j-1  
        a[j + 1] = temp  
  
def printArr(a): # function to print the array  
  
    for i in range(len(a)):  
        print (a[i], end = " ")  
  
a = [70, 15, 2, 51, 60]  
print("Before sorting array elements are - ")  
printArr(a)  
insertionSort(a)  
print("\nAfter sorting array elements are - ")  
printArr(a)  

METHOD 2:-
# creating a function for insertion  
def insertion_sort(list1):  
  
        # Outer loop to traverse through 1 to len(list1)  
        for i in range(1, len(list1)):  
  
            value = list1[i]  
  
            # Move elements of list1[0..i-1], that are  
            # greater than value, to one position ahead  
            # of their current position  
            j = i - 1  
            while j >= 0 and value < list1[j]:  
                list1[j + 1] = list1[j]  
                j -= 1  
            list1[j + 1] = value  
        return list1  
            # Driver code to test above  
  
list1 = [10, 5, 13, 8, 2]  
print("The unsorted list is:", list1)  
  
print("The sorted list1 is:", insertion_sort(list1)) 

Question 5:-
 Python program to sort a list of strings
 
lst = ['gfg', 'is', 'a', 'portal', 'for', 'geeks']
 
# Using sort() function
lst.sort()
 
print(lst)

METHOD 2:-
mylist = ["world", "LearnPython.com", "pineapple", "bicycle"]
>>> sorted_list = sorted(mylist)
>>> print(sorted_list)
['LearnPython.com', 'bicycle', 'pineapple', 'world']
