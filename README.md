# competitive-programming
```
import sys
import collections
import math
import itertools

# Fast input/output (I/O)
input = sys.stdin.read  # For faster input when reading large inputs at once
# input = sys.stdin.readline  # For reading input line by line if needed
output = sys.stdout.write  # For faster output

# Utility Functions
def input_int(): return int(input().strip())
def input_str(): return input().strip()
def input_list(): return list(map(int, input().split()))
def input_str_list(): return input().split()

# Custom debug function
def debug(*args):
    print("DEBUG:", *args, file=sys.stderr)

# Main function to solve the problem
def solve():
    n = input_str().split(';');
    res = 0
    for probs in n:
        if "-" in probs:
            start, end = probs.split("-")
            res += int(end) - int(start) + 1
        else:
            res += 1
    
    # Example input format:
    # n = input_int()  # Single integer
    # arr = input_list()  # List of integers
    # You can process inputs in various formats as required

    # Write your solution logic here
    
    print(res)  # Remove once logic is added

# Entry point
if __name__ == "__main__":
    solve()
```
