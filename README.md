# 1-circle-object
a practice of class
public class CirclePractice{
	public static void main(String[] args){
		Circle Cir1 = new Circle();
		showContent(Cir1);
		Circle Cir2 = new Circle(5);
		showContent(Cir2);
		Cir2.setRadius(10);
		showContent(Cir2);
	}

	public static void showContent (Circle c){
		System.out.println("Radius: " + c.getRadius());
		System.out.println("Area: " + c.getArea());
		System.out.println("Premeter:" + c.getPremeter());
	}
}

class Circle{
	double radius = 1;

	Circle () {
	}

	Circle(double r){
		radius = r;
	}

	double getRadius (){
		return radius;
	}
	
	double getArea () {
		return 3.14 *radius *radius;
	}

	double getPremeter () {
		return 2*3.14*radius;
	}

	void setRadius(double s) {
		radius = s;
	}
}
