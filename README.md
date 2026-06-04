# Two-Sum-II-Input-Array-Is-Sorted
numbers = list(map(int,input("Enter sorted numbers: ").split()))
target = int(input("Enter target: "))
left = 0
right = len(numbers) - 1
while left < right:
    s = numbers[left] + numbers[right]
    if s == target:
        print([left + 1, right + 1])  
        break
    elif s < target:
        left += 1
    else:
        right -= 1
