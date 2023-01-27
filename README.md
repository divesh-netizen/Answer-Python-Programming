# Answer-Python-Programming

1. Write a Python program that finds the longest common substring between two strings.

x = "asdfcg"
y = "asdf"

def get_longest_substring(m, n, count):
  if(m==0 or n == 0):
    return count
  if(x[m-1] == y[n-1]:
    count = get_longest_substring(m-1,n-1, count)
  count = max(count, max(get_longest_substring(i, j-1, 0), 
            get_longest_substring(i-1, j, 0))
  return count
  

print(get_longest_substring(len(x), len(y), 0)


2. Implement a Python function that takes a list of integers and a target number as input, and returns a tuple of two integers that add up to the target number.

def Solve(lst, num):
  i = 0
  n = len(lst)-1
  while(i<n):
    if lst[i] + lst[n] == num:
      return (lst[i], lst[n])
    if lst[i] + lst[n] < num:
      i+=1
    if lst[i] + lst[n] > num:
      n -= 1
    return -1


lst = [1, 2, 3, 5, 6, 7, 9]
num = 9
print(Solve(lst, num)

