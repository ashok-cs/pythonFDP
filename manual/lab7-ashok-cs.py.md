# Removing duplicates from a list

## Problem statement
Remove all duplicates from a list.

Examples

    input1=[23,12,12,14]
    output1=[23,12,14]

    input2=[12,12,12,12]      
    output2=[12]

    input3=[12,34,34,34]
    output3=[12,34]

## Pseudocode
```code

remove_duplicates():
input:mList
1. Initialize: result_list = emptyList
2. for each num in the mList,
    if num is not found in the result_list,
      append num to the result_list.
output:result_list
```

## Program
```python

def remove_duplicates(mList):
  result_list=[]
  for num in mList:
    if num not in result_list:
      result_list.append(num)
  return result_list
 ```
 
 ## Testing
 ```python
 
 def test(input,output):
  result=remove_duplicates(input)
  print("Given input: ",input)
  print("Expected output: ",output)
  print("Actual output: ",result)
  if result==output:
    print("Test case: pass")
  else:
    print("Test case: fail")
  
#Test cases
input1=[23,12,12,14]
output1=[23,12,14]
test(input1,output1)
input2=[12,12,12,12]      
output2=[12]
test(input2,output2)
input3=[12,34,34,34]
output3=[12,34]
test(input3,output3)
```
## Output
```
Given input:  [23, 12, 12, 14]
Expected output:  [23, 12, 14]
Actual output:  [23, 12, 14]
Test case: pass
Given input:  [12, 12, 12, 12]
Expected output:  [12]
Actual output:  [12]
Test case: pass
Given input:  [12, 34, 34, 34]
Expected output:  [12, 34]
Actual output:  [12, 34]
Test case: pass
```

## Viva Questions

1. What is immutable datatype. Why list is mutable.
2. How do you modify the code to check if all the elements in the list are integer values
3. How do you use `set()` to remove duplicates in a list.
4. Mention any two applications of `remove_duplicates()`
5. Modify the code to output only the elements which have duplicate entries.
```
Examples:
    input1=[23,12,12,14]
    output1=[12]

    input2=[12,12,12,12]      
    output2=[12]

    input3=[12,34,34,34]
    output3=[34]
```
6. Modify the code to output the elements with repeated entries along with their count. 
```
Examples:
    input1=[23,12,12,14]
    output1={12:2}

    input2=[12,12,12,12]      
    output2={12:4}

    input3=[12,34,34,34]
    output3={34:3}
 ```
 Note: The output is a dictionary.
