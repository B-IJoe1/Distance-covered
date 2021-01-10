# Distance-covered
The distance covered from using 4 points: x1, x2, y1, y2
Using the public main method to invoke the public static method userInput 


    package lab02;

    public class ExFinal {

    public static void main(String[] args) {

    Ex_Q1 A1=new Ex_Q1();
	  A1.userInput();
	    }
    }


/////////////////////////////////////

    public static void userInput()
    {
	Scanner input = new Scanner (System.in);
	System.out.print("print out num for x1");
	double x1 = input.nextDouble();
	System.out.print("print out num for x2");
	double x2 = input.nextDouble();
	System.out.print("print out num for y1");
	double y1 = input.nextDouble();
	System.out.print("print out num for y2");
	double y2 = input.nextDouble();
	
	distance(x1,x2,y1,y2);
    }


    public static void distance (double x1, double x2, double y1, double y2)
    {
	
	double result1 = (x2-x1) * (x2-x1);
	
	double result2 = (y2-y1) * (y2-y1);
	
	double result3 = result1 + result2;
	
	double finalresult= Math.sqrt(result3);
	

	System.out.print("The distance covered is: " + finalresult);
	
	
    }
