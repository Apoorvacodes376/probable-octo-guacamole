# A-December-of-Algorithms-2026

<div align="left">
<h1>
    <p align="center"><img alt="header" src="https://github.com/user-attachments/assets/0e894f27-882b-4e5d-a75d-7b2b9505e90d" width="500"></img></p>

</h1>
Welcome to A December of Algorithms 2026.

Building on the success and enthusiasm of previous years, we’re excited to bring you a fresh selection of algorithms to explore and implement this December!

Each Day, Each Algorithm ;)
Finish them all to get a certificate :)

**Send a pull request only after completing all 31 algorithms.**

**Please submit all PRs on or before January 1st 2027, 11:59 PM IST.**

## What Do I Do?

We have a small collection of algorithms, one for every day of the month. Scroll down to take a look at them.

All you need to do is fork this repository, implement all 31 algorithms and send a pull request over to us.

Check out our FAQ for more information.

## Index

1. [December 01 - Snack Pair Counter](#december-01---snack-pair-counter)
2. [December 02 - K-th Element of Two Sorted Arrays](#december-02---k-th-element-of-two-sorted-arrays)
3. [December 03 - Roman Numeral Converter with Digit Sum](#december-03---roman-numeral-converter-with-digit-sum)
4. [December 04 - Project TRI-FLOW – Detect the Three-Phase Traffic Pattern](#december-04---project-tri-flow--detect-the-three-phase-traffic-pattern)
5. [December 05 - Two Sum with Minimum Index Distance](#december-05---two-sum-with-minimum-index-distance)
6. [December 06 - Merge Two Sorted Lists (Excluding Negative Nodes)](#december-06---merge-two-sorted-lists-excluding-negative-nodes)
7. [December 07 - Sort an Array of Strings According to String Lengths](#december-07---sort-an-array-of-strings-according-to-string-lengths)
8. [December 08 - The Smart Campus Resource Tracker](#december-08---the-smart-campus-resource-tracker)
9. [December 09 - Smallest Subarray with Sum Greater Than a Given Value](#december-09---smallest-subarray-with-sum-greater-than-a-given-value)
10. [December 10 - Restore Friends' Finishing Order](#december-10---restore-friends-finishing-order)
11. [December 11 - Valid Palindrome](#december-11---valid-palindrome)
12. [December 12 - Add Digits](#december-12---add-digits)
13. [December 13 - Cargo Balance Triples](#december-13---cargo-balance-triples)
14. [December 14 - Cipher Crate Sorting](#december-14---cipher-crate-sorting)
15. [December 15 - Crater Fields](#december-15---crater-fields)
16. [December 16 - Fuel Cell Combinations](#december-16---fuel-cell-combinations)
17. [December 17 - Spore Spread](#december-17---spore-spread)
18. [December 18 - Module Boot Order](#december-18---module-boot-order)
19. [December 19 - Telemetry Climb](#december-19---telemetry-climb)
20. [December 20 - Maintenance Windows](#december-20---maintenance-windows)
21. [December 21 - Fuel Flow Intervals](#december-21---fuel-flow-intervals)
22. [December 22 - Median of Two Sorted Arrays](#december-22---median-of-two-sorted-arrays)
23. [December 23 - Unique Paths](#december-23---unique-paths)
24. [December 24 - Lunar Mining Colony: Dome Oxygen Containment](#december-24---lunar-mining-colony-dome-oxygen-containment)
25. [December 25 - Reactor Rod — Squared Cutting Cost](#december-25---reactor-rod--squared-cutting-cost)
26. [December 26 - Alternating-Sensor Transformations](#december-26---alternating-sensor-transformations)
27. [December 27 - Checkpoint-Safe Storage Rectangle](#december-27---checkpoint-safe-storage-rectangle)
28. [December 28 - Peak Window Baseline](#december-28---peak-window-baseline)
29. [December 29 - Bounded Palindrome Archive](#december-29---bounded-palindrome-archive)
30. [December 30 - Maximum Path Sum in a Binary Tree](#december-30---maximum-path-sum-in-a-binary-tree)
31. [December 31 - Count All Possible Routes](#december-31---count-all-possible-routes)

---

## December 01 - Snack Pair Counter

### Problem Statement

A school is organizing a snack distribution event where students receive snack packs with assigned points. Given an integer array points and an integer target, count the number of non-adjacent pairs (i < j where j - i > 1) such that points[i] + points[j] == target.

### Input Format

- Line 1: An integer n (number of snack packs).
- Line 2: n space-separated integers representing points.
- Line 3: An integer target.

### Output Format

Print a single integer representing the total number of valid non-adjacent pairs.

### Sample Input 1

```text
5
1 2 4 5 3
6
```

### Sample Output 1

```text
1
```

### Sample Input 2

```text
5
3 1 2 4 2
5
```

### Sample Output 2

```text
3
```

### Sample Input 3

```text
4
1 2 3 4
10
```

### Sample Output 3

```text
0
```

### Explanation

- Sample 1: Valid pair is (1, 5) at indices (0, 3) summing to 6.
- Sample 2: Valid non-adjacent pairs summing to 5 are (3, 2) at (0, 2), (3, 2) at (0, 4), and (1, 4) at (1, 3).
- Sample 3: No non-adjacent pairs sum to 10.

### Constraints

- 2 ≤ n ≤ 1000
- -1000 ≤ points[i] ≤ 1000
- -2000 ≤ target ≤ 2000

### Reference

- [Codeforces 1538C – Number of Pairs](https://codeforces.com/problemset/problem/1538/C) — Counts pairs whose sum lies within a specified range.
- [Codeforces 2051D – Counting Pairs](https://codeforces.com/problemset/problem/2051/D) — Counts pairs satisfying a condition involving the array sum.

---

## December 02 - K-th Element of Two Sorted Arrays

### Problem Statement

Given two sorted arrays `a[]` and `b[]` and an integer `k`, find the element that would be at the `k`-th position (1-based indexing) of the combined sorted array.

### Input Format

- The first line contains three integers `n`, `m`, and `k`, representing the sizes of `a[]` and `b[]` and the target position `k`.
- The second line contains `n` space-separated integers for `a[]`.
- The third line contains `m` space-separated integers for `b[]`.

### Output Format

Print a single integer representing the `k`-th element of the combined sorted array.

### Sample Input 1

```text
5 4 5
2 3 6 7 9
1 4 8 10
```

### Sample Output 1

```text
6
```

### Sample Input 2

```text
5 5 6
1 4 8 10 12
5 7 11 15 17
```

### Sample Output 2

```text
10
```

### Explanation

In sample 1, the combined sorted array is `[1, 2, 3, 4, 6, 7, 8, 9, 10]`, and the 5th element is `6`. In sample 2, the combined sorted array is `[1, 4, 5, 7, 8, 10, 11, 12, 15, 17]`, and the 6th element is `10`.

### Constraints

- `1 ≤ n, m ≤ 10^5`
- `1 ≤ k ≤ n + m`
- `0 ≤ a[i], b[i] ≤ 10^9`
- Both arrays are sorted in non-decreasing order.

### Reference

- [GeeksforGeeks – K-th Element of Merged Two Sorted Arrays](https://www.geeksforgeeks.org/dsa/k-th-element-two-sorted-arrays/)

---

## December 03 - Roman Numeral Converter with Digit Sum

### Problem Statement

Roman numerals are represented using seven symbols: `I`, `V`, `X`, `L`, `C`, `D`, and `M`.

Given a valid Roman numeral string `s`, convert it into its decimal integer representation. After converting it, calculate the sum of all the digits of the resulting integer. Return both the converted integer and its digit sum.

### Input Format

- A single string `s` representing a valid Roman numeral.

### Output Format

Print two integers separated by a space:
1. The decimal integer equivalent of the Roman numeral.
2. The sum of the digits of that integer.

### Sample Input 1

```text
III
```

### Sample Output 1

```text
3 3
```

### Sample Input 2

```text
LVIII
```

### Sample Output 2

```text
58 13
```

### Sample Input 3

```text
MCMXCIV
```

### Sample Output 3

```text
1994 23
```

### Explanation

In sample 1, `III` equals `3`, and its digit sum is `3`. In sample 2, `LVIII` equals `58`, and `5 + 8 = 13`. In sample 3, `MCMXCIV` equals `1994`, and `1 + 9 + 9 + 4 = 23`.

### Constraints

- `1 ≤ length of s ≤ 15`
- `s` contains only valid Roman numeral symbols (`I`, `V`, `X`, `L`, `C`, `D`, `M`).
- The resulting integer is between `1` and `3999`.

### Reference

- [LeetCode – Roman to Integer](https://leetcode.com/problems/roman-to-integer/)

---

## December 04 - Project TRI-FLOW – Detect the Three-Phase Traffic Pattern

### Problem Statement

A smart city traffic management system monitors vehicle speeds at consecutive checkpoints and identifies a special three-phase speed pattern called a **Trionic Array**:
1. **Acceleration Phase:** Vehicle speed strictly increases.
2. **Deceleration Phase:** Vehicle speed strictly decreases.
3. **Re-acceleration Phase:** Vehicle speed strictly increases again.

All three phases must be non-empty (each must contain at least one transition), and equal adjacent elements are not allowed. Determine whether the given speed array represents a valid Trionic Array.

### Input Format

- The first line contains an integer `n`, representing the number of checkpoints.
- The second line contains `n` space-separated integers representing vehicle speeds recorded at each checkpoint.

### Output Format

Print `true` if the given array is a Trionic Array; otherwise, print `false`.

### Sample Input 1

~~~
7
1 3 5 4 2 6 8
~~~

### Sample Output 1

~~~
true
~~~

### Sample Input 2

~~~
6
1 2 3 4 5 6
~~~

### Sample Output 2

~~~
false
~~~

### Sample Input 3

~~~
6
1 4 3 2 5 4
~~~

### Sample Output 3

~~~
false
~~~

### Explanation

In sample 1, the speeds strictly increase (`1 → 3 → 5`), strictly decrease (`5 → 4 → 2`), and strictly increase again (`2 → 6 → 8`). In sample 2, the array only increases without a decreasing phase. In sample 3, the final phase decreases instead of increasing.

### Constraints

- `4 ≤ n ≤ 10^5`
- `0 ≤ speed[i] ≤ 10^9`
- Equal adjacent elements are not allowed in valid transitions.

### Reference

- LeetCode – Trionic Array I: https://leetcode.com/problems/trionic-array-i/

---

## December 05 - Two Sum with Minimum Index Distance

### Problem Statement

A college is organizing a technical event. Each student has a score, and the organizers want to find two students whose combined scores equal a given target score `T`, with at least `D` positions between their indices in the registration list.

Given an array `A` of `N` integers representing student scores, a target sum `T`, and a minimum index distance `D`, find two indices `i` and `j` such that:
1. `i < j`
2. `A[i] + A[j] == T`
3. `j - i >= D`

If multiple valid pairs exist, choose the pair with the smallest second index `j`. If there are multiple choices for the same `j`, choose the smallest first index `i`. If no valid pair exists, print `-1 -1`.

### Input Format

- The first line contains three integers `N`, `T`, and `D`.
- The second line contains `N` space-separated integers representing the array `A`.

### Output Format

Print two space-separated integers `i` and `j`, or `-1 -1` if no valid pair exists.

### Sample Input 1

~~~
5 9 2
2 7 11 15 2
~~~

### Sample Output 1

~~~
1 4
~~~

### Sample Input 2

~~~
4 6 3
3 2 4 3
~~~

### Sample Output 2

~~~
0 3
~~~

### Sample Input 3

~~~
3 10 2
5 5 1
~~~

### Sample Output 3

~~~
-1 -1
~~~

### Explanation

In sample 1, `(0, 1)` sums to `9` but has distance `1 < 2`, so `(1, 4)` (`7 + 2 = 9`, distance `3`) is chosen. In sample 2, `(0, 3)` sums to `6` with distance `3`. In sample 3, no pair sums to `10` with distance at least `2`.

### Constraints

- `2 ≤ N ≤ 10^5`
- `1 ≤ D < N`
- `-10^9 ≤ A[i], T ≤ 10^9`

### Reference

- LeetCode – Two Sum: https://leetcode.com/problems/two-sum/

---

## December 06 - Merge Two Sorted Lists (Excluding Negative Nodes)

### Problem Statement

You are given the heads of two sorted linked lists `list1` and `list2`.

Merge the two lists into one sorted list by splicing together the nodes of the first two lists. **Any node with a negative value must be left out of the merged list.** Return the head of the merged linked list.

### Input Format

- The first line contains two integers `n` and `m`, the lengths of `list1` and `list2`.
- The second line contains `n` space-separated integers for `list1` (omit if `n = 0`).
- The third line contains `m` space-separated integers for `list2` (omit if `m = 0`).

### Output Format

Print the space-separated values of the merged non-negative linked list, or `[]` if the resulting list is empty.

### Sample Input 1

~~~
3 3
-3 1 4
0 2 5
~~~

### Sample Output 1

~~~
0 1 2 4 5
~~~

### Sample Input 2

~~~
2 1
-2 -1
-5
~~~

### Sample Output 2

~~~
[]
~~~

### Sample Input 3

~~~
0 1
0
~~~

### Sample Output 3

~~~
0
~~~

### Explanation

In sample 1, `-3` is excluded and the remaining nodes merge into `[0, 1, 2, 4, 5]`. In sample 2, all nodes are negative and excluded, leaving an empty list `[]`. In sample 3, `0` is non-negative and remains in the merged list.

### Constraints

- The number of nodes in both lists is in the range `[0, 200]`.
- `-1000 ≤ Node.val ≤ 1000`
- Both `list1` and `list2` are sorted in non-decreasing order.

### Reference

- [LeetCode – Merge Two Sorted Lists](https://leetcode.com/problems/merge-two-sorted-lists/)

---

## December 07 - Sort an Array of Strings According to String Lengths

### Problem Statement

Given an array `arr[]` of strings, sort the strings in ascending order based on their lengths. If two strings have the same length, their original relative order must be preserved in the final output (stable sort).

### Input Format

- The first line contains an integer `n`, the number of strings.
- The second line contains `n` space-separated strings.

### Output Format

Print the `n` sorted strings separated by spaces.

### Sample Input 1

~~~
4
GeeksforGeeks I from am
~~~

### Sample Output 1

~~~
I am from GeeksforGeeks
~~~

### Sample Input 2

~~~
4
You are beautiful looking
~~~

### Sample Output 2

~~~
You are looking beautiful
~~~

### Explanation

In sample 1, the lengths are `13, 1, 4, 2`, so sorting in ascending order gives `I am from GeeksforGeeks`. In sample 2, `You` and `are` both have length `3`, so `You` stays before `are`, followed by `looking` (length `7`) and `beautiful` (length `9`).

### Constraints

- `1 ≤ n ≤ 10^5`
- `1 ≤ length of each string ≤ 100`

### Reference
- [GeeksforGeeks – Sort an Array of Strings According to String Lengths](https://www.geeksforgeeks.org/sort-array-strings-according-string-lengths/)
- [LeetCode – Sort the People / Rearrange Words in a Sentence](https://leetcode.com/problems/rearrange-words-in-a-sentence/)

---

## December 08 - The Smart Campus Resource Tracker

### Problem Statement

A college is conducting a technical festival where students register every hour. Given an integer array `registrations`, where `registrations[i]` represents the number of students registered during hour `i`, calculate the cumulative total of registrations from the first hour up to each hour and return the resulting running sum array.

### Input Format

- The first line contains an integer `n`, the number of hours.
- The second line contains `n` space-separated integers representing `registrations`.

### Output Format

Print `n` space-separated integers representing the cumulative registrations after each hour.

### Sample Input 1

~~~
5
10 20 15 25 30
~~~

### Sample Output 1

~~~
10 30 45 70 100
~~~

### Sample Input 2

~~~
4
5 8 12 10
~~~

### Sample Output 2

~~~
5 13 25 35
~~~

### Explanation

In sample 1, the cumulative sums are `10`, `10 + 20 = 30`, `30 + 15 = 45`, `45 + 25 = 70`, and `70 + 30 = 100`. In sample 2, the cumulative sums are `5`, `5 + 8 = 13`, `13 + 12 = 25`, and `25 + 10 = 35`.

### Constraints

- `1 ≤ n ≤ 10^5`
- `0 ≤ registrations[i] ≤ 10^6`
- Expected time complexity: `O(n)`; auxiliary space: `O(1)` (excluding output).

### Reference
- LeetCode – Running Sum of 1D Array: https://leetcode.com/problems/running-sum-of-1d-array/

---

## December 09 - Smallest Subarray with Sum Greater Than a Given Value

### Problem Statement

Given a number `x` and an array of integers `arr[]`, find the length of the smallest contiguous subarray with a sum strictly greater than `x`. If no such subarray exists, return `0`.

### Input Format

- The first line contains two integers `n` and `x`, representing the size of the array and the target value `x`.
- The second line contains `n` space-separated integers representing `arr[]`.

### Output Format

Print a single integer representing the minimum subarray length with sum strictly greater than `x`, or `0` if none exists.

### Sample Input 1

~~~
6 51
1 4 45 6 0 19
~~~

### Sample Output 1

~~~
3
~~~

### Sample Input 2

~~~
5 100
1 10 5 2 7
~~~

### Sample Output 2

~~~
0
~~~

### Explanation

In sample 1, the minimum length subarray with a sum strictly greater than `51` is `[4, 45, 6]`, which has length `3` and sum `55`. In sample 2, the entire array sums to `25`, so no subarray has a sum greater than `100`.

### Constraints

- `1 ≤ n ≤ 10^5`
- `1 ≤ arr[i] ≤ 10^4`
- `1 ≤ x ≤ 10^9`
- Expected time complexity: `O(n)`; auxiliary space: `O(1)`.

### Reference
- [GeeksforGeeks – Smallest Subarray with Sum Greater than a Given Value](https://www.geeksforgeeks.org/minimum-length-subarray-sum-greater-given-value/)
- [LeetCode – Minimum Size Subarray Sum](https://leetcode.com/problems/minimum-size-subarray-sum/)

---

## December 10 - Restore Friends' Finishing Order

### Problem Statement

You are given an integer array `order` of length `n`, representing the finishing order of participants in a race. Each participant has a unique ID from `1` to `n`.

You are also given an integer array `friends`, containing the IDs of your friends in strictly increasing order.

Find and return an array containing only your friends' IDs, arranged according to their actual finishing order in the race.

### Input Format

- The first line contains two integers `n` and `m`, representing the number of participants and the number of friends, respectively.
- The second line contains `n` space-separated integers representing the participants' finishing order.
- The third line contains `m` space-separated integers representing the IDs of your friends.

### Output Format

Print the IDs of your friends in their finishing order, separated by spaces.

### Sample Input 1

~~~
5 3
3 1 2 5 4
1 3 4
~~~

### Sample Output 1

~~~
3 1 4
~~~

### Sample Input 2

~~~
5 2
1 4 5 3 2
2 5
~~~

### Sample Output 2

~~~
5 2
~~~

### Explanation

In Sample 1, the original finishing order is `[3, 1, 2, 5, 4]`. Among these participants, IDs `1`, `3`, and `4` belong to your friends, so their finishing order is `[3, 1, 4]`. In Sample 2, the friends have IDs `2` and `5`, and since participant `5` finishes before participant `2`, the resulting order is `[5, 2]`.

### Constraints

- `1 ≤ n ≤ 100`
- `1 ≤ m ≤ min(8, n)`
- `order` contains every integer from `1` to `n` exactly once.
- `1 ≤ friends[i] ≤ n`
- The `friends` array is sorted in strictly increasing order.
- Every ID in `friends` is guaranteed to exist in `order`.
- Target auxiliary space: `O(m)`

### Reference

- https://leetcode.com/problems/restore-finishing-order/description/?envType=problem-list-v2&envId=hash-table

---

## December 11 - Valid Palindrome

### Problem Statement

You are given a string `password` representing a password entered by a user.

A password is considered valid if it reads the same forward and backward after converting all uppercase letters into lowercase and removing all spaces and special characters.

Determine whether the given password is a palindrome. Return `true` if it is a palindrome; otherwise, return `false`.

### Input Format

- The first line contains a string `password`.

### Output Format

Print `true` if the password is a palindrome; otherwise, print `false`.

### Sample Input 1

~~~
Madam
~~~

### Sample Output 1

~~~
true
~~~

### Sample Input 2

~~~
Hello World
~~~

### Sample Output 2

~~~
false
~~~

### Explanation

In Sample 1, after converting the string to lowercase, it becomes `"madam"`. Reading it forward and backward gives the same result, so the output is `true`.

In Sample 2, `"helloworld"` is not the same when reversed, so the output is `false`.

### Constraints

- `1 ≤ password.length ≤ 200000`
- The string contains printable ASCII characters.
- The comparison must be case-insensitive.
- Only letters and digits are considered during palindrome checking.

### Reference

- https://leetcode.com/problems/valid-palindrome/

---

## December 12 - Add Digits

### Problem Statement

You are given a positive integer `num` representing a transaction ID.

To generate a verification digit, repeatedly calculate the sum of all digits of the number until the result contains only a single digit.

Return the final single-digit result.

### Input Format

- The first line contains an integer `num`.

### Output Format

Print the final single-digit sum.

### Sample Input 1

~~~
38
~~~

### Sample Output 1

~~~
2
~~~

### Sample Input 2

~~~
999
~~~

### Sample Output 2

~~~
9
~~~

### Explanation

In Sample 1:
- First iteration: `3 + 8 = 11`.
- Second iteration: `1 + 1 = 2`.
- Since `2` is a single-digit number, the process stops and the output is `2`.

In Sample 2:
- `9 + 9 + 9 = 27`.
- `2 + 7 = 9`.
- Therefore, the output is `9`.

### Constraints

- `0 ≤ num ≤ 2^31 - 1`
- The input is a non-negative integer.
- The process must continue until a single-digit number is obtained.

### Reference

- https://leetcode.com/problems/add-digits/

---

## December 13 - Cargo Balance Triples

### Problem Statement

A cargo bay holds `N` crates, each with a signed weight offset (positive = heavier than standard, negative = lighter). A **balanced triple** is three crates whose offsets sum to exactly `0`. Count the distinct balanced triples, where two triples are the same if they contain the same multiset of values. Crates with equal offsets are interchangeable.

### Input Format

- The first line contains `N`.
- The second line contains `N` integers, the crate offsets.

### Output Format

Print the number of distinct balanced triples.

### Sample Input 1

```
6
-1 0 1 2 -1 -4
```

### Sample Output 1

```
2
```

### Sample Input 2

```
3
0 1 1
```

### Sample Output 2

```
0
```

### Sample Input 3

```
4
0 0 0 0
```

### Sample Output 3

```
1
```

### Explanation

In sample 1, the distinct triples are `(-1, -1, 2)` and `(-1, 0, 1)`. In sample 2, no triple sums to zero. In sample 3, `(0, 0, 0)` counts once even though four crates can form it.

### Constraints

- `3 ≤ N ≤ 3000`.
- `-10^5 ≤ offset ≤ 10^5`.
- Expected time: `O(N^2)`; auxiliary space: `O(1)` beyond sorting.

### Reference

- [3Sum](https://leetcode.com/problems/3sum/)

---

## December 14 - Cipher Crate Sorting

### Problem Statement

Each of `N` crates is labelled with a lowercase word. Two crates belong to the same group if their labels are anagrams of each other, meaning one can be rearranged into the other. Report how many groups exist and the size of the largest group.

### Input Format

- The first line contains `N`.
- The second line contains `N` space-separated lowercase words.

### Output Format

Print the number of groups and the size of the largest group, separated by a space.

### Sample Input 1

```
6
eat tea tan ate nat bat
```

### Sample Output 1

```
3 3
```

### Sample Input 2

```
1
a
```

### Sample Output 2

```
1 1
```

### Sample Input 3

```
5
ab ba abc cab bca
```

### Sample Output 3

```
2 3
```

### Explanation

In sample 1, the groups are `{eat, tea, ate}`, `{tan, nat}`, and `{bat}`. Sample 2 has a single crate. In sample 3, `{ab, ba}` and `{abc, cab, bca}` form two groups.

### Constraints

- `1 ≤ N ≤ 10^4`.
- `1 ≤ |word| ≤ 100`.
- Words contain only lowercase English letters; duplicates are possible and count separately.

### Reference

- [Group Anagrams](https://leetcode.com/problems/group-anagrams/)

---

## December 15 - Crater Fields

### Problem Statement

A survey drone maps a region as an `m × n` grid. `1` marks a crater cell and `0` marks flat ground. Craters that touch up, down, left, or right belong to the same crater field. Diagonal contact does not connect cells. Find the number of crater fields and the area (cell count) of the largest one.

### Input Format

- The first line contains `m n`.
- The next `m` lines each contain `n` space-separated values, each `0` or `1`.

### Output Format

Print the number of crater fields and the largest area, separated by a space. Print `0 0` if there are no craters.

### Sample Input 1

```
4 5
1 1 0 0 0
1 1 0 0 0
0 0 1 0 0
0 0 0 1 1
```

### Sample Output 1

```
3 4
```

### Sample Input 2

```
2 2
1 0
0 1
```

### Sample Output 2

```
2 1
```

### Sample Input 3

```
1 3
0 0 0
```

### Sample Output 3

```
0 0
```

### Explanation

In sample 1, the fields have areas `4`, `1`, and `2`. In sample 2, the two craters touch only diagonally, so they are separate. Sample 3 has no craters.

### Constraints

- `1 ≤ m, n ≤ 300`.
- Each cell is `0` or `1`.
- Expected time: `O(mn)`.

### Reference

- [Number of Islands](https://leetcode.com/problems/number-of-islands/)

---

## December 16 - Fuel Cell Combinations

### Problem Statement

A rover is charged using fuel cells in `N` distinct capacities, with an unlimited supply of each. To reach a target charge of exactly `T`, find the fewest cells needed and the number of distinct combinations that reach `T`. Combinations are unordered, so `1 + 2` and `2 + 1` are the same.

### Input Format

- The first line contains `N T`.
- The second line contains `N` distinct positive integers, the capacities.

### Output Format

Print the minimum number of cells and the number of distinct combinations modulo `1,000,000,007`, separated by a space. Print `-1 0` if `T` cannot be reached.

### Sample Input 1

```
3 11
1 2 5
```

### Sample Output 1

```
3 11
```

### Sample Input 2

```
1 3
2
```

### Sample Output 2

```
-1 0
```

### Sample Input 3

```
3 10
1 5 10
```

### Sample Output 3

```
1 4
```

### Explanation

In sample 1, `5 + 5 + 1` uses three cells, and there are `11` unordered combinations in total. In sample 2, capacity `2` can never sum to `3`. In sample 3, a single `10` is optimal; the four combinations are `10`, `5 + 5`, `5 + 1×5`, and `1×10`.

### Constraints

- `1 ≤ N ≤ 12`.
- `0 ≤ T ≤ 10^4`.
- `1 ≤ capacity ≤ 10^4`.
- Expected time: `O(N · T)`.

### Reference

- [Coin Change](https://leetcode.com/problems/coin-change/)

---

## December 17 - Spore Spread

### Problem Statement

A greenhouse is an `m × n` grid. Each cell is `0` (empty), `1` (healthy plant), or `2` (infected plant). Every minute, each healthy plant that is directly up, down, left, or right of an infected plant becomes infected. Find the minimum number of minutes until no healthy plant remains, or report that it is impossible.

### Input Format

- The first line contains `m n`.
- The next `m` lines each contain `n` space-separated values from `{0, 1, 2}`.

### Output Format

Print the minimum number of minutes, or `-1` if some healthy plant can never be infected.

### Sample Input 1

```
3 3
2 1 1
1 1 0
0 1 1
```

### Sample Output 1

```
4
```

### Sample Input 2

```
3 3
2 1 1
0 1 1
1 0 1
```

### Sample Output 2

```
-1
```

### Sample Input 3

```
1 1
0
```

### Sample Output 3

```
0
```

### Explanation

In sample 1, the last plant is infected at minute `4`. In sample 2, the plant in the bottom-left corner is cut off by empty cells. In sample 3, there are no healthy plants, so `0` minutes are needed.

### Constraints

- `1 ≤ m, n ≤ 300`.
- Expected time: `O(mn)`.

### Reference

- [Rotting Oranges](https://leetcode.com/problems/rotting-oranges/)

---

## December 18 - Module Boot Order

### Problem Statement

A station controller has `N` modules numbered `0` to `N - 1`. Each dependency `a b` means module `a` must boot before module `b`. Among all valid boot orders, print the lexicographically smallest one (compare the sequences element by element). If the dependencies contain a cycle, no order exists.

### Input Format

- The first line contains `N M`.
- The next `M` lines each contain a dependency `a b`.

### Output Format

Print the `N` module numbers in boot order, separated by spaces, or `-1` if no valid order exists.

### Sample Input 1

```
4 4
1 0
2 0
3 1
3 2
```

### Sample Output 1

```
3 1 2 0
```

### Sample Input 2

```
2 2
0 1
1 0
```

### Sample Output 2

```
-1
```

### Sample Input 3

```
3 0
```

### Sample Output 3

```
0 1 2
```

### Explanation

In sample 1, module `3` must come before `1` and `2`, which must both come before `0`; the smaller choice `1` goes first. In sample 2, the two modules wait on each other. In sample 3, there are no dependencies, so the order is ascending.

### Constraints

- `1 ≤ N ≤ 10^5`; `0 ≤ M ≤ 2 × 10^5`.
- `0 ≤ a, b < N`; duplicate dependencies may appear.
- Expected time: `O((N + M) log N)`.

### Reference

- [Course Schedule II](https://leetcode.com/problems/course-schedule-ii/)

---

## December 19 - Telemetry Climb

### Problem Statement

A probe logs `N` sensor readings. A **climb** is a subsequence of readings, in original order, that is strictly increasing. Find the length of the longest climb and the number of distinct longest climbs. Climbs are distinguished by the indices they use, so equal values at different positions count separately.

### Input Format

- The first line contains `N`.
- The second line contains `N` integers, the readings.

### Output Format

Print the longest length and the number of longest climbs modulo `1,000,000,007`, separated by a space.

### Sample Input 1

```
5
1 3 5 4 7
```

### Sample Output 1

```
4 2
```

### Sample Input 2

```
5
2 2 2 2 2
```

### Sample Output 2

```
1 5
```

### Sample Input 3

```
3
5 4 3
```

### Sample Output 3

```
1 3
```

### Explanation

In sample 1, the longest climbs are `1 3 5 7` and `1 3 4 7`. In samples 2 and 3, no reading exceeds an earlier one, so every single reading is a climb of length `1`.

### Constraints

- `1 ≤ N ≤ 2000`.
- `-10^9 ≤ reading ≤ 10^9`.
- Expected time: `O(N^2)`.

### Reference

- [Number of Longest Increasing Subsequence](https://leetcode.com/problems/number-of-longest-increasing-subsequence/)

---

## December 20 - Maintenance Windows

### Problem Statement

A depot schedules `N` maintenance windows, each a closed integer interval `[l, r]` of hours. Two windows merge if they share at least one hour. Windows that are adjacent but share no hour, such as `[1, 2]` and `[3, 4]`, stay separate. After merging everything, report how many windows remain and the total number of distinct hours covered.

### Input Format

- The first line contains `N`.
- The next `N` lines each contain `l r`.

### Output Format

Print the number of merged windows and the number of distinct hours covered, separated by a space.

### Sample Input 1

```
4
1 3
2 6
8 10
15 18
```

### Sample Output 1

```
3 13
```

### Sample Input 2

```
2
1 4
4 5
```

### Sample Output 2

```
1 5
```

### Sample Input 3

```
2
1 2
3 4
```

### Sample Output 3

```
2 4
```

### Explanation

In sample 1, the merged windows are `[1, 6]`, `[8, 10]`, and `[15, 18]`, covering `6 + 3 + 4 = 13` hours. In sample 2, the windows share hour `4`. In sample 3, no hour is shared.

### Constraints

- `1 ≤ N ≤ 10^5`.
- `0 ≤ l ≤ r ≤ 10^9`.
- Input intervals are not sorted.
- Expected time: `O(N log N)`.

### Reference

- [Merge Intervals](https://leetcode.com/problems/merge-intervals/)

---

## December 21 - Fuel Flow Intervals

### Problem Statement

A pipeline sensor records the net fuel change `x[i]` for each of `N` consecutive minutes. Count the contiguous time intervals whose net change is exactly `K`. Intervals are counted by their start and end positions, so equal intervals at different positions count separately.

### Input Format

- The first line contains `N K`.
- The second line contains `N` integers, the per-minute net changes.

### Output Format

Print the number of contiguous intervals whose sum equals `K`.

### Sample Input 1

```
3 2
1 1 1
```

### Sample Output 1

```
2
```

### Sample Input 2

```
3 3
1 2 3
```

### Sample Output 2

```
2
```

### Sample Input 3

```
3 0
1 -1 0
```

### Sample Output 3

```
3
```

### Explanation

In sample 1, the intervals covering positions `0..1` and `1..2` each sum to `2`. In sample 2, positions `0..1` (`1 + 2`) and position `2` (`3`) each sum to `3`. In sample 3, the intervals `[1, -1]`, `[0]`, and `[1, -1, 0]` each sum to `0`.

### Constraints

- `1 ≤ N ≤ 2 × 10^5`.
- `-1000 ≤ x[i] ≤ 1000`; `-10^9 ≤ K ≤ 10^9`.
- The answer fits in a signed 64-bit integer.
- Expected time: `O(N)`.

### Reference

- [Subarray Sum Equals K](https://leetcode.com/problems/subarray-sum-equals-k/)

---

## December 22 - Median of Two Sorted Arrays

### Problem Statement

Given two integer arrays `nums1` and `nums2`, sorted in non-decreasing order, find the median of their combined elements. If the total length is even, the median is the average of the two middle elements. The solution must run in `O(log(m + n))` time.

### Input Format

- The first line contains `m n`, the lengths of the arrays.
- The next line contains `m` integers for `nums1`; omit it if `m = 0`.
- The next line contains `n` integers for `nums2`; omit it if `n = 0`.

### Output Format

Print the median to exactly five decimal places.

### Sample Input 1

```text
2 1
1 3
2
```

### Sample Output 1

```text
2.00000
```

### Sample Input 2

```text
2 2
1 2
3 4
```

### Sample Output 2

```text
2.50000
```

### Explanation

The combined sorted arrays are `[1, 2, 3]` and `[1, 2, 3, 4]`. Their medians are `2` and `(2 + 3) / 2 = 2.5`, respectively.

### Constraints

- `0 ≤ m, n ≤ 1000`; `1 ≤ m + n ≤ 2000`.
- `-10^6 ≤ nums1[i], nums2[i] ≤ 10^6`.
- Both arrays are sorted in non-decreasing order.
- Target auxiliary space: `O(1)`.

### Reference

- [Median of Two Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays/description/)

---

## December 23 - Unique Paths

### Problem Statement

Given an `m × n` grid, count the four-directional paths from the starting square to the ending square that visit every non-obstacle square exactly once. A move goes up, down, left, or right. A square cannot be revisited.

- `1`: starting square.
- `2`: ending square.
- `0`: empty square.
- `-1`: obstacle.

### Input Format

- The first line contains `m n`.
- The next `m` lines each contain `n` space-separated grid values.

### Output Format

Print the number of valid paths.

### Sample Input 1

```text
3 4
1 0 0 0
0 0 0 0
0 0 2 -1
```

### Sample Output 1

```text
2
```

### Sample Input 2

```text
3 4
1 0 0 0
0 0 0 0
0 0 0 2
```

### Sample Output 2

```text
4
```

### Sample Input 3

```text
2 2
0 1
2 0
```

### Sample Output 3

```text
0
```

### Explanation

In sample 1, exactly two routes cover all 11 non-obstacle cells before ending at `2`. In sample 2, there are four such routes. In sample 3, no route can cover every square exactly once and end at `2`.

### Constraints

- `1 ≤ m, n ≤ 20`; `1 ≤ m × n ≤ 20`.
- Each cell is `-1`, `0`, `1`, or `2`.
- There is exactly one starting square and one ending square.

### Reference

- [Unique Paths III](https://leetcode.com/problems/unique-paths-iii/description/)

---

## December 24 - Lunar Mining Colony: Dome Oxygen Containment

### Problem Statement

A lunar colony is represented by an `m × n` grid. `pressureMap[i][j]` is the height of the shielding structure at that cell. Gas settles in enclosed low areas and escapes through the boundary. Given an unlimited supply of gas, find the total volume the grid can retain. Boundary cells cannot retain gas.

### Input Format

- The first line contains `m n`.
- The next `m` lines contain `n` space-separated heights each.

### Output Format

Print the total trapped volume.

### Sample Input 1

```text
3 6
1 4 3 1 3 2
3 2 1 3 2 4
2 3 3 2 3 1
```

### Sample Output 1

```text
4
```

### Sample Input 2

```text
5 5
3 3 3 3 3
3 2 2 2 3
3 2 1 2 3
3 2 2 2 3
3 3 3 3 3
```

### Sample Output 2

```text
10
```

### Explanation

In sample 1, three interior cells retain `1`, `2`, and `1` units. In sample 2, the eight cells of height `2` each retain one unit, and the center retains two.

### Constraints

- `1 ≤ m, n ≤ 200`.
- `0 ≤ pressureMap[i][j] ≤ 2 × 10^4`.
- Expected time: `O(mn log(mn))`; space: `O(mn)`.

### Reference

- [Trapping Rain Water II](https://leetcode.com/problems/trapping-rain-water-ii/description/)

---

## December 25 - Reactor Rod — Squared Cutting Cost

### Problem Statement

A rod extends from coordinate `0` to `L`. Cut it once at each of `m` distinct specified positions, in any order. Cutting a current segment of length `d` costs `d²` energy. Each cut splits its current segment into two. Find the minimum total energy required.

### Input Format

- The first line contains `L m`.
- The second line contains the `m` distinct cut positions. Omit it when `m = 0`.

### Output Format

Print the minimum total energy as an integer.

### Sample Input 1

```text
7 2
2 4
```

### Sample Output 1

```text
65
```

### Sample Input 2

```text
5 1
1
```

### Sample Output 2

```text
25
```

### Sample Input 3

```text
10 0
```

### Sample Output 3

```text
0
```

### Explanation

In sample 1, cut at `4` first for `7² = 49`, then at `2` in the length-4 segment for `4² = 16`. The total is `65`. Sample 2 requires one cut; sample 3 requires none.

### Constraints

- `2 ≤ L ≤ 10^6`.
- `0 ≤ m ≤ min(100, L - 1)`.
- Cut positions are distinct integers strictly between `0` and `L`.
- Use 64-bit integers.

### Reference

- [Minimum Cost to Cut a Stick](https://leetcode.com/problems/minimum-cost-to-cut-a-stick/)

---

## December 26 - Alternating-Sensor Transformations

### Problem Statement

Each sensor code is a lowercase word of length `L`. Transform `start` into `target` by changing exactly one character per move. Every resulting code must be in the supplied dictionary. The position changed in each move must differ from the position changed in the immediately preceding move.

Find the minimum number of moves and the number of shortest valid sequences, modulo `1,000,000,007`. Different sequences of codes count separately. `start` may be absent from the dictionary; `target` must be present for a transformation to succeed. The two codes are distinct.

### Input Format

- The first line contains `start target`.
- The second line contains `N`.
- The next `N` lines each contain a distinct dictionary code.

### Output Format

Print the minimum number of moves and the number of shortest valid sequences, separated by a space. Print `-1 0` if no valid transformation exists.

### Sample Input 1

```text
hit cog
6
hot
dot
dog
lot
log
cog
```

### Sample Output 1

```text
4 2
```

### Sample Input 2

```text
aaa bba
2
baa
bba
```

### Sample Output 2

```text
2 1
```

### Sample Input 3

```text
aa cc
2
ba
cc
```

### Sample Output 3

```text
-1 0
```

### Explanation

Sample 1 has two shortest sequences: `hit → hot → dot → dog → cog` and `hit → hot → lot → log → cog`. In sample 2, the sequence is `aaa → baa → bba`. In sample 3, no valid sequence reaches `cc`.

### Constraints

- `1 ≤ L ≤ 10`; `1 ≤ N ≤ 5000`.
- All codes have length `L` and contain only lowercase English letters.
- Dictionary codes are distinct; `start` and `target` are distinct.

### Reference

- [Word Ladder II](https://leetcode.com/problems/word-ladder-ii/)

---

## December 27 - Checkpoint-Safe Storage Rectangle

### Problem Statement

A warehouse skyline has `N` adjacent bars. Bar `i` has height `h[i]` and positive width `w[i]`. Choose a nonempty consecutive range of entire bars that contains the zero-based checkpoint index `P`. A rectangle spanning the range has width equal to the sum of its bar widths and height at most the minimum bar height in the range. Find the maximum possible area. A height of zero is allowed.

### Input Format

- The first line contains `N P`.
- The second line contains `N` heights.
- The third line contains `N` widths.

### Output Format

Print the maximum area.

### Sample Input 1

```text
3 1
2 1 4
2 1 2
```

### Sample Output 1

```text
5
```

### Sample Input 2

```text
3 2
2 1 4
2 1 2
```

### Sample Output 2

```text
8
```

### Sample Input 3

```text
2 0
3 3
2 1
```

### Sample Output 3

```text
9
```

### Explanation

In sample 1, all bars span width `5` at height `1`. In sample 2, the last bar alone gives `4 × 2 = 8`. In sample 3, both bars give `3 × (2 + 1) = 9`.

### Constraints

- `1 ≤ N ≤ 200,000`; `0 ≤ P < N`.
- `0 ≤ h[i] ≤ 10^9`; `1 ≤ w[i] ≤ 10^4`.
- The answer fits in a signed 64-bit integer.

### Reference

- [Largest Rectangle in Histogram](https://leetcode.com/problems/largest-rectangle-in-histogram/)

---

## December 28 - Peak Window Baseline

### Problem Statement

A sensor records `N` integers. For each consecutive window of exactly `K` readings, sort its values and take the **lower median**, at zero-based position `floor((K - 1) / 2)`. Find the largest lower median and the smallest zero-based starting index of a window attaining it. Duplicate readings count separately.

### Input Format

- The first line contains `N K`.
- The second line contains `N` readings.

### Output Format

Print the maximum lower median and the earliest starting index, separated by a space.

### Sample Input 1

```text
8 3
1 3 -1 -3 5 3 6 7
```

### Sample Output 1

```text
6 5
```

### Sample Input 2

```text
3 2
2 2 2
```

### Sample Output 2

```text
2 0
```

### Sample Input 3

```text
4 2
5 1 4 2
```

### Sample Output 3

```text
2 2
```

### Explanation

In sample 1, the window beginning at index `5` is `[3, 6, 7]`, with median `6`. In sample 2 both windows have lower median `2`, so index `0` wins the tie. In sample 3 the lower medians are `1`, `1`, and `2`.

### Constraints

- `1 ≤ K ≤ N ≤ 200,000`.
- `-10^9 ≤ each reading ≤ 10^9`.

### Reference

- [Sliding Window Median](https://leetcode.com/problems/sliding-window-median/)

---

## December 29 - Bounded Palindrome Archive

### Problem Statement

Split a lowercase string `S` into nonempty contiguous palindromic segments, each of length at most `L`. Find the minimum number of segments and the number of partitions achieving that minimum. Partitions differ if their cut positions differ. Report the count modulo `1,000,000,007`.

### Input Format

- The first line contains `S`.
- The second line contains `L`.

### Output Format

Print the minimum segment count and the number of optimal partitions modulo `1,000,000,007`.

### Sample Input 1

```text
aab
2
```

### Sample Output 1

```text
2 1
```

### Sample Input 2

```text
abab
3
```

### Sample Output 2

```text
2 2
```

### Sample Input 3

```text
aba
2
```

### Sample Output 3

```text
3 1
```

### Explanation

The optimal partition in sample 1 is `aa | b`. In sample 2, the optimal partitions are `a | bab` and `aba | b`. In sample 3, `aba` exceeds the length limit, leaving `a | b | a`.

### Constraints

- `1 ≤ |S| ≤ 2000`; `1 ≤ L ≤ |S|`.
- `S` contains only lowercase English letters.

### Reference

- [Palindrome Partitioning II](https://leetcode.com/problems/palindrome-partitioning-ii/)

---

## December 30 - Maximum Path Sum in a Binary Tree

### Problem Statement

Given a binary tree with integer node values, find the maximum sum along any nonempty path. A path follows parent-child edges, cannot revisit a node, may start and end at any nodes, and need not pass through the root.

### Input Format

- The first line contains `N`, the number of tokens in the level-order representation, including missing-child markers.
- The second line contains `N` space-separated integers. `-1` denotes a missing child and cannot represent a node value. Starting with the root, each non-missing node consumes up to two subsequent tokens for its left and right children. Trailing missing children may be omitted.

### Output Format

Print the maximum path sum.

### Sample Input 1

```text
7
-10 9 20 -1 -1 15 7
```

### Sample Output 1

```text
42
```

### Sample Input 2

```text
5
-5 -2 -8 -1 -3
```

### Sample Output 2

```text
-2
```

### Explanation

In sample 1, the maximum path is `15 → 20 → 7`, with sum `42`. In sample 2, `-1` is a missing-child marker; the best path consists of the single node `-2`.

### Constraints

- `1 ≤ N ≤ 100,000`.
- Actual node values are between `-10,000` and `10,000`, excluding `-1`.
- The representation describes a valid tree with at least one actual node.
- The answer fits in a signed 32-bit integer.
- Expected time: `O(N)`; auxiliary space: `O(H)`, where `H` is the tree height.

### Reference

- [Binary Tree Maximum Path Sum](https://leetcode.com/problems/binary-tree-maximum-path-sum/)

---

## December 31 - Count All Possible Routes

### Problem Statement

You are given an array `locations` containing distinct positive integers, where `locations[i]` represents the position of city `i`. You are also given three integers: `start`, `finish`, and `fuel`, representing the starting city index, destination city index, and initially available fuel.

From any city `i`, you can travel directly to any other city `j`, provided `i` and `j` are different. The fuel required for the trip is the absolute difference between their positions: `|locations[i] - locations[j]|`.

A valid route is one in which the fuel never becomes negative. Cities can be visited multiple times, including the starting and destination cities.

Count all possible valid routes that start at `start` and end at `finish`. Return the result modulo `10⁹ + 7`.

### Input Format

- The first line contains an integer `n`, representing the number of cities.
- The second line contains `n` space-separated integers representing the `locations` array.
- The third line contains three space-separated integers: `start`, `finish`, and `fuel`.

### Output Format

Print a single integer representing the total number of valid routes modulo `1,000,000,007`.

### Sample Input 1

```text
5
2 3 6 8 4
1 3 5
```

### Sample Output 1

```text
4
```

### Sample Input 2

```text
3
4 3 1
1 0 6
```

### Sample Output 2

```text
5
```

### Sample Input 3

```text
3
5 2 1
0 2 3
```

### Sample Output 3

```text
0
```

### Explanation

In sample 1, the four valid routes are:

- `1 → 3`
- `1 → 2 → 3`
- `1 → 4 → 3`
- `1 → 4 → 2 → 3`

In sample 2, five valid routes exist, including routes that revisit cities.

In sample 3, no valid route exists because the minimum fuel required to reach city `2` is `4`, while only `3` units of fuel are available.

### Constraints

- `2 ≤ n ≤ 100`.
- `1 ≤ locations[i] ≤ 10⁹`.
- All values in `locations` are distinct.
- `0 ≤ start, finish < n`.
- `1 ≤ fuel ≤ 200`.
- The answer must be returned modulo `1,000,000,007`.

### Reference

- [Count All Possible Routes – LeetCode](https://leetcode.com/problems/count-all-possible-routes/)
- [Count All Possible Routes – TutorialsPoint](https://www.tutorialspoint.com/practice/count-all-possible-routes.htm)

---

## FAQ

#### Who can join the Challenge?

> Anyone who is passionate about coding and can dedicate a little time each day to the challenge over the next 31 days.

#### When should I submit the pull request?

> You don't need to submit a pull request every day. Submit it once you've completed all 31 algorithms.

#### What if I'm not able to code every day?

> Not a problem! While coding every day is nice, we understand that other commitments might get in the way.
>
> Plus, it's the holiday season! You don't have to solve one problem every day.
>
> Go at your own pace — one per day, seven a week, or even all 31 in a day!

#### What language should I use to code?

> Anything! New to GoLang? This is a great way to practise it.
>
> Want to find out what all the hype about Python is? Give it a try!
>
> Any and all programming languages are welcome.
>
> Maybe you could even try using a different language for every problem as a mini-challenge!

#### Fork? Pull request? What is all that? I don't know how to use GitHub!

> If you're new to Git or GitHub, check out this [GitHub guide](https://guides.github.com/activities/hello-world/) to get started.

#### How should I complete these programs?

> We have a folder for each day of the month. Simply complete your code and move the file into the corresponding folder.
>
> Be sure to rename your file using the following format:
>
> `username_problemname`
>
> **Example:** `exampleUser_probname.py`
>
> **Please do not modify any existing files in the repository.**

#### I forked the repository, but some problems were added only after that. How do I access those problems?

> Not to worry! Open your terminal or command prompt and navigate to your forked repository.
>
> Run the following commands:
>
> ```bash
> git remote add upstream https://github.com/SVCE-ACM/A-December-of-Algorithms-2026.git
> git fetch upstream
> git merge upstream/main
> ```
>
> These commands add a remote named `upstream` linked to the original repository, fetch its latest changes, and merge them into your local branch.
>
> **Note:** If you've already added the upstream repository, you don't need to add it again. Simply fetch and merge the latest changes.

#### I received a merge error. What do I do?

> This shouldn't happen unless you've modified existing files in the repository.
>
> If you encounter a merge conflict, the simplest approach is to:
> 1. Make a copy of your completed code outside the repository.
> 2. Clone the repository again.
> 3. Follow the steps in the previous answer to sync your fork.
> 4. Add your completed code to the appropriate folders.
>
> You can then proceed with your pull request.

#### I'm facing difficulties with or need help understanding a particular question.

> Open an [issue](https://github.com/SVCE-ACM/A-December-of-Algorithms-2026/issues) in this repository, and we'll do our best to help you out!

---

[**Back to Top ↑**](#a-december-of-algorithms-2026)
