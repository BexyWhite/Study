#Study Encapsulation
##Feature
When you creat a class which contains private variables,you should create a public method to make them accessable.
```java
class Calculator{
	private int num1;
	private int num2;
	private	char option ;
  //a public method			
	public void initCalculator(int n1 , int n2 , char o){
		num1 = n1;
		num2 = n2;
		if(o=='+'||o=='-'||o=='*'||o=='/'){
			option = o;
		}else{
			option = '+';	
		}
	}
	public void calculate(){...}

class Demo 
{
	public static void main(String[] args) 
	{
		Calculator c = new Calculator();
		//set
		c.initCalculator(1,2,'a');
		c.calculate();
	}
}

```
