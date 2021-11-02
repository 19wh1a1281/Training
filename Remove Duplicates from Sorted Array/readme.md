Remove Duplicates from Sorted Array

class Solution {

public:

    int removeDuplicates(vector<int>& nums) {
    
        return std::unique((nums.begin()),(nums.end()))-nums.begin() ;
        
    }
    
};
