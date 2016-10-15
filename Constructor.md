#Constructor
##feature
* Everytime `new` a object,the constructor will be excute too.
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
