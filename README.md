# MAXofSUBarray
In this repository, We were exploring java programs and projects.


import java.util.*;
public class samp {
    public static void SUBBARRAY(int number[]){
        int Max= Integer.MIN_VALUE;
        int CURRENTval =0;
        for(int i=0;i<number.length;i++){
            int first=number[i];
            for(int j=i;j<number.length;j++){
                int last =number[j];
                 CURRENTval=0;
                for(int k=first;k<=last;k++){
                    CURRENTval += number[k];
                }
                System.out.println(CURRENTval);
                    if(Max<CURRENTval){
                        Max=CURRENTval;
                    }
                }
            }
       System.out.println("max sum ="+Max);
        }
   public static void main(String[] args) {
    int number[] = {2, 4, 6, 8, 10};
           SUBBARRAY(number);
   }
    }


