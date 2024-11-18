# Index-After-Rotations

Emma has an array of n unique integers arranged in ascending order, and she enjoys experimenting with it. One of her favorite activities is to rotate the array counterclockwise. In each rotation, she moves the last element of the array to the beginning, shifting all other elements one position to the right. After performing this rotation k times, Emma is curious: what will be the new index of the original first element in the rotated array? Can you help her figure out its position?

# Input reading
n = int(input())  # Size of the array
arr = list(map(int, input().split()))  # The array (not actually needed for the calculation)
k = int(input())  # Number of rotations

# Calculate the new index of the original first element
new_index = (k % n) + 1

# Output the result
print(new_index)
