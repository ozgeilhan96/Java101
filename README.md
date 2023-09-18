# Java101
import java.sql.SQLOutput;
import java.util.Scanner;
public class Baslangic {
public static void main(String[] args) {
        int n1,n2,select;
        Scanner input=new Scanner(System.in);
        System.out.print("İlk sayıyı giriniz:");
        n1=input.nextInt();
        System.out.print("İkinci sayıyı giriniz:");
        n2=input.nextInt();
        System.out.println("Yapacağınız işlemi seçiniz:");
        System.out.println("1-Toplam\n2-Çıkarma\n3-Çarpma\n4-Bölme");
        select=input.nextInt();
        switch(select){
            case 1:
                System.out.println("Toplam="+(n1+n2));
                break;
            case 2:
                System.out.println("ÇLıkarma="+(n1-n2));
                break;
            case 3:
                System.out.println("Çarpma="+(n1*n2));
                break;
            case 4:
                if(n2!=0){
                    System.out.println("Bölme="+(n1/n2));
                }
                System.out.println("Bir sayı 0'a bölünemez!");
                break;
            default:
                System.out.println("Hatalı bir işlem seçtiniz!");
                break;

        }
    }
}
