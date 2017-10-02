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
