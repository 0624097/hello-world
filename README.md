    interface Shape
    {
      abstract void getArea(double);
    }
    
    class Rectangle implements Shape
    {
      double length;
      double width; 
      public void getArea()
      {
        return ("area="+length*width);
      }
      public String toString()
      {
        return "length:"+length+""+"width:"+width+""+"area:"+getArea;
      }      
    }
    
    class Triangle implements Shape
    {
      double base;
      double height;
      public void getArea()
      {
        return ("area="+(base*height)/2);
      }
      public String toString()
      {
        return "base:"+base+""+"height:"+height+""+"area:"+getArea;
      }  
    }
    
    public static void main(String arg[])
    {
      Rectangle s1=new Rectangle(3,4);
      Triangle s2=new Triangle(3,4);
      system.out.println(s1);
      system.out.println(s2);
    }
    
    
