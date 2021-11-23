class Solution {
public:
    string longestCommonPrefix(vector<string>& strs) {
        string prefix="";
        int i,j;
        for(i=0;i<strs[0].size();i++)
        {
            for(j=1;j<strs.size();j++)
            {
                if(strs[j][i]!=strs[0][i])
                    return prefix;
            }
            prefix = prefix+strs[0][i];
        }
        return prefix;
        
    }
};
        
    
