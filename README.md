# unit-9-
9.9
public class RegularPolygon {

    private int n = 3;
    private double side = 1;
    private double x = 0;
    private double y = 0;
    public RegularPolygon()
    {
  	  
    }
    public RegularPolygon(int n,double side)
    {
  	  this.n=n;
  	  this.side=side;
    }
    public RegularPolygon(int n,double side,double x,double y)
    {
  	  this(n,side);
  	  this.x=x;
  	  this.y=y;
    }
    public int getn()
    {
    	return n;
    }
    public void setN(int n)
    {
    	this.n = n;
    }
    public double getside()
    {
    	return side;
    }
    public void setside(double side)
    {
    	this.side = side;
    }
    public double getx()
    {
    	return x;
    }
    public void setx(double x)
    {
    	this.x = x;
    }
    public double gety()
    {
    	return y;
    }
    public void sety(double y)
    {
    	this.y = y;
    }
    public double getPerimeter()
    {
    	return n*side;
    }
    public double getArea()
    {
    	return (n*side*side)/(4*Math.tan(Math.PI/n));
    }
    public static void main(String[] args) {
		// TODO Auto-generated method stub
		RegularPolygon regular1 = new RegularPolygon();
		System.out.println("regular1周长："+regular1.getPerimeter()+"    "+"regular1面积："+regular1.getArea());
		RegularPolygon regular2 = new RegularPolygon(6,4);
		System.out.println("regular2周长："+regular2.getPerimeter()+"    "+"regular2面积："+regular2.getArea());
		RegularPolygon regular3 = new RegularPolygon(10,4,5.6,7.8);
		System.out.println("regular1周长："+regular3.getPerimeter()+"    "+"regular1面积："+regular3.getArea());
	}
}
