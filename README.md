import java.util.Scanner;

public class Concatenation {
   public static String Concatenation(String str1, String str2, String str3, String str4) {
        
        Scanner s = new Scanner(System.in);
        
        System.out.print("Enter your first name  : ");  
        str1 = s.nextLine();
        
        System.out.print("Enter your second name : ");  
        str2 = s.nextLine();
       
        System.out.print("Enter your middle name : ");  
        str3 = s.nextLine();
        
        System.out.print("Enter your last name   : ");
        str4 = s.nextLine();
        
        
        int len1 = str1.length();                
        int len2 = str2.length();                     
        int len3 = str3.length();  
        int len4 = str4.length();
         
        char[] str5 = new char[len1 + len2 + len3 + len4];     
        
        int i = 0;                                      
        while (i < len1) {
            str5[i] = str1.charAt(i);
            i++;
        }
        
        int j = 0;
        while (i < len1 + len2) {
            str5[i] = str2.charAt(j);
            i++;
            j++;
        }
        
        int x = 0;
        while (i < len1 + len2 + len3) {         
            str5[i] = str3.charAt(x);
            i++;
            j++;
            x++;
       }
        
        int y = 0;
        while (i < len1 + len2 + len3 + len4) {  
            str5[i] = str4.charAt(y);
            i++;
            j++;
            x++;
            y++;
           
       }

        return new String(str5);
        
    }
    
    
    public static void main(String[] args) {
       String str1 = " ";
       String str2 = " ";
       String str3 = " ";
       String str4 = " ";
       
       
       String StringConcatenation = Concatenation(str1, str2, str3, str4);
       System.out.println(StringConcatenation);
         
    }
}
