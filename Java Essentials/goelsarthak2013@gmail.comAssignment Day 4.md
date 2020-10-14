### Create an int array with 5 values and print only odd values.
```
class Main {
  public static void main(String[] args) {
    int arr[] = new int[5];//declare array
    Scanner sc = new Scanner(System.in);
    for(int i=0;i<5;i++)
    {
      arr[i] = sc.nextInt();
      if(i % 2 != 0 || i == 1)
      System.out.println(arr[i]);
    }
  }
}
```
### Create an int array of size 5, take all the values from the user, add all the values and print the sum.
```
class Main {
  public static void main(String[] args)
  {
    int arr[] = new int[5];
    Scanner sc = new Scanner(System.in);
    int sum = 0;
    for(int i = 0 ; i<5;i++)
    {
      arr[i] = sc.nextInt();
      sum += arr[i];
    }
    System.out.println(sum);
  }
}
```
### create a class avenger with properties (name,age,power,weapon,planet) and with functions-getDetails() and displayDetails(). create 5 objects as an array in the main method and call.
```
import java.util.*;
class Avenger{
  int age;
  String power="", name, planet, weapon;
  void getDetails(){
    Scanner sc = new Scanner(System.in);
    System.out.println("Enter the details for Avenger ");
    System.out.println("Enter the age");
    this.age = sc.nextInt();
    System.out.println("Enter the name");
    this.name = sc.nextLine();
    System.out.println("Enter the power");
    this.power = sc.nextLine();
    System.out.println("Enter the weapon");
    this.weapon = sc.nextLine();
    System.out.println("\nThanks for entering details...\n");
  }
  void displayDetails(){
    System.out.println("Displaying details for AVENGER "+"\n\nThe name: "+this.name+"\n"+"The age: "+this.age+"\n"+"The power: "+this.power+"\n"+"The weapon: "+this.weapon+"\n"+"The planet: "+this.planet);
  }
}
class Main {
  public static void main (String[] args) {
    Avenger av[] = new Avenger[5];
    for(int i = 0; i < 5;)
    {
      System.out.println("Enter the details for Avenger: "+i);
      av[i].getDetails();
      System.out.println("Displaying the details for Avenger: "+i);
      av[i].displayDetails();
      i += 1;
    }
  }
}
```
