# My-Notes
All Day to Day Interview Preparation Notes.

Usages of Abstaract Class.
	When you want to create some common functnality and restrict to create object of that class then mark that class as Abstract.
Usage of abstarct method.
	When you mark a method as abstract then child class must implement it by marking it as Override keyword.
	Example
		abstract class test1 { 
		public abstract int mul(int i, int j);  
		}  
		class test2: test1 {  
		public override int mul(int i, int j) {  
		return i * j;  
		}  
		} 
