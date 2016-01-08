MEKELLE UNIVERSITY
ETHIOPIAN INSTITUATE OF TECHNOLOGY(EIT-M)	
SCHOOL OF COMPUTING
DEPARTMENT OF INFORMATION SYSTEM	
Assignment: Java
                         section-3

Group  members:
Name                                              Id
1.	Tamene yirsaw                  Eit-m/ur84079/07                              
2.	Misgan yidersal                   Eit-m/ur83905/07
3.	 Mebrahtu tesfhuney           Eit-m/ur163648/06
4.	Teamuru Gebremariam            Eit-m/ur84026/07
5.	 . G/geyoregis Abrha           Eitm/ur83710 /07





1.	
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

packagefibonacci;

import java.util.Scanner;


 */
public class Fibonacci {

    

     
public static void main(String[] args) { 
        //input to print Fibonacci series upto how many numbers
System.out.print("Enter number upto which Fibonacci series to print: ");
int number = new Scanner(System.in).nextInt();

System.out.println("\n\nFibonacci series upto " + number +" numbers : ");
        //printing Fibonacci series upto number
for(int i=1; i<=number; i++){
System.out.print(fibonacciRecusion(i) +" ");
        }
    } 

    // Java program for Fibonacci number using recursion.
public static intfibonacciRecusion(int number){
if(number == 1 || number == 2){
return 1;
        }

returnfibonacciRecusion(number-1) + fibonacciRecusion(number -2); //tail recursion
    }

    // Java program for Fibonacci number using Loop.
public static intfibonacciLoop(int number){
if(number == 1 || number == 2){
return 1;
        }
int fibo1=1, fibo2=1, fibonacci=1;
for(int i= 3; i<= number; i++){
fibonacci = fibo1 + fibo2; //Fibonacci number is sum of previous two Fibonacci number
            fibo1 = fibo2;
            fibo2 = fibonacci;

        }
returnfibonacci; //Fibonacci number
    }     


1.2   package factorial;

import java.util.Scanner;


 
 
 
public class Factorial {


public static void main(String[] args) {

      Scanner scanner = new Scanner(System.in);
System.out.println("Enter the number for factorial calculations");

int a = scanner.nextInt();
double fact= 1;

System.out.println("Factorial of " +a+ ":");
for (int i= 1; i<=a; i++){
fact=fact*i;
      }
System.out.println(fact);
   }
}
2.
importjava.util.HashMap;
importjava.util.Map;

importjavax.xml.stream.events.Characters;

public class EncryptDecrypt {
	static Map<String,String> Dictionary = new HashMap<String,String>(); 
	static Map<String,String>RevDictionary = new HashMap<String,String>();
	
	EncryptDecrypt(){
		
		Dictionary.put("A","%");
		Dictionary.put("a","9");
		Dictionary.put("B","@");
		Dictionary.put("b","#");
		Dictionary.put("C","1");
		Dictionary.put("c","2");
		Dictionary.put("D","3");
		Dictionary.put("d","4");
		Dictionary.put("E","5");
		Dictionary.put("e","6");
		Dictionary.put("F","7");
		Dictionary.put("f","8");
		Dictionary.put("G","0");
		Dictionary.put("g","}");
		Dictionary.put("H","{");
		Dictionary.put("h","]");
		Dictionary.put("I","[");
		Dictionary.put("i",",");
		Dictionary.put("J",".");
		Dictionary.put("j",">");
		Dictionary.put("K","<");
		Dictionary.put("k","/");
		Dictionary.put("L","0");
		Dictionary.put("l","\\-");
		Dictionary.put("M","\\\"");
		Dictionary.put("m","::");
		Dictionary.put("N",";");
		Dictionary.put("n","+");
		Dictionary.put("O","S");
		Dictionary.put("n","-");
		Dictionary.put("Q","$");
		Dictionary.put("q","%");
		Dictionary.put("R","^");
		Dictionary.put("r","&");
		Dictionary.put("S","*");
		Dictionary.put("s","(");
		Dictionary.put("T",")");
		Dictionary.put("t","~");
		Dictionary.put("U","10");
		Dictionary.put("u","5");
		Dictionary.put("V","\\\\");
		Dictionary.put("v","+");
		Dictionary.put("W","=");
		Dictionary.put("w","7");
		Dictionary.put("X","~");
		Dictionary.put("x",")");
		Dictionary.put("Y","2");
		Dictionary.put("y","*");
		Dictionary.put("Z","]");
		Dictionary.put("z","8");
	
	}
	
	
	static String Encrypt(String input){
		
				
		String encrypted="";
		String character;
		charcharOfString;
		
		for(int i=0;i<input.length();i++){
			
			charOfString = input.charAt(i);
			character = ""+charOfString;
	
			if(Dictionary.containsKey(character)){
		encrypted =encrypted + Dictionary.get(character);
	       }
		}
		
		return encrypted;
	}	
	
	static String Decrypt(String input){
		
		String Decrypted = "";
		
		String character;
		charcharOfString;
		
		for(int i=0;i<input.length();i++){
			
			charOfString = input.charAt(i);
			character = ""+charOfString;
	
			if(Dictionary.containsKey(character)){
		   Decrypted =Decrypted + Dictionary.get(character);
	       }
			System.out.println(Dictionary);
		}
		return Decrypted;
	}
	public static void main(String[] args) {
		// TODO Auto-generated method stub
         String val ="Kibrom";
		 String encrypt = Encrypt(val);
		
		LinearCrypto op = new LinearCrypto();
		System.out.println(op.getCode());
		
	}

}
3.


packageBanck;

import java.util.Scanner;
public class customer2 {
double deposit;
intaccount_number;
        String name;
double balance;
double withdraw;
double  deposit(double x){
        Scanner input=new Scanner(System.in);
System.out.println(" enter amount to be deposit");
      x=input.nextDouble();
balance+=x;
return balance;
    }
double withdraw(double y){ 
        Scanner input=new Scanner(System.in);
System.out.println("enter  amount to be withdraw");
        y=input.nextDouble();
if(y<=balance){
balance-=y;
    } 
else {

System.out.println("your balance is low");
        }
return balance;
        }
public static void main(String[] args)
       {
            String name;
intaccount_number;
            Banck3 bk=new Banck3();
            Scanner input=new Scanner(System.in);
System.out.print("enter your name");
name=input.nextLine();
System.out.println("enter your account_number");
account_number=input.nextInt();
bk.deposit();
bk.withdraw();


   } 
   }
4.


package reverse22;
import java.io.*;
import java.io.BufferedReader;
import java.io.IOException;
importjava.io.InputStreamReader;


public class Reverse{

    
     * @param args the command line arguments
     * @throws java.io.IOException
     */
public static void main(String[] args) throws IOException {
        // TODO code application logic here
          BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
System.out.print("Enter string: ");
        String s = br.readLine();
        String reverse = "";
int length = s.length();

for (int i = length - 1; i >= 0; i--)
        {
reverse = reverse + s.charAt(i);
System.out.println("Result:" + reverse); 
        // TODO code application logic here
    }
}
}


5. 


import java.util.Scanner;

/*
 * To change this license header, choose License Headers in Project Properties.z
public class number1 { 
intoddnumber=0;
intsmallestnumber=0;
intlargestnumber=0;
intevennumber=0;
intprimenumber=0;
voidNnum(){
int N;
        Scanner input=new Scanner(System.in);
System.out.println("enter the amount of number");
      N=input.nextInt(); 
for(int i=1;i<=N;i++){
if(i%2==0){
evennumber++;
System.out.println("the number are even" +i);
            }
else  if(i%2!=0){ 
oddnumber++;
System.out.println("the number are odd" +i +oddnumber);
                }
else if((i%2!=0)&&(i%3!=0)){
primenumber++;
System.out.println("the number are primenumber"+i);
            }
else if(i<++i){
largestnumber++;
System.out.println("the largestnumber is"+ ++i);

                }
else
                 {
smallestnumber++;
System.out.println("the number is smallestnumber"+i);
            }}

  }
public static void main(String[] args)
           {
number1num=new number1();
num.Nnum();

            }
        }
















