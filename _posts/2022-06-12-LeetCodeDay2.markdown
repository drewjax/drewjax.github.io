---
layout: post
title:  "LeetCode day 2"
date:   2022-06-12 16:16:26 -0400
---

Today (and a little of last night) I continued my journey into practicing for my technical interviews. I continued in the Array and Hashing category, in hopes to get proficient with what I may need to do. I did 2 problems, Group Anagrams and returning the Kth most frequent integers in an Array. 

Group Anagrams was not too difficult, as the previous problem I did dealt with anagrams. Essentially I took what I did in the previous problem, and did it in a larger scale. I sorted all the strings (as in "tea" would be "aet") in the list I was given and then used a nested for loop to create "sub arrays" keeping the indexed from the original input and the sorted array. I would then append this new sub array into a new array which would be the answer. I used something I called a blackMark, which would keep track of the indexed that I already used so I would not get repeats of sub arrays.
[Group-Anagrams][groupanagrams]

Finding the Kth most frequent integers in an array was a bit more difficult. I was expected to do this in O(n log n) time,
which made it bit more difficult. At first I was a little troubled with the wording of the question, but at the end I understood that it more or less wanted an ascending list of the integers with the most frequency. I tried a few approached, using a dictionary where I would have the integer and the count/frequency as its value pair. Which ended up being right, but I tried to do something weird where I would try to sort the dictionary but I was unsuccessful. I ended up using the solution in part to solve my answer. I was close with the dictionary, but I needed a large array and then would append each unique number into a new array, and when it reaches the desired K length, it would return. 
[Kth-Element][kelement]

As I will continue to document my leetcode, and post the solution here and on Github, I want to also continue with jotting notes down about side projects I want to do. I want to create an app in which will track live scores of my annual golf tournament. The tournament is really for fun, but I think it would be cool to see how you compare to your opponents in real time. This would be a big challenge for me, but also a great learning experience, and something that would be useful and cool to use for the future of the tournament.


[groupanagrams]: https://github.com/drewjax/Leetcode/blob/main/ArrayandHashing/GroupAnagram.py
[kelement]: https://github.com/drewjax/Leetcode/blob/main/ArrayandHashing/KElements.py
