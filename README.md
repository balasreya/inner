# inner
import java.util.*;
class outer
{
    int outer_x;
   void test()
   {
       System.out.println("enter value of outer_x"); 
       Scanner k=new Scanner(System.in);
       outer_x=k.nextInt();
       inner s=new inner();
       s.display();
   }
}
class inner
{
    void display()
    {
        System.out.println("value of outer_x",+outer_x);
    }
}
class Main
{
    public static void main(String[]args)
    {
        outer.o=new outer();
        o.test();
    }
}
