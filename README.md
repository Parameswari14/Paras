1. Pyramid Program
*
* *
* * *
* * * *
* * * * *
Let’s write the java code to understand this pattern better.

public class Edureka
{
public static void pyramidPattern(int n)
{
for (int i=0; i<n; i++) //outer loop for number of rows(n) { for (int j=n-i; j>1; j--) //inner loop for spaces
{
System.out.print(" "); //print space
}
for (int j=0; j<=i; j++ ) //inner loop for number of columns
{
System.out.print("* "); //print star
}

System.out.println(); //ending line after each row
}
}

public static void main(String args[]) //driver function
{
int n = 5;
pyramidPattern(n);
}
}

2. Right Triangle Star Pattern
*
* *
* * *
* * * *
* * * * *

public class Edureka
{
public static void rightTriangle(int n)
{
int i, j;
for(i=0; i<n; i++) //outer loop for number of rows(n) { for(j=2*(n-i); j>=0; j--) // inner loop for spaces
{
System.out.print(" "); // printing space
}
for(j=0; j<=i; j++) // inner loop for columns
{
System.out.print("* "); // print star
}
System.out.println(); // ending line after each row
}
}
public static void main(String args[])
{
int n = 5;
rightTriangle(n);
}
}
3. Left Triangle Star Pattern

*
* *
* * *
* * * *
* * * * *
public class Edureka
{
public static void printStars(int n)
{
int i, j;
for(i=0; i<n; i++) //outer loop for number of rows(n) { for(j=2*(n-i); j>=0; j--) // inner loop for spaces
{
System.out.print(" "); // printing space
}
for(j=0; j<=i; j++) // inner loop for columns
{
System.out.print("* "); // print star
}
System.out.println(); // ending line after each row
}
}
public static void main(String args[])
{
int n = 5;
printStars(n);
}

3. Left Triangle Star Pattern

*
* *
* * *
* * * *
* * * * *
public class Edureka
{
public static void printStars(int n)
{
int i, j;
for(i=0; i<n; i++) //outer loop for number of rows(n) { for(j=2*(n-i); j>=0; j--) // inner loop for spaces
{
System.out.print(" "); // printing space
}
for(j=0; j<=i; j++) // inner loop for columns
{
System.out.print("* "); // print star
}
System.out.println(); // ending line after each row
}
}
public static void main(String args[])
{
int n = 5;
printStars(n);
}
}

4. Diamond Shape Pattern Program in Java
Enter the number of rows: 5

*
***
*****
*******
*********
*******
*****
***
*

import java.util.Scanner;
public class Edureka
{
public static void main(String args[])
{
int n, i, j, space = 1;
System.out.print("Enter the number of rows: ");
Scanner s = new Scanner(System.in);
n = s.nextInt();
space = n - 1;
for (j = 1; j<= n; j++)
{
for (i = 1; i<= space; i++)
{
System.out.print(" ");
}
space--;
for (i = 1; i <= 2 * j - 1; i++)
{
System.out.print("*");
}
System.out.println("");
}
space = 1;
for (j = 1; j<= n - 1; j++)
{
for (i = 1; i<= space; i++)
{
System.out.print(" ");
}
space++;
for (i = 1; i<= 2 * (n - j) - 1; i++)
{
System.out.print("*");
}
System.out.println("");
}
}
}

5. Downward Triangle Star Pattern
Enter the number of rows: 5

* * * * *
* * * *
* * *
* *
*

import java.util.Scanner;
public class Edureka
{
public static void main(String[] args)
{
Scanner sc = new Scanner(System.in);

System.out.println("Enter the number of rows: "); //takes input from user

int rows = sc.nextInt();

for (int i= rows-1; i>=0 ; i--)
{
for (int j=0; j<=i; j++)
{
System.out.print("*" + " ");
}
System.out.println();
}
sc.close();
}
}

6. Mirrored Right Triangle Star Program
Enter the number of rows: 5

*
**
***
****
*****
******

import java.util.Scanner;
public class Edureka
{
public static void main(String[] args)
{
Scanner sc = new Scanner(System.in);

System.out.println("Enter number of rows: "); // takes input from user

int rows = sc.nextInt();

for (int i= 0; i<= rows; i++)
{
for (int j=1; j<=rows-i; j++)
{
System.out.print(" ");
}
for (int k=0;k<=i;k++)
{
System.out.print("*");
}
System.out.println("");
}
sc.close();

}
}

7. Reversed Pyramid Star Pattern
Enter the number of rows: 5

* * * * *
* * * *
* * *
* *
*
import java.util.Scanner;
public class Edureka
{
public static void main(String[] args)
{
Scanner sc = new Scanner(System.in);
System.out.println("Enter the number of rows: ");

int rows = sc.nextInt();
for (int i= 0; i<= rows-1 ; i++)
{
for (int j=0; j<=i; j++)
{
System.out.print(" ");
}
for (int k=0; k<=rows-1-i; k++)
{
System.out.print("*" + " ");
}
System.out.println();
}
sc.close();

}
}

8. Right down Mirror Star Pattern
Enter the number of rows: 5

*****
****
***
**
*

import java.util.Scanner;
public class Edureka
{

public static void main(String[] args)
{
Scanner sc = new Scanner(System.in); // takes input
System.out.println("Enter number of rows: ");
int rows = sc.nextInt();
for (int i= rows; i>= 1; i--)
{
for (int j=rows; j>i;j--)
{
System.out.print(" ");
}
for (int k=1;k<=i;k++)
{
System.out.print("*");
}
System.out.println("");
}
sc.close();
}
}
 

9. Right Pascal’s Triangle
Enter the number of rows: 5

*
* *
* * *
* * * *
* * * * *
* * * *
* * *
* *
*
 


import java.util.Scanner;
public class Edureka
{
public static void main(String[] args)
{
Scanner sc = new Scanner(System.in);
System.out.println("Enter the number of rows: ");

int rows = sc.nextInt();
for (int i= 0; i<= rows-1 ; i++)
{
for (int j=0; j<=i; j++) { System.out.print("*"+ " "); } System.out.println(""); } for (int i=rows-1; i>=0; i--)
{
for(int j=0; j <= i-1;j++)
{
System.out.print("*"+ " ");
}
System.out.println("");
}
sc.close();
}
}

10. Left  Triangle Pascal’s
Enter the number of rows: 5

*
**
***
****
*****
****
***
**
*
import java.util.Scanner;
public class Edureka
{

public static void main(String[] args)
{
Scanner sc = new Scanner(System.in);
System.out.println("Enter the number of rows: ");

int rows = sc.nextInt();
for (int i= 1; i<= rows ; i++)
{
for (int j=i; j <rows ;j++)
{
System.out.print(" ");
}
for (int k=1; k<=i;k++) { System.out.print("*"); } System.out.println(""); } for (int i=rows; i>=1; i--)
{
for(int j=i; j<=rows;j++)
{
System.out.print(" ");
}
for(int k=1; k<i ;k++)
{
System.out.print("*");
}
System.out.println("");

}
sc.close();
}
}
