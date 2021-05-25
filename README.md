# oop
package project;

import java.util.Scanner;

/**
 *
 * @author Mahmoud Elgzar
 */
public class PROJECT2 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        CAR bmw=new CAR("red","atomatic",2020,4, 130);
         /*bmw.color="red";
         bmw.birthday=2020;
         bmw.tybe="atomatic";
         bmw.speed=130;
         bmw.doors=4;*/
        bmw.setdoors(5);
        System.out.println(bmw.getdoors());
         VAN marcedes=new VAN();
         marcedes.ID=12345;
         marcedes.birthday=2019;
         marcedes.color="white";
        /* marcedes.doors=2;*/
         marcedes.tybe="atomatic";
         marcedes.speed=120;
        
         
         BUS mazda=new BUS();
         mazda.birthday=2010;
         mazda.color="blue";
        /* mazda.doors=1;*/
         mazda.tybe="atomatic";
         mazda.speed=110;
         mazda.chais=60;
         
         MICROBUS Toyota=new MICROBUS();
          
         Toyota.birthday=2015;
         Toyota.color="black";
        /* Toyota.doors=2;*/
         Toyota.tybe="manual";
         Toyota.speed=140;
         Toyota.chais=12;
         Toyota.size=150;
         
         
        Scanner input =new Scanner(System.in);
       int choice =input.nextInt();
       
   switch(choice){
    case 1: System.out.println("color :"+bmw.color+"\n"+"tybe :"+bmw.tybe+"\n"+"age:"+bmw.getage(bmw.birthday)+"\n"+"birthday:"+bmw.birthday+"\n"+/*"doors:"+bmw.doors+"\n"+*/"speed:"+bmw.speed+"\n");
              break;
    case 2: System.out.println("ID:"+marcedes.ID+"\n"+"color :"+marcedes.color+"\n"+"tybe :"+marcedes.tybe+"\n"+"age:"+marcedes.getage(marcedes.birthday)+"\n"+"birthday:"+marcedes.birthday+"\n"+/*"doors:"+marcedes.doors+"\n"+*/"speed:"+marcedes.speed+"\n");
             break;
    case 3: System.out.println("chais:"+mazda.chais+"\n"+"color :"+mazda.color+"\n"+"tybe :"+mazda.tybe+"\n"+"age:"+mazda.getage(mazda.birthday)+"\n"+"birthday:"+mazda.birthday+"\n"+/*"doors:"+mazda.doors+"\n"+*/"speed:"+mazda.speed+"\n");
             break;
    case 4: System.out.println("chais:"+Toyota.chais+"\n"+"color :"+Toyota.color+"\n"+"tybe :"+Toyota.tybe+"\n"+"age:"+Toyota.getage(Toyota.birthday)+"\n"+"birthday:"+Toyota.birthday+"\n"+/*"doors:"+Toyota.doors+"\n"+*/"speed:"+Toyota.speed+"\n"+"size"+Toyota.size+"\n");
             break;
             
             package project;

import java.util.Date;

/**
 *
 * @author Mahmoud Elgzar
 */
public class CAR {
    
  
  public CAR(){
}
    
  public CAR(String color,String tybe,int birthday,int doors, double speed)
   {
     this.color=color;
     this.tybe=tybe;
     this.birthday=birthday;
     this.doors=doors;
     this.speed=speed;
   }
    
    String color ;
   String tybe;
   int birthday;
  private int doors;
   double speed;
   
  Date d=new Date();
   int year=d.getYear()+1900;

    public void setdoors(int doors){
        this.doors=doors;
    }
   int getage(int birthday){
       return year-birthday;
   }
   
    String getcolor(){
        return color;
    }
   String gettybe(){
       return tybe;
   }
   
   int getbirthday(){
       return birthday;
   }
   
   int getdoors(){
       return doors;
   }
   
   double getspeed(){
       return speed;
   
    }
}
package project;

/**
 *
 * @author Mahmoud Elgzar
 */
public class BUS extends CAR {
    int chais;
    
}
package project;

/**
 *
 * @author Mahmoud Elgzar
 */
public class VAN extends CAR{
    double ID;
    package project;

/**
 *
 * @author Mahmoud Elgzar
 */
public class MICROBUS extends BUS {
   
    int size;
    
}

      }}}
