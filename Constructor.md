#Constructor
##feature
* Everytime `new` a object,the constructor will be excute too.
```java
class Emp{
	static	int count = 0;	//counter
	public Emp(){  //Everytime `new` a object,the constructor will be excute too.
		count++;
	}
	public void showCount(){
		System.out.println("Newed "+ count+" objects");
	}
}

class Demo 
{
	public static void main(String[] args) 
	{
		Emp e1 = new Emp();
		Emp e2 = new Emp();
		Emp e3 =new Emp();
		e3.showCount();
	}
}

```
##this
*  `this` can call other methods in its Constructor.(`this` must be the `first` sentence)

 ```java
class demo{
	public demo(int a,string b){
		this();
		...
	}
	public demo(){... }
}
```

* `this` can't make `recursion` happened.
 ```java
class demo{
	public demo(int a,string b){
		this(a);
		...
	}
	public demo(int a){
   `this(a,'bexy');`
  }
}
```
