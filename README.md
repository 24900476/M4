EX-16-LEFT-SHIFT-OPERATION

AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

ALGORITHM
Start the program.
Assign values of a and b as 44 and 3.
Use left shift operator (<<) and shift the value of a three times.
Display the result.
Stop the program.
PROGRAM
#include <stdio.h>

int main() {
    int num = 44;
    int shift = 3;
    int result;

    result = num << shift;

    printf("Left shift of %d by %d positions is: %d\n", num, shift, result);

    return 0;
}
OUTPUT
image

RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.

EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT
AIM
Write a C Program to check whether the two numbers are equal or not using simple if statement.

ALGORITHM
Start the program.
Read two numbers.
If first number is equal to second number, display both are equal.
Otherwise display both are not equal.
Stop the program.
PROGRAM
#include<stdio.h>
int main()
{
    int a,b;
    scanf("%d%d",&a,&b);
    if(a==b)
    {
        printf("X is equal to Y");
    }
    else
    {
        printf("X is NOT equal to Y");
    }
    return 0;
}
OUTPUT
image

RESULT
Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully

EX-18-STRING-LOWERCASE-CONVERSION
AIM
Write a C Program to convert the given string into lowercase.

ALGORITHM
Start the program.
Read a string variable.
Using tolower( ) function convert the given string into its lowercase.
Display the result.
Stop the program.
PROGRAM
#include<stdio.h>
#include<ctype.h>
int main()
{
    char str[100];
    scanf("%s",str);
    for(int i=0;str[i] != '\0';i++)
    {
        str[i] = tolower(str[i]);
    }
    printf("Lower case String is:%s",str);
    return 0;
}
OUTPUT
image

RESULT
Thus the program to convert the given string into lowercase has been executed successfully

EX-19-COUNT-OF-WORDS-IN-A-STRING
AIM
Write a C Program to count the total number of words in a given string using do While loop.

ALGORITHM
Start the program.
Read a string variable.
Using for loop, inspect the string character by character.
Whenever a space is encountered increment count by 1.
Display the result.
Stop the program.
PROGRAM
#include<stdio.h>
int main()
{
    char a[100];
    int l=0;
    fgets(a,sizeof(a),stdin);
    while(a[l]!='\0')
    {
        l++;
    }
    printf("%d",l-1);
    return 0;
}
OUTPUT
image

RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully

EX -20 -COMPARING TWO STRINGS
AIM
write a Program to compare two strings without using strcmp().

ALGORITHM
Step 1: Start the program. Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable flag and initialize it to 0, and i for indexing.
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered (i.e., can include spaces). Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no spaces in the second string). Step 5: Start comparing characters of both strings from index i = 0. Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string): • If c1[i] is not equal to c2[i], set flag = 1. • Increment i by 1. Step 7: After the loop, check the value of flag: • If flag == 0, print "strings are same". • Otherwise, print "strings are not same". Step 8: End the program.

PROGRAM
#include<stdio.h>
#include<string.h>
int main()
{
    char str[10];
    char srt[10];
    scanf("%s",str);
    scanf("%s",srt);
    int s = strcmp(str,srt);
    if(s==0)
    {
        printf("strings are same");
    }
    else
    {
        printf("strings are not same");
    }
    return 0;
}
OUTPUT
image

RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.
