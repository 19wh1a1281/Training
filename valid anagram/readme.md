class Solution {
public:
    bool isAnagram(string s, string t) {
        int nums = s.size();
        int nums1 = t.size();
        int i;
        map<char,int>mp;
        if(nums!=nums1)
        {
            return false;
        }
        else
        {
            for(i=0;i<nums;i++)
            {
                s[i]=tolower(s[i]);
                mp[s[i]]++;
            }
            for(i=0;i<nums1;i++)
            {
                t[i]=tolower(t[i]);
                    mp[t[i]]--;
                if(mp[t[i]]<0)
                {
                    return false;
                break;
            }
                if(mp[t[i]]==0)
                {
                    mp.erase(t[i]);
                }
                
            }
        }
            if(mp.size()==0)
                return true;
            return false;
        
    }
};
