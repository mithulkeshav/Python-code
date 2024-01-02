write a program to accept integer array and search a particular value in the array , if it exists then the function should display “exists” otherwise should display “does not exists”.
# Function to search for a value in an array
def search_value(arr, value):
 for i in range(len(arr)):
 if arr[i] == value:
 return i # Return the index where the value is found
 return -1 # Return -1 if the value is not found
# Input: Accept an integer array from the user
arr = list(map(int, input("Enter integers separated by spaces: ").split()))
# Input: Accept the value to search for
search_val = int(input("Enter the value to search for: "))
# Search for the value in the array
result = search_value(arr, search_val)
if result != -1:
 print(f"{search_val} found at index {result}.")
else:
 print(f"{search_val} not found in the array.")
