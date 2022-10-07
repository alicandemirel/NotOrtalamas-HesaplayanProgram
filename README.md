import  java.util.Scanner;

public class OrtalamaHesaplaProgramı {
    public static void main(String[] args) {
        int mat, fizik, kimya, turkce, tarih, muzik;

        Scanner inp = new Scanner(System.in);

        System.out.print("Matematik notunu giriniz: ");
        mat = inp.nextInt();


        System.out.print("Fizik notunu giriniz: ");
        fizik = inp.nextInt();


        System.out.print("Kimya notunu giriniz: ");
        kimya = inp.nextInt();

        System.out.print("Türkçe notunu giriniz: ");
        turkce = inp.nextInt();

        System.out.print("Tarih notunu giriniz: ");
        tarih = inp.nextInt();

        System.out.print("Müzik notunu giriniz: ");
        muzik = inp.nextInt();

        int toplam = (mat + fizik + kimya + turkce + tarih + muzik);
        double ort = toplam/6;
        System.out.print("Ortalamanız: ");
        System.out.println(ort);

        boolean sonuc = ort>60;

        System.out.println("----------------------------------");

        String str = sonuc ? "Tebrikler sınıfı geçtiniz!" : "Sınıf tekrarı... :(";
        System.out.print(str);


    }
}
