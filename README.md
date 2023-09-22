# MergeStringAlternatively
Merging the two String alternately
this is the leet code question from 75 question
class Solution {
    public String mergeAlternately(String word1, String word2) {
     StringBuilder result = new StringBuilder();

        String w1= word1.toLowerCase();
        String w2= word2.toLowerCase();
        for (int i=0;i<w1.length() || i<w2.length(); i++){
            if(i< w1.length()){
            result.append(w1.charAt(i));
            }
            if(i<w2.length()){
                result.append(w2.charAt(i));
                }
        }
        return result.toString();
    }
}
