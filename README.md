# Restaurant-Bill-Splitter
It Splits The bill :)
    
    import java.util.Scanner;
    public class Main {
    public static  void main(String[]args){

        Scanner scanner = new Scanner(System.in);

        double Bill ;
        double tip ;
        int people ;
        double tipReceived;
        double totalBill ;
        double billShared ;
        char percentage = '%';



        System.out.print("Hi , I hope you enjoyed your meal . Please tell us the bill amount :$" );
        Bill = scanner.nextDouble();

        System.out.print(" Ok , Please tell the amount of tip you want to give (If you wish ) : " + percentage );
        tip = scanner.nextDouble();

        System.out.print(" And please mention the amount of people splitting the bill : ");
        people = scanner.nextInt();

        tipReceived = (tip / 100) * Bill;
        totalBill = Bill + tipReceived ;

        billShared = totalBill / people;

        System.out.println(" Your total bill is :$ " + totalBill + "\n And among " + people + " people ,each person will give :$ " + billShared );

        scanner.close();
