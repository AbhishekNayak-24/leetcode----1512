# leetcode----1512
Number of Good pairs
//code in c++
class Solution {
 public:
  int numIdenticalPairs(vector<int>& nums) {
    int ans = 0;
    vector<int> count(101);

    for (const int num : nums)
      ans += count[num]++;

    return ans;
  }
};
