package UASAlpro_202253109;
import java.util.Scanner;
/**
 *
 * @author HP
 */
public class Sistem_Topup_Sederhana {
    private static Scanner input = new Scanner(System.in);

    public static void main(String[] args) {
        int jika, pilihan;
        
        do {
            garis();
            System.out.println("\t SELAMAT DATANG ");
            System.out.println("Metastore.id - Tempat Topup Terpercaya");
            garis();
            System.out.println("\t1. Topup Mobile Legends");
            System.out.println( "\t2. Topup Valorant");
            garis();
            System.out.print("Masukan Pilihan Anda = ");
            jika = input.nextInt();
            if (jika == 1) {
                garis();
                mL();
            } else {
                garis();
                valo();
            }
            garis();
            System.out.println("Apakah anda ingin lanjut membeli?");
            System.out.print("(1. Ya/ 2. Tidak) : ");
            pilihan = input.nextInt();
        }
        while (pilihan == 1);
        garis();
        System.out.println(">>> Terimakasih sudah order <<<");
    }
    
    public static void garis() {
        int i; 
        for (i=0;i<20;i++) 
             System.out.print("--");
          System.out.println("");
        
    }
    
    public static void mL() {
        String nick;
        int id, server, bayar, p;
        String[] jumlah = new String[2];
        
        jumlah[0] = "100 Diamond";
        jumlah[1] = "257 Diamond";
        String[] pembayaran = new String[2];
        
        pembayaran[0] = "Cash";
        pembayaran[1] = "E-Wallet";
        double[] total = new double[2];
        
        total[0] = 30000;
        total[1] = 42000;
        System.out.println("Pricelist Mobile Legends : ");
        System.out.println("1. 100 Diamond Rp. 30.000");
        System.out.println("2. 257 Diamond Rp. 42.000");
        garis();
        System.out.print("Masukan pilihan anda : ");
        p = input.nextInt();
        if (p == 1) {
            garis();
            System.out.println("Nama Game : Mobile Legends ");
            System.out.print("Masukan Nick anda : ");
            nick = input.next();
            System.out.print("Masukan ID : ");
            id = input.nextInt();
            System.out.print("Masukan Server : ");
            server = input.nextInt();
            System.out.println("Metode Pembayaran yang tersedia : ");
            System.out.println("1.Cash");
            System.out.println("2.E-Wallet");
            System.out.print("Masukan pembayaran anda : ");
            bayar = input.nextInt();
            
            if (bayar == 1) {
                garis();
                System.out.print("Nick : ");
                System.out.println(nick);
                System.out.print("ID : ");
                System.out.println(id);
                System.out.print("Server : ");
                System.out.println(server);
                System.out.print("Jumlah Topup : ");
                System.out.println(jumlah[0]);
                System.out.print("Pembayaran melalui :  ");
                System.out.println(pembayaran[0]);
                System.out.print("Total yang harus dibayar : Rp.  ");
                System.out.println(total[0]);
            } else {
                garis();
                System.out.print("Nick : ");
                System.out.println(nick);
                System.out.print("ID : ");
                System.out.println(id);
                System.out.print("Server : ");
                System.out.println(server);
                System.out.print("Jumlah Topup : ");
                System.out.println(jumlah[0]);
                System.out.print("Pembayaran melalui : ");
                System.out.println(pembayaran[1]);
                System.out.print("Total yang harus dibayar : Rp.  ");
                System.out.println(total[0]);
            }
        } else {
            garis();
            System.out.println("Nama Game : Mobile Legends ");
            System.out.print("Masukan Nick anda : ");
            nick = input.next();
            System.out.print("Masukan ID : ");
            id = input.nextInt();
            System.out.print("Masukan Server : ");
            server = input.nextInt();
            System.out.println("Metode Pembayaran yang tersedia : ");
            System.out.println("1.Cash");
            System.out.println("2.E-Wallet");
            System.out.print("Masukan pembayaran anda : ");
            bayar = input.nextInt();
            if (bayar == 1) {
                garis();
                System.out.print("Nick : ");
                System.out.println(nick);
                System.out.print("ID : ");
                System.out.println(id);
                System.out.print("Server : ");
                System.out.println(server);
                System.out.print("Jumlah Topup : ");
                System.out.println(jumlah[1]);
                System.out.print("Pembayaran melalui :  ");
                System.out.println(pembayaran[0]);
                System.out.print("Total yang harus dibayar : Rp.  ");
                System.out.println(total[1]);
            } else {
                garis();
                System.out.print("Nick : ");
                System.out.println(nick);
                System.out.print("ID : ");
                System.out.println(id);
                System.out.print("Server : ");
                System.out.println(server);
                System.out.print("Jumlah Topup : ");
                System.out.println(jumlah[1]);
                System.out.print("Pembayaran melalui : ");
                System.out.println(pembayaran[1]);
                System.out.print("Total yang harus dibayar : Rp. ");
                System.out.println(total[1]);
            }
        }
    }
    
    public static void valo() {
        String nick, server;
        int id, p;
        int bayar;
        String[] pembayaran = new String[2];
        
        pembayaran[0] = "Cash";
        pembayaran[1] = "E-Wallet";
        String[] jumlah = new String[2];
        
        jumlah[0] = "200 Valorant Point";
        jumlah[1] = "360 Valorant Point";
        double[] total = new double[2];
        
        total[0] = 40000;
        total[1] = 55000;
        System.out.println( "Pricelist Valorant: ");
        System.out.println("1. 200 Vp Rp. 40.000");
        System.out.println("2. 360 Vp Rp. 55.000");
        garis();
        System.out.print("Masukan pilihan anda : ");
        p = input.nextInt();
        if (p == 1) {
            garis();
            System.out.println("Nama Game : Valorant");
            System.out.print("Masukan Riot ID : ");
            id = input.nextInt();
            System.out.print("Masukan Server : ");
            server = input.next();
            System.out.print("Masukan Nick Anda : ");
            nick = input.next();
            System.out.println("Metode Pembayaran yang tersedia : ");
            System.out.println("1.Cash");
            System.out.println("2.E-Wallet");
            System.out.print("Bayar melalui : ");
            bayar = input.nextInt();
            if (bayar == 1) {
                garis();
                System.out.print("Nick : ");
                System.out.println(nick);
                System.out.print("ID : ");
                System.out.println(id);
                System.out.print("Server : ");
                System.out.println(server);
                System.out.print("Jumlah Topup : ");
                System.out.println(jumlah[0]);
                System.out.print("Pembayaran melalui :  ");
                System.out.println(pembayaran[0]);
                System.out.print("Total yang harus dibayar : Rp.  ");
                System.out.println(total[0]);
            } else {
                System.out.print("Nick : ");
                System.out.println(nick);
                System.out.print("ID : ");
                System.out.println(id);
                System.out.print("Server : ");
                System.out.println(server);
                System.out.print("Jumlah Topup : ");
                System.out.println(jumlah[0]);
                System.out.print("Pembayaran melalui :  ");
                System.out.println(pembayaran[1]);
                System.out.print("Total yang harus dibayar : Rp.  ");
                System.out.println(total[0]);
            }
        } else {
            garis();
            System.out.println("Nama Game : Valorant");
            System.out.print("Masukan Riot ID : ");
            id = input.nextInt();
            System.out.print("Masukan Server : ");
            server = input.next();
            System.out.print("Masukan Nick Anda : ");
            nick = input.next();
            System.out.println("Metode Pembayaran yang tersedia : ");
            System.out.println("1.Cash");
            System.out.println("2.E-Wallet");
            System.out.print("Bayar melalui : ");
            bayar = input.nextInt();
            
            if (bayar == 1) {
                System.out.print("Nick : ");
                System.out.println(nick);
                System.out.print("ID : ");
                System.out.println(id);
                System.out.print("Server : ");
                System.out.println(server);
                System.out.print("Jumlah Topup : ");
                System.out.println(jumlah[1]);
                System.out.print("Pembayaran melalui :  ");
                System.out.println(pembayaran[0]);
                System.out.print("Total yang harus dibayar : Rp.  ");
                System.out.println(total[1]);
            } else {
                garis();
                System.out.print("Nick : ");
                System.out.println(nick);
                System.out.print("ID : ");
                System.out.println(id);
                System.out.print("Server : ");
                System.out.println(server);
                System.out.print("Jumlah Topup : ");
                System.out.println(jumlah[1]);
                System.out.print("Pembayaran melalui :  ");
                System.out.println(pembayaran[1]);
                System.out.print("Total yang harus dibayar : Rp.  ");
                System.out.println(total[1]);
            }
        }
    }
}
