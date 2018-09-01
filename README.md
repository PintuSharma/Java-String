# Java-String
Given a string, s , matching the regular expression [A-Za-z !,?._'@]+, split the string into tokens.

Given a string, , matching the regular expression [A-Za-z !,?._'@]+, split the string into tokens. We define a token to be one or more consecutive English alphabetic letters. Then, print the number of tokens, followed by each token on a new line.
Note: You may find the String.split method helpful in completing this challenge.

Input Format
A single string, s

s is composed of any of the following: English alphabetic letters, blank spaces, exclamation points (!), commas (,), question marks (?), periods (.), underscores (_), apostrophes ('), and at symbols (@).



Solution

import java.io.*;
import java.util.*;

public class Solution {

    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        String s = scan.nextLine();
        s=s.trim();
        if(s.length()>0)
        {
        String [] a=s.split("[ !,?._'@]+");
       System.out.println(a.length);
        for(String retval : a)
        System.out.println(retval);
        }
        else
            System.out.println("0");
        
        // Write your code here.
        scan.close();
    }
}
