class Solution {
public:
    bool isPalindrome(int x) {
         long long int t,r,s=0;
        t = x;
        while(x > 0)
        {
            r = x%10;
            s = s*10+r;
            x= x/10;
        }
        if(s==t)
            return true;
    
        return false;
    }
};
