# java-

//calculate x^n without loop
import java.util.*;
public class Main {
   // function for caculate x^n
    public static int calcPower(int x , int n){
        if(n==0){ //base case 1
            return 1;
        }
        if(x==0){ //base case 2
            return 0;
        }
        int xpownm1= calcPower(x,n-1);//recursive function
        int xpown =x*xpownm1;
        return xpown;
    }
    public static void main(String[] args) {//main function
       Scanner sc=new Scanner(System.in);
       int x=sc.nextInt();
       int n=sc.nextInt();
       int ans = calcPower(x,n);//calling calcPower function
        System.out.println(ans);

    }
}
