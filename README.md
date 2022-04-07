# INF_Alish
Just repo.
#Bubble sort
inp = input("Enter a list element separated by space ")
elm = inp.split()
tmp = 0;

print("Elements of original array: ");


  i = low - 1

for i in range(0, len(elm)):
  for j in range(low, high):
    if array[j] <= pivot:
      i = i + 1
      (array[i], array[j]) = (array[j], array[i])
  (array[i + 1], array[high]) = (array[high], array[i + 1])

print();
def quickSort(array, low, high):
  if low < high:
    pi = partition(array, low, high)
    quickSort(array, low, pi - 1)
    quickSort(array, pi + 1, high)
    
quickSort(elm, 0, size - 1)

print("Elements of array sorted in ascending order by Bubble Sort: ");
for i in range(0, len(elm)):
 print(elm[i], end=" ");
