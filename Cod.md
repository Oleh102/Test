import java.util.Scanner;
import java.util.StringTokenizer;

class Main {
	private static Scanner sc;

	public static void main(String[] args) {
		sc = new Scanner(System.in);
		System.out.print("String: ");
		String s = sc.nextLine();

		s.trim();
	StringTokenizer st = new StringTokenizer(s, " ");

		int min = st.nextToken().length();
		int max = min;

		while(st.hasMoreTokens()){
			int length = st.nextToken().length();
			if(min>length) min = length;
			if(max<length) max = length;
		}

		System.out.println("Longest: " + max +"\nShortest: "+min);
		
	}
}








Cod lab 5
class Main

{ 
public static void main (String [] args) 
{ try 
{ 

int n = Integer.parseInt (args [0]); 
System.out.println ("After parselnt ()"); 
System.out.println ("10 / n =" + (10 / n)); 
System.out.println ("After results output"); 
}
catch (ArithmeticException ae) 
{ 
System.out.println ("From Arithm.Exc.catch:" + ae); 
} 
catch (ArrayIndexOutOfBoundsException arre) 
{ 
System.out.println ("From Array.Exc.catch:" + arre); 
}
{ System.out.println ("From finally"); 
} 
System.out.println ("After all actions"); 
}
}
