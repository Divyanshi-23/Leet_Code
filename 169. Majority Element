import java.util.*;
class Solution {
    public int majorityElement(int[] nums) {
        int k = nums.length;
        int ncount = 0;
        int count = 0;
        int ans = 0;
        int val = 0;
        HashSet<Integer> hs = new HashSet<>();
        for(int i=0;i<k/2;i++){
            hs.add(nums[i]);
        }
        if(hs.size()==1){
            return nums[0];
        }
        for(int i=0;i<k;i++){
            val = nums[i];
            for(int j=0;j<k;j++){
                if(val==nums[j]){
                    ncount++;
                }
            }
            if(ncount>count){
                count = ncount;
                ans = val;
            }
            ncount = 0;
        }
        return ans;
    }
}
