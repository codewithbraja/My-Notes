# My-Notes
All Day to Day Interview Preparation Notes.

<B>Usages of Abstaract Class:</B>
	When you want to create some common functnality and restrict to create object of that class then mark that class as Abstract.<br/>
<B>Usage of abstarct method:</B>
	When you mark a method as abstract then child class must implement it by marking it as Override keyword.<br/>
	<B>Example:</B><br/>
		abstract class test1 { 
		public abstract int mul(int i, int j);  
		}  
		class test2: test1 {  
		public override int mul(int i, int j) {  
		return i * j;  
		}  
		} 
<br/>
<B>Why Singleton pattern have private constructor and sealed class</B>
Ans:Bcz private constructor restrict to create object of the class outside of the class.
Class A
{
 private A()
 {}
 Class B:A
 {}
}
In this example,we can create object of B which internally create object of A.
To Restrict inheritance as well ,we can make class A sealed.
<br/>
<br/>
<B>SQL Functions</B>
<br/>
--SUBSTRING( string, start_position, length )
declare @variable varchar(20)='Girls I Love u..'
set @variable='BOY'+substring(@variable,5,len(@variable)-4)
print @variable
<h5>o/p:</h5>BOYs I Love u..
<br/>
--STUFF (source_string, start, length, add_string)
<br/>
declare @variable1 varchar(20)='Girls I Love u..'
set @variable1=stuff(@variable1,1,4,'BOY')
print @variable1
<h5>o/p:</h5>BOYs I Love u..
