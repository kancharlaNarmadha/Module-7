
# EX 7A POLYMORPHISM & EXCEPTION HANDLING
## DATE:
## AIM:
To write a java program to perform sum of two numbers and three numbers using Method Overloading(Compile time polymorphism)











## Algorithm

1.Create a class raj with two sum() methods: one taking two integers, another taking three integers.

2.The first sum() method returns the sum of two numbers, and the second one returns the sum of three numbers.

3.In the main() method, use Scanner to take three integer inputs from the user.

4.Create an object of the raj class to call both sum() methods.

5.Display the results of both method calls to show method overloading in action.




## Program:

Developed by: Kancharla Narmadha
Register Number: 212222110016
```

import java.util.*;
class Calculation{
  
 void sum(int a,int b)
  {
     System.out.println(a+b);
  }
  void sum(int a,int b,int c){
     System.out.println(a+b+c);
   }
  
}


public class HelloWorld{

     public static void main(String []args)
     {
       
  Calculation obj=new Calculation();
  Scanner sc=new Scanner(System.in);
  int a=sc.nextInt();
  int b=sc.nextInt();
  int c=sc.nextInt();
  obj.sum(a,b);
  obj.sum(a,b,c);
}
}


    
```

## Output:
![image](https://github.com/user-attachments/assets/edee8242-94bc-4d63-ade4-766d1fe90672)


## Result:
The program successfully demonstrates method overloading by defining multiple sum() methods with different parameter lists. The appropriate method is invoked based on the number of arguments passed.






