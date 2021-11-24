# C++ basics

## Data types or literals
>always type inside int main

### Char

- `char initial = 'B';`
- single quotation mark
- always end with semi coloan
- **single letters**

### String

- `string name = "dhanasekaren" or "i am dhanasekaren";`
- varible are strings
- double quotation mark
- always end with semi coloan 
- **words or sentence** 

### Integers

- `int age = 1 or 2 or 3;`
- int do not want any quotations
- always end with semi coloan
- integers 32 bit **(whole, octal, hex)**

### Folat point

- `double mark = 72.5 or 63.23 ;`
- double do not want any quotations
- always end with semi coloan
- double 64 bit **(decimal)**
 
### Booliean

- `bool studying = true or false;`
-  do not want any quotations
- always end with semi coloan
- boolean constants **1 and 0** or  true or false

### Printing

- `cout << "i am typing" << endl;`
- double quotation mark
- always end with semi coloan
- this is **constant** without using any other datas 

### Pointer

- `cout << &name << endl;`
- the program the shows the location of the name in ram
- we call it pointer
- & is the comment to show the location
- if we  use * it go the location and give the output 

## String

> name : dhanasekaren

- `cout << "dhanasekaren \n come here" << endl;`
- `\n` : newline
- `\\` : backslash 
- `\'` : single quote
- `\"` : double quote

### Length

- `cout << name.length << endl;`
- output :11
- **total number** of characters inside a string
- before the null char `\0`

### Index pos

- `cout << name[2] << endl;`
- output : a
- always start from zero
- it gives the **exact letter** when we give the index value
- change character like

### Change index pos

-  `name[0] = 'G';`
- `cout << name << endl`
- output : Ghanasekaren
- to **change a char in string**

### Find index pos using char

- `cout << name.find("s",0);`
- output : 5
- to find the **position of the index** 

### Start to end

- `cout << name.substr(5,7) << endl`
- output : sekaren
- we tell index to **start to end**

## Numbers and maths

> For math use `include <cmath>`

- **arithmetic** it uses BODMAS or PEMDAS rule
- `+ add` , ex : `cout << 4 + 2 << endl;` output = 6
- `- sub` , ex : `cout << 4 - 2 << endl;` output = 2
- `* mul` , ex : `cout << 4 * 2 << endl;` output = 8
- `/ div` , ex : `cout << 4 / 2 << endl;` output = 2
- `% rem` , ex : `cout << 5 / 2 << endl;` output = 1 

### Default add 1

- `++` adds 1
- `int num = 4;`
- `num++;` 
- `cout << num << endl;` output = 5

### Default sub 1

- `--` subs 1
- `int num = 4;`
- `num -- ;` 
- `cout << num << endl;` output = 3 

### Add

- `+= 5` adds any number we give
- `int num = 4;`
- `num += 5 ;` 
- `cout << num << endl;` output = 9 
 
### Sub

- `-= 2` adds any number we give
- `int num = 4;`
- `num += 2 ;` 
- `cout << num << endl;` output = 2 

### Mult and Divi

- same thing for `*=` and `/=`
- output = 8
- output = 2

### Power

- `cout << pow (4, 2) << endl;`
- pow is power of ex : $4^2$
- output : 16

### Square root

- `cout << sqrt(4) << endl;` 
- it is opp of pow it gives the squre root of 4
- output : 2

### Round value using >5 or <5

- `cout << round(5.68656) << endl;`
- it rounds the value 
- output : 6 
- if we give (5.4), output : 5

### Round value to highest

- `cout << ceil(5.4123123) << endl;`
- automatically round the number to the next highest number
- output : 6

### Round value to lowest

- `cout << floor(5.9999) << endl;`
- opp of **ceil** number
- output : 5

### To find bigger value

- `cout << fmax(5, 11) << endl;`
- its tell which number is bigger
- output : 11

### To find lowest value

- `cout << fmin(5, 11) << endl;` 
- its tell the smallest number
- output : 5

## Input

> for output we use cout 
> for input we use cin

### How get input from user

- sample code for get input (for words)
- cin >> name ;
``` 
string name;
cout << "what is your name : ";
cin >> name ;
cout << "hi " << name << " i am computer";
```

### Get input from user 

- sample code for get input (sentence, words, letters and numbers)
- getline(cin,anyname)
```
string name;
cout << "what is your name : ";
getline(cin,name);
cout << "hi " << name << " i am computer";
```

## operators

- **switch operator** get the input and switch 
 
	```
	 switch (expression)
	 {
	 case /* constant-expression */:
	 /* code */
	 break;

	 default:
	 break;
	 }
	```

## Arrays

> we can use all data types 
> varible is like (only integer or only char) 

- arrays example
 
	```
	 string names[] = {"dhanasekaren", "mohanen", "bala", "karthi", "rambai", "vijay", "dhanush"};
	 cout << names[0]<< endl;
	```

- now we can take what name we want by using index value
- and same for char, int, float, double and strings
- **2d arrays** 
- same like arrays
		```
		 string names[][] = {dhana,saker},{mohan,bala};
		 cout << names[0][1]<< endl;
		```
- we use another list
- list[][] like this 

## Functions

> A set of instructions
> int main () is also a function

- example for fuction
	```
	#include <iostream>
	using namespace std;

	void names(int num)
	{
	 string name[] = {"dhanasekaren", "mohanen", "bala", "karthi", "rambai", "vijay", "dhanush"};
	 cout << name[num] << endl;
	}
	int main()
	{
	 names(3)
	 return 0;
	}
	```
- here void is a function 
- we can call function many times
- always create a function above the main function

## return statement

- example for return
	```
	#include <iostream>
	#include <cmath>
	using namespace std;

	int number (int num)
	{
	 num = num + num + num;
	 return num;
	}
	int main()
	{
	 cout << number(2) <<endl;
	 return 0;
	}
	```
- to return the value to the orginal

## if state ment

- user name and password ex for if statement
	```
	#include <iostream>
	using namespace std;
	int main()
	{
	 string myname = "dhanasekaren";
	 string password = "pingu";
	 string name;
	 string pass;
	 cout << "Enter your name : " ;
	 cin >> name ;
	 cout << "Enter your password : ";
	 cin >> pass ;
	 if (myname == name && password == pass)
	 {
	 cout << "Hello " << myname << endl;
	 cout << "Welcome to home" << endl;
	 }
	 else
	 {
	 (myname != name) && (password != pass);
	 cout << "Wrong user name or password" << endl;
	 }
	 return 0;
	}
	```
- if (), else if(), else are various types to use

## while loop 

- while loop ex :
	```
	 int age = 1;
	 int myage = 17;
	 while(age <= myage)
	 {
	 cout << age << endl;
	 age ++;
	 }
	```
- output : 1,2,3,4,.....,17
- if loop god is equal program will stop

## do while loop

- do while loop ex:
	```
	int age = 18;
	 int myage = 17;
	 do{
	 cout << age << endl;
	 age ++;
	 }while(age <= myage);
	```
- output : 18
- if loop god is equal still do loop will run 1 time

##  for loops

- for loops ex 
	```
	for(i=1;i<=5;i++){
	cout<<i<<endl;
	}
	```

- for is also like while loop but it easier compare to while loop
- we can give a list to for check

## nested for loop

- it basically for 2d arrays or more
- its is same as for loops
- but add 1 more for loop
- for the second list

## class
- we can create our own class by using class
- personal , private
- class make our job simple and easier

## inheritance
- we can call a function form 1 class to another
- we call it super class and sub class
- super class is the one which give function to other class
- sub class is we can take fucntion from other class if its is public

