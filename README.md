        interface Shape
        {
          abstract void getArea(double area);
        }

        class Rectangle implements Shape
        {
          double length;
         double width; 
          public Rectangle(double length,double width)
          {
            this.length=length;
            this.width=width;
         }
          public double getArea()
         {
           return ("area="+length*width);
        }
         public String toString()
         {
           return "area="+getArea();
         }      
        }

        class Triangle implements Shape
        {
          double base;
          double height;
        public Triangle(double base,double height)
         {
            this.base=base;
            this.height=height;
        }
         public double getArea()
         {
           return ("area="+base*height/2);
         }
         public String toString()
         {
           return "area="+getArea();
         }  
        }

        public class app1126{
         public static void main(String arg[])
         {
         Rectangle s1=new Rectangle(3,4);
         Triangle s2=new Triangle(3,4);
         System.out.println(s1);
         System.out.println(s2);
        }
        }
