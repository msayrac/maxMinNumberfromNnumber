# maxMinNumberfromNnumber
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

        int max = 0, min = 0;
        Scanner input = new Scanner(System.in);
        System.out.println("Kac tane sayi gireceksiniz : ");
        int n1 = input.nextInt();
        for (int i = 1; i <= n1; i++) {
            System.out.println(i + ". sayiyi giriniz : ");
            int sayi = input.nextInt();
            if (i == 1) {

                max = sayi;
                min = sayi;

            } else {

                if (sayi > max) {
                    max = sayi;
                } else if (sayi < min) {
                    min = sayi;
                }
            }
        }
        System.out.println("En buyuk sayi :" + max);
        System.out.println("En kucuk sayi :" + min);

    }
}
