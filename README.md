# Taksimetre-Program-

Java ile gidilen mesafeye (KM) göre taksimetre tutarını ekrana yazdıran programı yazın.

Taksimetre KM başına 2.20 TL tutmaktadır.
Minimum ödenecek tutar 20 TL'dir. 20 TL altında ki ücretlerde yine 20 TL alınacaktır.
Taksimetre açılış ücreti 10 TL'dir.


import java.util.Scanner;
public class Main {
    public static void main (String[]orgs) {
        // Değişkenleri oluşturuyorum.
        int km;
        double startKm = 2.20, toplam = 10;

        Scanner input = new Scanner(System.in);
        System.out.print("Mesafeyi Km Cinsinden Giriniz : ");
        km = input.nextInt();

       toplam = (km * startKm);
       toplam += 10;

       toplam = (toplam < 20 ) ? 20 : toplam;
       System.out.print("Ödeyeceğiniz Tutar : " + toplam);


