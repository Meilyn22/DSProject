# Single Number.

`Given a non-empty array of integers nums, every element appears twice except for one. Find that single one.
You must implement a solution with a linear runtime complexity and use only constant extra space.
`

Example 1:

```
Input: nums = [2,2,1].

Output: 1
```
Example 2:

```
Input: nums = [4,1,2,1,2]

Output: 4
```

Example 3:

```
Input: nums = [1]

Output: 1
```

## My solution.

We can solve this problem in O(n) time and constant space if we use a dictionary.
First of all we would want to use a frequency counter in this case to see how many times a single number appears.

``` python

    def singleNumber(nums):
        # dictionary to hold frequency. 
        a = {}
        # loop over the numbers in the list.
        for i in nums:
        # if the numbers are in the dictionary as keys, 
        # then we want to increment the value by 1.
            if i in a:
                a[i] += 1
        # if the key is not in the dictionary, 
        # we want to add the key and assign the value as one. 
            else:
                a[i] = 1
        # We can loop over our dictionary and 
        # return the key where the value is 1.       
        for key, value in a.items():
            if value == 1:
                return(key)
```

# Find All Numbers Disappeared in an Array.

`Given an array nums of n integers where nums[i] is in the range [1, n], return an array of all the integers in the range [1, n] that do not appear in nums.
`

Example 1:
```
Input: nums = [4,3,2,7,8,2,3,1]

Output: [5,6]
```


Example 2:
```
Input: nums = [1,1]

Output: [2]
```

## My solution.

We are supposed to return an array of numbers that aren't in the range. A range can be from 1-10, 0-50 or 50-10. In this case our range is from 1-n. n represents the length of our list.

Our edge case here is if there are duplicate numbers. So we need to watch out for that since it can mess up our program. We are going to use a set to eliminate an duplicate we might have. This solution is O(n).

``` python
    def findDisappearedNumbers(nums):
        # Our set will help us eliminate 
        # any duplicate we might have. 
        setn = set(nums)
        # We need a stack or a list 
        # to put the numbers that don't appear. 
        a = []
        # We iterate over the nums list
        # and also grab our range from 1 - len(nums).
        for i,v in enumerate(nums, 1):
            # if any number from 1-len(nums) doesn't appear in our set
            # then we want to append that number to our list and return the list.
            if i not in setn:
                a.append(i)
        return a
```

# Contains Duplicate
`Given an integer array nums, return true if any value appears at least twice in the array, and return false if every element is distinct.`

Example 1:

```
Input: nums = [1,2,3,1]

Output: true
```

Example 2:

```
Input: nums = [1,2,3,4]

Output: false
```

Example 3:

```
Input: nums = [1,1,1,3,3,4,3,2,4,2]

Output: true
```

## My solution.

We want to return true if any number in our array appears twice.
We will use a set since sets help us eliminate duplicates. We will create a set and then use it to compare the length of our list>

``` python
    def containsDuplicate(nums):
        # Create our set to help eliminate duplicates. 
        num = set(nums)
        
        # Then we check if the num list has 
        # the same number of items as our set.
        if len(num) == len(nums):
            # if they have the same number of items, 
            # then our list isn't a duplicate. Else, it's a duplicate.
            return False
        else:
            return True
```

# Missing Number

`
Given an array nums containing n distinct numbers in the range [0, n], return the only number in the range that is missing from the array.
`

Example 1:
```
Input: nums = [3,0,1]

Output: 2

Explanation: n = 3 since there are 3 numbers, so all numbers are in the range [0,3]. 2 is the missing number in the range since it does not appear in nums.
```

Example 2:
```
Input: nums = [0,1]

Output: 2

Explanation: n = 2 since there are 2 numbers, so all numbers are in the range [0,2]. 2 is the missing number in the range since it does not appear in nums.

```
Example 3:
```
Input: nums = [9,6,4,2,3,5,7,0,1]

Output: 8

Explanation: n = 9 since there are 9 numbers, so all numbers are in the range [0,9]. 8 is the missing number in the range since it does not appear in nums.
```

## My Solution

``` python
    def missingNumber(nums:)
        for i in range(0, len(nums)+1):
            if i not in nums:
                return i
```