# my-java-
package ass7;

public class Date {
	private int day,month,year;
	public Date()
	{
		day=month=1;
		year=2022;
		
	}
	public Date(int d,int m,int y)
	{
		day=d;
		month=m;
		year=y;
	}
   public String  displayDate()
   {
	   return "Date :"+day+"month"+month+"year"+year;
   }
	

}
package ass7;

public class Person 

	{
		// TODO Auto-generated method stub

	private String name;
	private Date dob;
	public Person()
	{
		name=null;
		dob=null;
	}
	public Person(String name,Date dob)
	{
		this.name=name;
		this.dob=dob;
	}
	public Person(String nm,int d,int m,int y)
	{
		name =nm;
		dob=new Date(d,m,y);
		
	}
	public void displayinfo()
	{
		System.out.println("Pearson:"+name+"dob:"+dob.displayDate());
	}
	}


package ass7;

public class Demoperson {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Date d1=new Date(1,11,2022);
		Person p1=new Person("Seeta",d1);
		Person p2 =new Person("geesta",12,2,2012);
		p1.displayinfo();
		p2.displayinfo();

	}

}
