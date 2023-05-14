# Java-program-to-find-number-of-days-in-a-month

## PROGRAM:
```
import java.util.Scanner;
public class DaysInMonth{
    public static void main(String[] args){
        Scanner sc= new Scanner(System.in);
        System.out.print("Enter the month in number:");
        int month=sc.nextInt();
        System.out.print("Enter the year:");
        int year=sc.nextInt();
        switch(month)
        {
            case 1:
            case 3:
            case 5:
            case 7:
            case 8:
            case 10:
            case 12:
                System.out.print("\nThis month has 31 days.");
                break;
            case 4:
            case 6:
            case 9:
            case 11:
                System.out.print("\nThis month has 30 days.");
                break;
            case 2:
                if(year%4==0)
                {
                    System.out.print("\nThis month has 29 days.");
                }
                else
                {
                    System.out.print("\nThis month has 28 days.");
                }
                break;
            default:
                System.out.print("Enter a valid number of the month.");
        }
    }
}
```

## OUTPUT:
```
C:\Users\Dell\.jdks\openjdk-19.0.2\bin\java.exe "-javaagent:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2022.3.3\lib\idea_rt.jar=8156:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2022.3.3\bin" -Dfile.encoding=UTF-8 -Dsun.stdout.encoding=UTF-8 -Dsun.stderr.encoding=UTF-8 -classpath "C:\Users\Dell\IdeaProjects\Java 1\out\production\Java 1" DaysInMonth
Enter the month in number:12
Enter the year:2004

This month has 31 days.
```
Process finished with exit code 0
