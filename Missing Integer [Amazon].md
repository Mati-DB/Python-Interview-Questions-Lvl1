
# Missing Integer [Amazon]
Please note that all the information regarding the case study has been sourced from the following [link](https://datalemur.com/questions/python-missing-integer).

## Index
 - [Interview Question](#Interview-Question)
 - [Solution](#Solution)

***

## Interview Question
Given an input list containing 𝑛 distinct numbers in the range 0 to 𝑛, return the only number in the range that is missing from the list.

For example, given ```input = [0,1,3]```, return ```2```. Because the input list has 3 elements in it, we expect to see the numbers 0 to 3 in there, but 2 is missing.

Another example: given ```input = [4, 3, 2, 1]```, return ```0```. We return 0 becuase the input list has 4 elements in it, so we expect to see the numbers 0 to 4 in there, but 0 itself is missing!
***

## Solution

```python
def missing_int(input_list):
    
    # Loop through numbers from 0 to the length of the input list
    for i in range(len(input_list) + 1):
        
        # Check if the current number is in the input list
        if i in input_list:
            
            # If true, continue to the next iteration
            continue
        
        else:
            
            # If false, return the current number as the missing integer
            return i
```
