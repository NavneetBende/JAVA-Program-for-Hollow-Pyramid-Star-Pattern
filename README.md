Printing Hollow Pyramid Star Pattern
In this JAVA program we’re going to code hollow pyramid star pattern program .

The logic of this program is this take any number input from user and store it in variable n and then run the for loop start from i=1 to i<=n and inside the outer for loop take another for loop for (j = i; j < n; j++) to print spaces .

After this run a while loop (k!=(2*i-1)) and inside while loop take if k==0 or k==2*i-2 then print line changement statement and then print star statement.

Hollow Pyramid Star Pattern
Algorithm:
Enter the number from the user and store it in any variable.(‘n‘ in this case).
Run a loop ‘n’ number of times to iterate through each of the rows. From i=0 to i<=n. The loop should be structured as for (i = 1; i <= n; i++)
 Run a nested loop inside the main loop to print the spaces before the pyramid. From j=i to j<n The loop should be structured as for (j = i; j < n; j++)
Inside this nested loop print white space System.out.println(” “).
Run a while loop in condition while (k != (2 * i – 1))
Inside while loop take if k==0 or k==2*i-2 and print System.out.print(“*”); 
Inside main loop move to the next line by printing a new line . System.out.println();
Take for (i = 0; i < 2 * n – 1; i++) to print last line System.out.print(“*”);
Code in Java:
import java.util.Scanner;
public class Pattern1 {

	public static void main(String[] args) {
		int i, j, k = 0; 
		Scanner sc = new Scanner(System.in);
		System.out.println("Enter number");
                int n=sc.nextInt();
        for (i = 1; i <= n; i++)  
        { 
            
            for (j = i; j < n; j++)  
                System.out.print(" "); 
            while (k != (2 * i - 1)) { 
                if (k == 0 || k == 2 * i - 2) 
                    System.out.print("*"); 
                else
                    System.out.print(" "); 
                k++; 
                ; 
            } 
            k = 0; 
            System.out.println();  
        } 
        // print last row 
        for (i = 0; i < 2 * n - 1; i++)  
            System.out.print("*"); 
        
    } 
}
