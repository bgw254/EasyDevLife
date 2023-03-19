Here are some Python coding interview templates for different patterns:

### Sliding Window

### Maximum Sum Subarray of Size K

```
def max_sum_subarray(arr, k):
    window_sum = sum(arr[:k])
    max_sum = window_sum
    for i in range(k, len(arr)):
        window_sum += arr[i] - arr[i-k]
        max_sum = max(max_sum, window_sum)
    return max_sum

```

### Two Pointers

### Two Sum

```
def two_sum(nums, target):
    left, right = 0, len(nums) - 1
    while left < right:
        current_sum = nums[left] + nums[right]
        if current_sum == target:
            return [left, right]
        elif current_sum < target:
            left += 1
        else:
            right -= 1
    return []

```

### Depth-First Search

### Permutations

```
def permute(nums):
    def backtrack(first = 0):
        if first == n:
            output.append(nums[:])
        for i in range(first, n):
            nums[first], nums[i] = nums[i], nums[first]
            backtrack(first + 1)
            nums[first], nums[i] = nums[i], nums[first]

    n = len(nums)
    output = []
    backtrack()
    return output

```

### Breadth-First Search

### Level Order Traversal

```
from collections import deque

def level_order(root):
    if not root:
        return []
    result = []
    queue = deque()
    queue.append(root)
    while queue:
        level_size = len(queue)
        current_level = []
        for _ in range(level_size):
            current_node = queue.popleft()
            current_level.append(current_node.val)
            if current_node.left:
                queue.append(current_node.left)
            if current_node.right:
                queue.append(current_node.right)
        result.append(current_level)
    return result

```

### Backtracking

### Letter Combinations of a Phone Number

```
def letter_combinations(digits):
    if not digits:
        return []
    phone_map = {
        '2': 'abc',
        '3': 'def',
        '4': 'ghi',
        '5': 'jkl',
        '6': 'mno',
        '7': 'pqrs',
        '8': 'tuv',
        '9': 'wxyz'
    }
    def backtrack(index, path):
        if len(path) == len(digits):
            result.append(path)
            return
        for letter in phone_map[digits[index]]:
            backtrack(index + 1, path + letter)
    result = []
    backtrack(0, '')
    return result


def generate_parentheses(n):
    def backtrack(s, left, right):
        if len(s) == 2 * n:
            output.append(s)
            return
        if left < n:
            backtrack(s + '(', left + 1, right)
        if right < left:
            backtrack(s + ')', left, right + 1)

    output = []
    backtrack('', 0, 0)
    return output

def permute(nums):
    def backtrack(first = 0):
        if first == n:
            output.append(nums[:])
        for i in range(first, n):
            nums[first], nums[i] = nums[i], nums[first]
            backtrack(first + 1)
            nums[first], nums[i] = nums[i], nums[first]
s
    n = len(nums)
    output = []
    backtrack()
    return output

```



### Dynamic Programming

### Longest Increasing Subsequence

```
def longest_increasing_subsequence(nums):
    n = len(nums)
    dp = [1] * n
    for i in range(1, n):
        for j in range(i):
            if nums[j] < nums[i]:
                dp[i] = max(dp[i], dp[j] + 1)
    return max(dp)

```

I hope these templates are helpful! Let me know if you have any questions or if there's anything else I can help you with!