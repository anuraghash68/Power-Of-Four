# Power-Of-Four
# August leetcode week 1 solution

// Code in JAVA
class Solution {
    public boolean isPowerOfFour(int num) {
        if((num > 0) && (num & (num-1)) == 0 && (num & 0xaaaaaaaa)==0)//second condition for checking 1 set bit and 3rd condition for taking AND with power of 
            return true;                                              //2 and power of given number is zero or not? if given number is power of 4 then,AND will be 0 
        else return false;
    }
}

// Code in C


bool isPowerOfFour(int num){
if((num > 0) && (num & (num-1)) == 0 && num%3==1) return true;
else return false;
}
