# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: Mohanish.k
RegisterNumber: 22002294

def selection_sort(nums):
    # write your code here using selection sort
    for i in range(len(nums)):
        lowest_value_index = i
        for j in range (i+1,len(nums)):
            if nums[j] < nums[lowest_value_index]:
                lowest_value_index=j
        nums[i], nums[lowest_value_index]=nums[lowest_value_index],nums[i]

list_of_nums = eval(input())
# use the selection sort function
# print the sorted list
selection_sort(list_of_nums)
print(list_of_nums)





```
ii)	#Insertion Sort
```
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: Mohanish.K
RegisterNumber: 22002294

def insertion_sort(nums):
    # Write your code here to sort the elements in the list using Insertion sort algorithm
    for i in range(1,len(nums)):
        item_to_insert = nums[i]
        j=i-1
        while j>=0 and nums[j]>item_to_insert:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1]=item_to_insert
    
    
list_of_nums = eval(input())
# use the insertion sort function to get the sorted list
# print the sorted list
insertion_sort(list_of_nums)
print(list_of_nums)





```

## Input:
1)![WhatsApp Image 2023-01-24 at 9 31 41 AM](https://user-images.githubusercontent.com/111619160/214209980-c0652048-1286-4fb7-9a1f-e369af95a658.jpeg)
2)![WhatsApp Image 2023-01-24 at 9 31 45 AM](https://user-images.githubusercontent.com/111619160/214209992-21f7f674-2b9b-4dc9-b396-80c52f3d5cfd.jpeg)
##OUTPUT:
3)![WhatsApp Image 2023-01-24 at 9 31 55 AM](https://user-images.githubusercontent.com/111619160/214210006-4555ce63-fde0-41b7-8235-39a29cd100a3.jpeg)
4)![WhatsApp Image 2023-01-24 at 9 32 02 AM](https://user-images.githubusercontent.com/111619160/214210014-ceefd0b9-b76b-4912-b803-40b7aeeb9dcc.jpeg)



## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
