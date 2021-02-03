# LearningPortfolio
public class Test {

	public static void main(String[] args) {

		System.out.println("Is this a palindrome");

		java.util.Scanner s = new java.util.Scanner(System.in);
		
		String input = s.nextLine();
		
		System.out.println("You typed this.");
		System.out.println(input);
		
		boolean isPalindromebool = false;
		
		isPalindromebool = isPalindromemethod(input);
		
		
		if (isPalindromebool)
			System.out.println("Yes is a palindrome : "+ input);
		else
			System.out.println("No is not a palindrome : "+ input);
	}

	private static boolean isPalindromemethod(String input) {
		
		int i = 0, j = input.length() -1; 
		
		while (i<j) {
			
		if (input.charAt(i) != input.charAt(j))
			return false;
		
		i++;
		j--;
		
		return true; 
		
		}
		return false;
	
	}

}
