

```java
    public static void main(String a[])
    {
        int num1 = 3;
        int num2 = 5;
        int result = num1 + num2;
        System.out.print(result);
    }
```
<br>



```java
        float f = 5.6f;
        int t = (int) f;
        System.out.print(t);
        //5
```
<br>


```java
        int n = 3;

        switch (n) {
            case 1:
                System.out.println("monday");
                break;
            case 2:
                System.out.println("tuesday");   
                break;
            case 3:
                System.out.println("wednesday");
                break;
            default:
                System.out.println("Enter a valid numbah");                
        }
        //wednesday
```
<br>

cara baru tulis switch statement
```java
        String day = "sunday";

        switch(day)
        {
            case "saturday", "sunday" -> System.out.println("6am");
            case "moday" -> System.out.println("8am");
            default -> System.out.println("7am");
        }
        //6am
```

```java
        String day = "sunday";
        String result = "";

        switch(day)
        {
            case "saturday", "sunday" -> result = "6am";
            case "moday" -> result = "8am";
            default -> result = "7am";           
        }                 

        System.out.println(result);
        //6am
```

```java
        String day = "sunday";
        String result = "";

        result = switch(day)
        {
            case "saturday", "sunday" -> "6am";
            case "moday" -> "8am";
            default -> "7am";           
        };                 

        System.out.println(result);
        //6am
```
<br>

while
```java
        int i = 1;

        while (i<=2) {
            System.out.println("Hi " + i);
            i++;
        }

        System.out.println("Bye " + i);
        //Hi 1
        //Hi 2
        //Bye 3
```
<br>

do while  
kita tetap nak run code tu even condition false
```java
    {
        int i = 5;

        do {
            System.out.println("Hi " + i);
            i++;
        } while (i<=4);
    }
    //Hi 5
```
<br>

5 hari 9am-5pm
```java
        for(int i=1; i<=5; i++)
        {
            System.out.println("Day " + i);

            for(int j=1; j<=9; j++)
            {
                System.out.println("  " + (j+8) + "-" +(j+9));
            }
        }
```
<br>

**object**.    
create object calc    
calc boleh pakai methods dlm class Calculator  


```java
class Calculator
{
    public int add(int num1, int num2)
    {
        int result = num1 + num2;
        return result;
    }
}


class Demo
{
    public static void main(String a[])
    {
        int num1=4;
        int num2=5;

        Calculator calc = new Calculator();

        int result = calc.add(num1,num2);

        System.out.println(result);

    }
}
//9
```
<br>

method wajib ada data type if return something  
kalu void baru x yah buh data type sebab void = x return something
```java
    public int add( int num1, int num2)
    {
        int result = num1 + num2;
        return result;
    }
```
<br>

`method overloading`  
method nama sama.   
bil parameter beza.  
if bil parameter sama, datatype wajib beza  (entah ler yg ni aku test jadi error)
```java
class Calculator
{
    public int add( int num1, int num2, int num3)
    {  
        return num1 + num2 + num3;
    }
    public int add( int num1, int num2)
    {
        return num1 + num2;
    }
    
}

class Demo
{
    public static void main(String a[])
    {
        int num1 = 2;
        int num2 = 2;
        int num3 = 2;

        Calculator calc = new Calculator();

        int result1 = calc.add(num1, num2, num3);
        int result2 = calc.add(num1, num2);

        System.out.println(result1);
        System.out.println(result2);
    }
}
//6
//4
```
<br>

array
```java
    public static void main(String a[])
    {
        int nums[] = {3,7,2};
        nums[1] = 6;

        for (int i = 0; i < 3; i++) {
            System.out.println(nums[i]);
        }
    }
//3
//6
//2
```

```java
    public static void main(String a[])
    {
        int nums[] = new int[4];
        nums[0] = 3;
        nums[1] = 6;
        nums[2] = 2;

        for (int i = 0; i < 3; i++) {
            System.out.println(nums[i]);
        }
    }
//3
//6
//2
```
multi dimensional array

```java
int[][] nombors = { {1, 2, 3, 4}, {5, 6, 7} };
System.out.println(nombors[1][2]);
//7
```

```java
        int nums[][] = new int[3][4];

        for (int i = 0; i < 3; i++) {
            for (int j = 0; j < 4; j++) {
                nums[i][j] = (int) (Math.random() * 10);
            }
        }

        for (int i = 0; i < 3; i++) {
            for (int j = 0; j < 4; j++) {
                System.out.print(nums[i][j] + " ");
            }
            System.out.println();
        }
//4 2 7 2
//0 0 2 7
//9 3 4 1
```
<br>

Array of objects

```java
class Student
{
    String name;
    int marks;
}

class Demo
{
    public static void main(String a[])
    {
        Student s1 = new Student();
        s1.name = "abu";
        s1.marks = 78;

        Student s2 = new Student();
        s2.name = "ali";
        s2.marks = 88;

        Student students[] = new Student[2];
        students[0] = s1;
        students[1] = s2;

        for (int i = 0; i < students.length; i++) {
            System.out.println(students[i].name + " : " + students[i].marks);
        }
    }
}
//abu : 78
//ali : 88
```
<br>

Enhanced for loop (macam foreach)

```java
class Student
{
    String name;
    int marks;
}

class Demo
{
    public static void main(String a[])
    {
        Student s1 = new Student();
        s1.name = "abu";
        s1.marks = 78;

        Student s2 = new Student();
        s2.name = "ali";
        s2.marks = 88;

        Student students[] = new Student[2];
        students[0] = s1;
        students[1] = s2;

        for(Student stud : students)
        {
            System.out.println(stud.name + " : " +stud.marks);
        }
    }
}
//abu : 78
//ali : 88
```
<br>


String adalah class  
bila create variable, sebenarnya kita create object  
tak perlu taip `String name = new String("ali");`  
just taip `String name = "ali";`
```java
class Demo
{
    public static void main(String a[])
    {
        String name = "ali";

        System.out.print("Hello " + name);
    }
}
//Hello ali
```
<br>



```java

```
<br>



```java

```
<br>



```java

```
<br>



```java

```
<br>



```java

```
<br>



```java

```
<br>



```java

```
<br>



```java

```
<br>



```java

```
<br>



```java

```
<br>



```java

```
<br>



```java

```
<br>



```java

```
<br>



```java

```
<br>



```java

```
<br>




