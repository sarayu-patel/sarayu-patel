import java.util.*;
public class Main{
    public static void main(String[]args){
        int arr[]={8,2,5,9,11};
        for(int i=0;i<arr.length-1;i++){
            for(int j=0;j<arr.length-i-1;j++){
//for swaping the values  after checking the condition:
                if(arr[j]>arr[j+1]){
                    int temp=arr[j];
                    arr[j]=arr[j+1];
                    arr[j+1]=temp;
                }
            }
        }
        System.out.println("after sorting");
        for(int elements:arr){
            System.out.print(elements + " ");
        }
    }
}
