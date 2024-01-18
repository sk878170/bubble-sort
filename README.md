Bubble sort is a simple sorting algorithm used to arrange a list of elements in a specific order, usually from the smallest to the largest. It gets its name because the smaller elements "bubble" to the top of the list, like bubbles rising in water.

Algorithm:

1. Comparison:
   - The algorithm starts by comparing the first two elements of the list. 
   - If the first element is larger than the second, they swap places; otherwise, they stay where they are.

2. Move to the Next Pair:
   - The algorithm then moves on to compare the second and third elements. Again, if the second element is larger than the third, they swap places.

3. Continue Comparing and Swapping:
   - This process continues, comparing and swapping adjacent elements until the algorithm reaches the end of the list.

4. First Pass:
   - After the first pass through the list, the largest element has "bubbled up" to the end of the list.

5. Repeat:
   - The algorithm repeats this process for the remaining elements in the list, excluding the last (already sorted) element.

6. Multiple Passes:
   - Bubble sort continues with multiple passes until the entire list is sorted.

Time Complexity: O(n^2)

Space Complexity: O(1) 

code explaination:
Certainly! Let's go through the code step by step:

```python
def bubble_sort(list):
    for i in range(length):
        for j in range(length-i-1):
            if list[j] > list[j+1]:
                list[j], list[j+1] = list[j+1], list[j]
    return list

length = int(input("Enter the length of list:"))
list = []
for k in range(length):
    num = int(input("Enter a number:"))
    list.append(num)

print("Given list:", list)
sorted_list = bubble_sort(list)
print("The sorted list:", sorted_list)
```

1. Function `bubble_sort`:
    - This function takes a list as an input parameter and performs the bubble sort algorithm on it.
    - The outer loop (`for i in range(length)`) iterates through each element of the list.
    - The inner loop (`for j in range(length-i-1)`) iterates through the unsorted portion of the list.
    - The `if` statement checks if the current element (`list[j]`) is greater than the next element (`list[j+1]`). If true, it swaps them using tuple assignment (`list[j], list[j+1] = list[j+1], list[j]`).
    - This process is repeated for each element, ensuring that the largest element "bubbles up" to its correct position in each pass.

2. Taking Input for List:
    - The code first asks the user to input the length of the list (`length`).
    - Then, a loop (`for k in range(length)`) is used to take user input for each element of the list, which is appended to the `list` using `list.append(num)`.

3. Printing the Given List:
    - The code prints the original list that the user entered using `print("Given list:", list)`.

4. Sorting and Printing the Sorted List:
    - The `bubble_sort` function is called with the user-entered list (`sorted_list = bubble_sort(list)`).
    - The sorted list is then printed using `print("The sorted list:", sorted_list)`.




