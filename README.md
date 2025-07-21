# p1
arr = [7, 1, 9, 3, 6, 9, 5]
n = len(arr)

max1 = arr[0]
max2 = arr[0]

for i in range(1, n):
    if arr[i] > max1:
        max2 = max1
        max1 = arr[i]
    elif arr[i] < max1 and (max2 == max1 or arr[i] > max2):
        max2 = arr[i]

if max1 == max2:
    print("There is no second highest element.")
else:
    print("Second highest element:", max2)
