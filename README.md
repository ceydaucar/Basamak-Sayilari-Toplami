# Basamak-Sayilari-Toplami
Patika.dev > Java101 > Döngüler > Pratik6 - Basamak Sayıları Toplamı

### Ödev
Bir sayının basamak sayılarının toplamını hesaplayan program yazınız.

Örnek : 1643 = 1 + 6 + 4 + 3 = 14


      import java.util.*;

      public class basamak_sayilari_toplami {

        public static void main(String[] args) {

          Scanner sc =  new Scanner(System.in);

          System.out.println("Enter the number: ");
          int n = sc.nextInt();

          int sum = 0;

          while(n != 0) {
            int rakam = n % 10;
            sum += rakam;
            n /=10;

          }

          System.out.println("Sum of digits: " + sum);
        }
      }
