import java.util.Scanner;

class Do{
	public void findException(){
       int i=2;
       int a[]= new int[4];
       int k;
       try{
    	   Scanner input = new Scanner(System.in);
    	   System.out.println("enter a number");
    	   int j = input.nextInt();
    	   k=i/j;
    	   for(int c=0;c<=4;c++)
    	   {
    		   a[c]=c;
    	   }
    	   for(int value : a)
    	   {
    		   System.out.println(value);
    	   }
       }
       catch(ArithmeticException ae)
       {
    	   System.out.println("Number cant be divided by zero : " + ae);
       }
       catch(ArrayIndexOutOfBoundsException e)
       {
    	   System.out.println("Max numbers in array is 4 :" + e);
       }
       catch(Exception e)
       {
    	   System.out.println("Unkonown exception: " + e);
       }
    }
}
class Jala {
	public static void main(String[] args){
		Do example = new Do();
        example.findException();
	}
}
