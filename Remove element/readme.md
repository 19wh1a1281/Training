class Solution {
public:
    int removeElement(vector<int>& nums, int val) {
         int n=nums.size();
        int count = 0,i;
        for (int n:nums) {
            if (n!= val) {
                nums[count]=n;
                
                count++;
            }
        }
        return count;
        
    }
};
