package com.cafeform.algorithm;

import java.util.Date;

/**
 *
 * @author kaizawa
 */
public class Fact1 {

    public static void main(String[] args) {
        long input = 10;
        new Fact1().doByLoop(input);
        new Fact1().doByRecursive(input);
    }
    
    private void doByLoop(long input){
        long start = new Date().getTime();
        long ans = 1;
        for(long i = input ; i > 0  ; i--)
        {
            ans = ans * i;
        }
        long end = new Date().getTime();
        System.out.println("By Loop: " + ans + " took " + (end - start) + "ms");
       
    }
    
    private void doByRecursive(long input){
        long start = new Date().getTime();        
        long ans = doFact(input);
        long end = new Date().getTime();        
        System.out.println("By Recursive: " + ans + " took " + (end - start) + "ms");        
    }
    
    private long doFact(long input){
        if(0 == input){
            return 1;
        }
        return input * doFact(input -1);
    }
}
