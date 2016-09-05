import java.util.Scanner;

public class myproject {
	
	public static void main(String[] args){
		int result;
		int res =2;
		System.out.println("Give a number");
		Scanner n = new Scanner(System.in);
		int number = n.nextInt();
		int temp = 0;
		System.out.println("The prime numbers from 0 to " + number + " are:");
		for (int i=2; i<=number; i++){
			result = 0;
			temp = i;
			for(int j = 1; j<=temp; j++){
				res = temp % j;
				if (res == 0){
					result+= 1;
				}
			}
		if (result == 2){
			System.out.println(temp);
		}
		}
	}	
}
