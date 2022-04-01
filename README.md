# Recap Basics

1. Which data types do you know and how are they to be declared?
~~~java
boolean a = true; float b = 1f; double c = 2.0; int d = 2; long e = 4; String a = "Hello World!"; char a = 'a';
~~~

2. Declare and initialise a variable with a certain value (pay attention to the correct syntax). Overwrite the value with another value.
~~~java
int a = 25;
a = 30;
~~~

3. Which operators do you know in detail (logical, relational, and mathematical)?
~~~java
logical
||, &&, ==, !=
relational
<, >, <=, >=
mathematical
+, -, /, *, +=, -=, a++, ++a, a++
~~~

4. What are the main differences between the if branch and the switch branch?
~~~java
switch allows for multiple conditions to be met (1 AND 2 AND 3)
~~~

5. Which loops do you know? Brief description of the differences.
~~~java
do, while, for

do usually comes with while at the end and will always run at least one iteration of the loop.
while only enters if the condition is met at the start and will continue to do so until this changes.
for requires a conditional variable which is declared in the statement of the loop itself.
~~~

6. Describe the syntax in detail of the for loop and the while loop, what's the main difference? Are they equally powerful?
~~~java
while (x < 0) — this will continue to loop until x becomes bigger than 0, but will not enter the loop if x is already 0 or bigger

for (int x = -2; x < 0; x++) x is initialised within the statement and continue to run until it becomes equal or bigger than zero, every time the loop is finished, one is added to x, if x equals or is bigger than 0 after one iteration, the loop will end

while is more "powerful" because it does not require a complete statement to terminate the loop before entering, this allows for a much easier possibility of endless loops than for.
~~~

7. Print the numbers 1 to 10 with a specific loop that you can choose yourself.
~~~java
int x = 1;
while (x < 11) {
    System.out.println(x);
    x++;
}

for (int i = 1; i < 11; i++) {
    System.out.print(i);
}
~~~

## Methods
1. Why should we use methods?
~~~java
methods allow for specific actions to be used multiple times without retyping code and can be used across multiple applications
~~~

2. Declare a simple method and describe the structure in detail. Which keywords are important?
~~~java
public static void method (String input1, int input2) {

}
"public" allows for the method to be used "publicly" and not only by the contained class
static
"void" defines whether the method will return something or not. "void" will not return anything after running the method, "int" for example will require an Integer to be returned after finishing the function (e.g.: return int x = 0;)
~~~

3. Which return types do you know?
~~~java
(void [nothing is returned]), any data type available
~~~

4. Declare a method with every return type you know.
~~~java
public static void method (String input1, int input2)
public static boolean method (String input1, int input2)
public static float method (String input1, int input2)
public static double method (String input1, int input2)
public static int method (String input1, int input2)
public static long method (String input1, int input2)
public static String method (String input1, int input2)
public static char method (String input1, int input2)
~~~

## Arrays
1. What is an array?
~~~java
a group or block of elements of the same datatype
~~~

2. Are arrays dynamic?
~~~java
no, arrays can not be changed after initialisation.
~~~

3. Can arrays have more than one dimension?
~~~java
yes, they can have n dimensions
~~~

4. Do you need to know the size of arrays during compile time?
~~~java
yes, array sizes have to be explicitly set before creating it
~~~

5. Which types can arrays have?
~~~java
any of the available data types (declared with e.g. int[])
~~~

6. Declare arrays in two different ways. At least one one-dimensional and one multidimensional 
array.
~~~java
int[] array = new int[2]; //empty one-dimensional array with 2 "slots"
int[][] array2 = {{1,2},{3,4}}; //two-dimensional 2-by-2 array containing the numbers 1 to 4
~~~

7. Sort an arbitrary integer array. Use any algorithm you like.
~~~java
Arrays.sort(array);
~~~

8. Print out a two-dimensional array.
~~~java
for (int i = 0; i < array.length; i++) {
    for (int j = 0; j < array[0].length; j++) {
        System.out.println(array[i][j]);
    }
}

System.out.println(Arrays.toString(array));
~~~

~~~java
String s = "Hello";
~~~
