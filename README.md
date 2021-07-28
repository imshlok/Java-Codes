# Java-Codes
import java.lang.Math;
class process
{
	void prime(int num1,int p1)
	{
		int j,count=0;
		for(j=2;j<num1-1;j++)	//To check if prime
		{
			if(num1%j==0)
			{
				count++;
				break;
			}
		}
		if(count==0)
		{
			System.out.println("Number = "+num1+" and value of 'p' = "+p1);
		}
	}
}
public class Mersenne	//main class
{
	public static void main(String[] args)
	{
		int num;
		process obj = new process();	//Creating object
		for(int i=2;i<32;i++)
		{
			num = ((int)Math.pow(2,i))-1;
			obj.prime(num,i);
		}
	}
}
