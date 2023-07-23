package org.constr;
public class Employee1 {
	String name,projectname;
	int id;
	static String companyName="tcs";
	static {
		String companyName ;
	}
	public Employee1(String string,int i,String string2) {
		this.name=string;
		this.id=i;
		this.projectname=string2;
	}
	private void empDetail() {
		System.out.println("name is"+name);
		System.out.println("id is"+id);
		System.out.println("projectname is"+projectname);
		System.out.println("companyname is"+companyName);
	}
	private static void changecompanyname() {
		companyName="wipro";
	}
	public static void main(String[] args) {
		Employee1 revanth=new Employee1("revanth",4326,"canary");
		Employee1 naveen=new Employee1("naveen",3245,"mercury");
		Employee1 pavin=new Employee1("pavin",5436,"batman");
		Employee1 deepan=new Employee1("deepan",6754,"whistler");
		revanth.empDetail();
		System.out.println();
		naveen.empDetail();
		Employee1.changecompanyname();
		pavin.empDetail();
		deepan.empDetail();
	}
 }
