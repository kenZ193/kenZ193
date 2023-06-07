
package ws3part2;
import java.util.Scanner;
import java.util.regex.Pattern;
import java.util.regex.Matcher;


public class WS3part2 {
   
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Management management = new Management();
        
        while(true){
      System.out.println("Enter 1 : To insert a new guitar ");
      System.out.println("Etner 2: To search guitar by serialNumber");
      System.out.println("Enter 3: To exit");
      System.out.print("Enter your option: ");
      String type = sc.nextLine();
      switch(type){
          case "1":{
              String serialNumber;
              Matcher matcher;
 Pattern pattern = Pattern.compile("SE\\d{6}$");

do {
    System.out.println("Enter serialNumber: ");
    serialNumber = sc.nextLine();
    matcher = pattern.matcher(serialNumber);
    
    if (!matcher.matches()) {
        System.out.println("Serial number không hợp lệ. Vui lòng nhập lại.");
    }
} while (!matcher.matches());
            
              System.out.println("Enter price: ");
              int price =sc.nextInt();
              sc.nextLine();
              System.out.println("Enter builder: ");
              String builder = sc.nextLine();
              System.out.println("Enter model: ");
              String model = sc.nextLine();
              System.out.println("Enter back Wood: ");
              String backWood = sc.nextLine();
              System.out.println("Enter top Wood: ");
              String topWood = sc.nextLine();
              guitars guitar = new guitars(serialNumber,price,builder,model,
              backWood,topWood);
              management.addGuitar(guitar);
              System.out.println("=====================");
              guitar.Show();
              System.out.println("=====================");
              
              break;
          }  
          case "2":{
              System.out.println("Search serialNumber: ");
              String serial = sc.nextLine();
              System.out.println("The result: ");
              management.searchByserial(serial);
          } 
          case "3":{
              return;
        }
    }
    }
    }
}
