# Find a string

The user enters a string and a substring. You have to print the number of times that the substring occurs in the given string. String traversal will take place from left to right, not from right to left.

NOTE: String letters are case-sensitive.


```python

def count_substring(string, sub_string):
  count = 0
  for i in range(0, len(string)):
    if string[i:i + len(sub_string)] == sub_string:
      count+=1
  return count

if __name__ == '__main__':
    string = input().strip()
    sub_string = input().strip()
    
    count = count_substring(string, sub_string)
    print(count)
```
