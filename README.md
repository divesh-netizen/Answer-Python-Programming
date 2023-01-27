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


2. 

