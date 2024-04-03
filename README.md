# Pair-the-container in python
numContainers = int(input())
containers = list(map(int, input().split()))
containers.sort(reverse=True)
left = 0
right = numContainers - 1
while left < right:
    print(containers[left], containers[right])
    left += 1
    right -= 1
if numContainers % 2 != 0:
    print(containers[left], 0)
