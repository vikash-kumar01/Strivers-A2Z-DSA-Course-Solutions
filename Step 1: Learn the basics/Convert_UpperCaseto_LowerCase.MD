# Convert UpperCase to LowerCase

     for(int i =0;i<ans.length();i++){
        char ch = ans.charAt(i);

        if (ch>='A'  && ch<='Z'){
            temp += (char)((int)(ch+32));
        }
        else
            temp += ans.charAt(i);
        }


### Remove non-Alphanumeric Characters from string 
    
    String ans =s.replaceAll("[^A-Za-z0-9]", "");
