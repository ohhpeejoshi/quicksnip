---
title: Check Palindrome
description: Checks if a given string is a palindrome.
author: ohhpeejoshi
tags: cpp,string,palindrome,utility
---

```cpp
#include <string>

bool isPalindrome(const std::string& str) {
    int left = 0;
    int right = str.length() - 1;
    
    // Compare characters from both ends towards the center
    while (left < right) {
        if (str[left] != str[right]) {
            return false; // Not a palindrome
        }
        left++;
        right--;
    }
    return true; // The string is a palindrome
}
```