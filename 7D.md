
# EX 7D SYNCHRONIZATION
## DATE:
## AIM:
To write a Java Program to perform multiplication table  for 5 & 7 using Synchronization block for the below Scenario

1. Create a Class Table with void printTable method in that perform multiplication table

Note :Assume Sleep as 400 ms  i.e Thread.Sleep(400)









## Algorithm


1.Create a class Table that contains a static method printTable(int n) to print the multiplication table for a given number.

2.Use static synchronized keyword to make the method thread-safe so only one thread accesses it at a time.

3.Inside the method, use a loop to print the table from 1 to 10 for the given number.

4.Add a delay using Thread.sleep(400) after printing each line to simulate thread activity.

5.Surround Thread.sleep() with try-catch block to handle any InterruptedException that may occur during sleep.




## Program:

Developed by: Kancharla Narmadha
Register Number: 212222110016
```


class Table{
    static synchronized void printTable(int n){
        for(int i=1;i<=10;i++){
            System.out.println("Multiplication Table for "+n+"*"+i+" :"+(n*i));
        }
        try{
            Thread.sleep(400);
        }
        catch(Exception e){
            System.out.println(e);
        }
    }
}

    
```

## Output:
![image](https://github.com/user-attachments/assets/4fdd7b53-3bab-4253-a800-047af8af9b1a)


## Result:
The method prints a multiplication table from 1 to 10 for the given input number, and is synchronized to prevent concurrent access by multiple threads.









