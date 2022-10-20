# Lab 8 C# Basics
## Exercise 1

```c
using System;

class Program
{
    static void Main(string[] args)
    {
        for(int i = 0; i < 11; i++)
        {
                Console.Write(i + “ ”);
        }
            
    }  
}
```

## Exercise 2

```c
using System;

class Program
{
    static void Main(string[] args)
    {
        int i = 1;
     
        while (i <= 10)
        {
            Console.WriteLine(i);
            i++;
        }
       
    }  
}
```

## Exercise 3

```c
using System;

class Program
{
    static void Main(string[] args)
    {
        int i = 0;
        do
        {
            Console.WriteLine(i);
            i++;
        } while (i <= 10);
    }  
}
```

## Exercise 4

```c
using System;

class Program
{
    static void Main(string[] args)
    {
        int i = 0;
        while (i <= 100){

          if (i % 3 == 0 || i % 4 == 0)
               {
                   Console.WriteLine(i);
    			}

          i++;
                        }

    }  
}

```

## Exercise 5

```c
Result has no initial value defined
```

## Exercise 6

```c

using System;

class Car
    {
        public string make { 
			ReadOnly { return make;} 

			set{ 
                    if (string.IsNullOrEmpty(make))
				{make = vlaue; }
                  }

			}

        public string model { ReadOnly { return model;} }

        public string colour { ReadOnly { return colour;} }

        public string registration-number { ReadOnly { return registration-number;} }
  
		public int Display ( )
			{
  			  Console.WriteLine( "make:"+make+
							" model:"+model+
							" colour:"+colour+
							" registration-name"+registration-name);
			}

        public Car(string make,string model,string colour,string registration-number) {

            this.make = make;

            this.model = model;

            this.colour = colour;

            this.registration-number = registration-number;

        }
    }

```

## Exercise 7

```c
Start1:

 while (true)
 {
 
try {

 if(!(double.TryParse(Console.ReadLine(), out double a))){
 Console.WriteLine("Please enter a numnber!");
 goto Start1;}

 }    catch (Exception ex){ }  

Start2:

try {

 if(!(char.TryParse(Console.ReadLine(), out char c))){
 Console.WriteLine("Please enter correct operator: + - * / ");
 goto Start2;}
 
 else if (!(c == '+' || c == '-' || c == '*' || c == '/'))
 {
 Console.WriteLine("Please enter correct operator: + - * / ");
 goto Start2;
 }
 
 }    catch (Exception ex){ }

Start3:

try{
 if (!(double.TryParse(Console.ReadLine(), out double b)))
 {
 Console.WriteLine("Please enter a numnber!");
 goto Start3;
 }
}     catch (Exception ex){ }

finally{
 if (c == '+')
 {
 Console.WriteLine(a.ToString() + " + " + b.ToString() + " = " + 
(a + b));
 }


 else if (c == '-')
 {
 Console.WriteLine(a.ToString() + " - " + b.ToString() + " = " + 
(a - b));
 }


 else if (c == '*')
 {
 Console.WriteLine(a.ToString() + " * " + b.ToString() + " = " + 
a * b);
 }


else if (c == '/')
 {
 Console.WriteLine(a.ToString() + " / " + b.ToString() + " = " + 
(Math.Round((a / b), 2)).ToString());
}
}


```
