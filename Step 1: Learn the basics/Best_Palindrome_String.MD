# Must Use paindrome way
### https://practice.geeksforgeeks.org/problems/palindrome-string0817/1

         int isPalindrome(String S) {

               int n = S.length()-1;

               for(int i=0;i<S.length()/2;i++){
                   if(S.charAt(i)!=S.charAt(n-i)) return 0;
               }

               return 1;
            }
            
# https://leetcode.com/problems/valid-palindrome/submissions/

    static  boolean isPalindrome(String s) {
           
             s = s.toLowerCase();
             StringBuilder b = new StringBuilder();
             
             for(int i=0;i<s.length();i++){
                 if(Character.isDigit(s.charAt(i)) || Character.isLetter(s.charAt(i))){  //Include if char is Letter / Digit
                     b.append(s.charAt(i));
                 }
             }
             
             int n = b.length()-1;
             for(int i=0;i<b.length()/2;i++){
                 if(b.charAt(i)!=b.charAt(n-i)) return false;
                 
                 
             }
             
             return true;
     }
