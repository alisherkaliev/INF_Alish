# INF_Alish
Just repo.
#Bubble sort
inp = input("Enter a list element separated by space ")
elm = inp.split()
tmp = 0;

print("Elements of original array: ");
for i in range(0, len(elm)):
    print(elm[i], end=" ");

for i in range(0, len(elm)):
    for j in range(i+1, len(elm)):
        if(elm[i] > elm[j]):
            tmp = elm[i];
            elm[i] = elm[j];
            elm[j] = tmp;

print();

print("Elements of array sorted in ascending order by Bubble Sort: ");
for i in range(0, len(elm)):
 print(elm[i], end=" ");
