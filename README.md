import java.util.*;
import java.lang.*;
import java.io.*;

public class Main
{
	public static void main (String[] args) throws java.lang.Exception
	{
		//your code here
                Scanner sc=new Scanner(System.in);
                int n=sc.nextInt();
                int arr[]=new int[n];
                for(int i=0;i<n;i++){
                        arr[i]=sc.nextInt();
                }
                int max=0;
                int res=0;
                for(int i=0;i<n;i++){
                        if(arr[i]==0){
                                max=0;
                        }
                        else{
                                max++;
                                res=Math.max(res, max);
                        }
                }
                System.out.println(res);
	}
}
