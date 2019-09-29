package Sorting;

import java.util.Arrays;

public class BubbleSortExample {
    public static void main(String[] args) {
        int[] arr = {5,1,4,2,8};
        int temp=0;
        for(int i=0; i<arr.length; i++){
            for(int j=1; j<(arr.length-1); j++){
                if(arr[j-1]>arr[j]){
                    temp= arr[j-1];
                    arr[j-1]=arr[j];
                    arr[j]=temp;
                }
            }
        }
        System.out.println(Arrays.toString(arr));

    }
}
