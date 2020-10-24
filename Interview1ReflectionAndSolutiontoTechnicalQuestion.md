## Review
I think I did a reasonably good talking about myself. The only big change I would make there is never say that I don't have a project I am proud. 
Talk about a project I worked on at university, just something anything other then saying I don't have anything.
On the program problem I need to do a better job of using the interviewer as a resource if he/she says I can.
Secondly don't just jump straight into writing code. Work through the problem verbally and with tracing, etc. before writing any code. Essentially create an abstract and 
work out what needs to be implemented and the basics of how before starting to code.

The technical problem I was given was to move all the zeroes to the end of a given array without cloning the array.
Here is my solution that I have since come up with:

```Java
import java.util.Arrays;

public class Main {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		int[] input1 = {0,1,4,5,0};
		int[] input2 = {0,9,0,4,5,0,3,2,1};
		int[] input3 = {1,0,2,0,3};
		input1 =moveZeroes(input1);
		System.out.println(Arrays.toString(input1));
		input2 =moveZeroes(input2);
		System.out.println(Arrays.toString(input2));
		input3 =moveZeroes(input3);
		System.out.println(Arrays.toString(input3));
	}
	
	public static int[] moveZeroes(int[] n) {

		int count = 0;
		for (int i = 0; i < n.length; i++)     
			if (n[i] != 0)         
				n[count++] = n[i]; 
		
		while (count < n.length) {
			n[count++] = 0; 		
		}
		
		return n;
	}

}
```
