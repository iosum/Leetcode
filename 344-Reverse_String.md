Write a function that reverses a string. The input string is given as an array of characters char[].

Do not allocate extra space for another array, you must do this by modifying the input array in-place with O(1) extra memory.

You may assume all the characters consist of printable ascii characters.

 
```
Example 1:

Input: ["h","e","l","l","o"]
Output: ["o","l","l","e","h"]

Example 2:

Input: ["H","a","n","n","a","h"]
Output: ["h","a","n","n","a","H"]
```

```c++
class Solution {
public:
    void reverseString(vector<char>& s) {
        int left = 0;
        int right = (int)s.size() -1;
        while(left < right) {
            swap(s[left++], s[right--]);
        }
    }
};
```



```c++
class Solution {
public:
    void reverseString(vector<char>& s) {
        int left = 0;
        int right = (int)s.size() -1;
        cout<<right;
        while(left<right){
             cout<<s[left];
            cout<<s[right];
                       swap(s[left++], s[right--]);
            cout<<s[left];
            cout<<s[right];
        }
 
        
    }
};

```


````
Your input
["a","b","c","d","e"]
stdout
4aebdbdcc
Output
["e","d","c","b","a"]
Expected
["e","d","c","b","a"]

```