# Count-Items-Matching-a-Rule
#Array Leetcode problem solution
class Solution {
    public int countMatches(List<List<String>> items, String ruleKey, String ruleValue) {
        int count=0;
        int key=0;
        if(ruleKey.equals("color"))
            key=1;
        if(ruleKey.equals("name"))
            key=2;
        for(List<String> item:items)
        {
            if(item.get(key).equals(ruleValue))
                count=count+1;
        }
        return count;
    }
}
