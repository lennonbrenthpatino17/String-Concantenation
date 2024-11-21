# String-Concantenation
import java.util.Scanner;

public class StringConcatenation {
   public static String Concatenation(String str1, String str2, String str3) {
        
        Scanner scan = new Scanner(System.in);
        
        System.out.print("Enter your first name  : ");  
        str1 = scan.nextLine();
        
        System.out.print("Enter your second name : ");  
        str2 = scan.nextLine();
       
        System.out.print("Enter your last name   : ");  
        str3 = scan.nextLine();
        
        
        int len1 = str1.length();                
        int len2 = str2.length();                     
        int len3 = str3.length();                       
         
        char[] str4 = new char[len1 + len2 + len3];     
        
        int i = 0;                                      
        while (i < len1) {
            str4[i] = str1.charAt(i);
            i++;
        }
        
        int j = 0;
        while (i < len1 + len2) {
            str4[i] = str2.charAt(j);
            i++;
            j++;
        }
        
        int x = 0;
        while (i < len1 + len2 + len3) {         
            str4[i] = str3.charAt(x);
            i++;
            j++;
            x++;
       }

        return new String(str4);
        
    }
    
    
    public static void main(String[] args) {
       String str1 = " ";
       String str2 = " ";
       String str3 = " ";
       
       
       String StringConcatenation = Concatenation(str1, str2, str3);
       System.out.println(StringConcatenation);
         
    }
}
