package Exercise;

import java.util.Scanner;

public class sınıfıGeçme {
    public static void main(String[] args) {

        int mat, fizik, kimya, turkce, music;
        int toplamNot=0 ,  dersSayisi =0;








        Scanner input = new Scanner(System.in);

        System.out.print("Matematik notunuz: ");
        mat = input.nextInt();
        if (mat >= 0 && mat <= 100) {
            toplamNot += mat;
            dersSayisi++;
        }

        System.out.print("Fizik notunuz: ");
        fizik = input.nextInt();
        if (fizik >= 0 && fizik <= 100) {
            toplamNot += fizik;
            dersSayisi++;
        }

        System.out.print("Kimya notunuz: ");
        kimya = input.nextInt();
        if (kimya >= 0 && kimya <= 100) {
            toplamNot += kimya;
            dersSayisi++;
        }

        System.out.print("Türkçe notunuz: ");
        turkce = input.nextInt();
        if (turkce >= 0 && turkce <= 100) {
            toplamNot += turkce;
            dersSayisi++;
        }

        System.out.print("Müzik notunuz: ");
        music = input.nextInt();
        if (music >= 0 && music <= 100) {
            toplamNot += music;
            dersSayisi++;
        }

        if (dersSayisi > 0) {

            double average = (mat + fizik + turkce + music + kimya) / 5;
            if (average >= 55) {
                System.out.println("Tebrikler sınıfı geçtiniz");
            } else {
                System.out.print("Sınıfta kaldnız!");
            }
            System.out.print("Ortalamanız : " + average);
        } else {
            System.out.println("HATA! Ortalama hesaplanamadı lütfen girdiğiniz değerleri kontrol ediniz.");
        }


    }
}
