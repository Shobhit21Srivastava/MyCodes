/* package codechef; // don't place package name! */

import java.util.*;
import java.lang.*;
import java.io.*;

/* Name of the class has to be "Main" only if the class is public. */
class Codechef
{
	public static void main (String[] args) throws java.lang.Exception
	{
	 Scanner sc=new Scanner(System.in);
	 int k=sc.nextInt();
	 int size=sc.nextInt();
	 int arr[]=new int[size];
	 int result[]=new int[size];
	 for(int i=0;i<size;i++)
	 {
	     arr[i]=sc.nextInt();
	 }
	 if(k>size)
	 {
	     k=k%size;
	 }
	 for(int i=0;i<k;i++)
	 {
	     result[i]=arr[size-k+i];
	 }
	 int j=0;
	 for(int i=k;i<size;i++)
	 {
	     result[i]=arr[j];
	     j++;
	 }
	 for(int i=0;i<size;i++)
	 {
	  System.out.print(result[i]);   
	 }
	 
	 
	}
}
