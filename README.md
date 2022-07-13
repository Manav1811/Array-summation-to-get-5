# Array-summation-to-get-5

import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        int a[]=new int[3];
        int b[]=new int[3];
        Scanner s=new Scanner(System.in);
        int c[]=new int[6];
        
        System.out.println("Enter first array:");
        
        for(int i=0;i<3;i++)
        {
            a[i]=s.nextInt();
        }
       
        System.out.println("Enter second array:");
       
        for(int i=0;i<3;i++)
        {
            b[i]=s.nextInt();
        }
        
        int k=0;
        for(int i=0;i<3;i++)
        {
            for(int j=0;j<3;j++)
            {
                if(a[i]+b[j]==5)
                {
                    c[k]=a[i];
                    k+=1;
                    c[k]=b[i];
                }
            }
        }
        
        System.out.println("Your array for summation 5 is :");
        for(int i=0;i<k;i++)
        {
            System.out.print(c[i]);
        }
    }
}
