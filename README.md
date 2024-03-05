# Arraylist-and-LinkedList

package Collectionn;

package Collectionn;

import java.util.ArrayList;
import java.util.Iterator;
import java.util.List;

public class Arraylistt {

	public static void main(String[] args) 
	{
		List al = new ArrayList();
		//It is use to add the method
		al.add("Kiran");
		al.add("Xyz");
		al.add("ABc");
		al.add("PQR");
		al.add(0, "PQR"); //PQR is added at 0 index.
		al.add("Xyz");
		
		System.out.println(al);
//		iterator use to print element one by one
		Iterator itr = al.iterator();
		while(itr.hasNext())
		{
			System.out.println(itr.next());
		}
//		use to clear everything
		al.clear();
		System.out.println(al);
//		it is use to make a copy .
				
		System.out.println(al);
//		it will tell the last index of that object if it not present then output will be negative
		System.out.println(al.lastIndexOf("PQR")); //last position
		System.out.println(al.lastIndexOf("PQr")); //-1
//		it check wether it is empty or not
		System.out.println(al.isEmpty());
		
		System.out.println(al.contains("Pqr"));
//		it will tell the first index value of that of value
		System.out.println(al.indexOf("PQR"));
		al.remove("PQR");
		System.out.println(al);
//		al.removeRange(0,3);
//		it will pirnt the sublist
		System.out.println(al.subList(1, 3));
//		 	 it will tell the size of arraylist
		System.out.println(al.size());
//		it will reset new value at given index
		al.set(0, "KKKKK");
		System.out.println(al);
	}
	

}




--------------------------------------------LINKED LIST-------------------------------------------------




import java.util.*;  
public class LinkedList3 {  
  
        public static void main(String [] args)  
        {  
           LinkedList<String> ll=new LinkedList<String>();  
           ll.add("Ravi");  
           ll.add("Vijay");  
           ll.add("Ajay");  
           ll.add("Anuj");  
           ll.add("Gaurav");  
           ll.add("Harsh");  
           ll.add("Virat");  
           ll.add("Gaurav");  
           ll.add("Harsh");  
           ll.add("Amit");  
           System.out.println("Initial list of elements: "+ll);  
         //Removing specific element from arraylist  
              ll.remove("Vijay");  
              System.out.println("After invoking remove(object) method: "+ll);   
         //Removing element on the basis of specific position  
              ll.remove(0);  
              System.out.println("After invoking remove(index) method: "+ll);   
              LinkedList<String> ll2=new LinkedList<String>();  
              ll2.add("Ravi");  
              ll2.add("Hanumat");  
         // Adding new elements to arraylist  
              ll.addAll(ll2);  
              System.out.println("Updated list : "+ll);   
         //Removing all the new elements from arraylist  
              ll.removeAll(ll2);  
              System.out.println("After invoking removeAll() method: "+ll);   
         //Removing first element from the list  
              ll.removeFirst();  
              System.out.println("After invoking removeFirst() method: "+ll);  
          //Removing first element from the list  
              ll.removeLast();  
              System.out.println("After invoking removeLast() method: "+ll);  
          //Removing first occurrence of element from the list  
              ll.removeFirstOccurrence("Gaurav");  
              System.out.println("After invoking removeFirstOccurrence() method: "+ll);  
          //Removing last occurrence of element from the list  
              ll.removeLastOccurrence("Harsh");  
              System.out.println("After invoking removeLastOccurrence() method: "+ll);  
  
              //Removing all the elements available in the list       
              ll.clear();  
              System.out.println("After invoking clear() method: "+ll);   
       }  
    }  
