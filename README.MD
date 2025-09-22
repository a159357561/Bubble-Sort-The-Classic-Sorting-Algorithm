Title

# “Bubble Sort: The Classic Sorting Algorithm”

## Content

In computer science, sorting is one of the most fundamental problems. Although modern applications use advanced algorithms like Quick Sort or Merge Sort, the Bubble Sort remains a classic example often taught to beginners.

## How It Works

Bubble Sort repeatedly steps through the list, compares adjacent items, and swaps them if they are in the wrong order. This process continues until no swaps are needed.

## Pseudocode
```
procedure bubbleSort(A : list of sortable items)
  n = length(A)
  repeat
    swapped = false
    for i = 1 to n-1 do
      if A[i] > A[i+1] then
        swap(A[i], A[i+1])
        swapped = true
      end if
    end for
  until not swapped
end procedure
```

## Example in Python
```
def bubble_sort(arr):
    n = len(arr)
    for i in range(n):
        for j in range(0, n - i - 1):
            if arr[j] > arr[j + 1]:
                arr[j], arr[j + 1] = arr[j + 1], arr[j]
    return arr

print(bubble_sort([5, 2, 9, 1, 5, 6]))
```

## Pros & Cons

✅ Easy to understand and implement
✅ Good for teaching the basics of algorithm design
❌ Very inefficient for large datasets (O(n²) time complexity)

## Conclusion

Bubble Sort may not be practical today, but it remains an important stepping stone in learning programming fundamentals. It introduces the ideas of iteration, conditionals, and algorithm efficiency — key concepts that every programmer needs.
