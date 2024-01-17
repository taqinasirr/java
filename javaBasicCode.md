

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


