# praktikum4 inheritance
```
NAMA    : HABIB SUPRAYOGA
NIM     : 312310608
KELAS   : TI.23.A6
MATKUL  : Pemrograman Orientasi Objek
```

## Latihan
-   Buat kode java mendeklarasikan class Person dengan atribut Nama, JenisKelamin, Umur. Lengkap dengan access modifier nya.
-   Lalu buat objek class person bernama Anton & Riko.
-   Lengkapi latihan class
    Mahasiswa dengan setter dan getter.
-   implementasikan java
    code diagram class dengan materi yang ada di ecampus

  ### Class java
  - kelas induk
 ```
public class Pegawai {
    private String nama;
    private double gajiPokok; 
 ```
    Pengatur untuk nama
    public void setNama(String nama) {
        this.nama = nama;
    }
    
    Pengambil untuk nama
    public String getNama() {
        return nama;
    }
    
     Pengatur untuk gajiPokok
    public void setGajiPokok(double gajiPokok) {
        this.gajiPokok = gajiPokok;
    }
    
    Pengambil untuk gajiPokok
    public double getGajiPokok() {
        return gajiPokok;
    }
    
     Method untuk mencetak informasi
    public void cetakInfo() {
        System.out.println("Nama: " + nama);
        System.out.println("Gaji Pokok: " + gajiPokok);
    }


Kelas Manager mewarisi dari Pegawai
```
public class Manager extends Pegawai {
    private double tunjangan; 
    
    Pengatur untuk tunjangan
    public void setTunjangan(double tunjangan) {
        this.tunjangan = tunjangan;
    }
    
    Pengambil untuk tunjangan
    public double getTunjangan() {
        return tunjangan;
    }
    
    Override cetakInfo untuk menambahkan tunjangan
    @Override
    public void cetakInfo() {
        super.cetakInfo();
        System.out.println("Tunjangan: " + tunjangan);
    }
    
    Method untuk mencetak tunjangan
    public void cetakTunjangan() {
        System.out.println("Tunjangan Manager: " + tunjangan);
    }


 Kelas Programmer mewarisi dari Pegawai
public class Programmer extends Pegawai {
    private double bonus; 
    
    Pengatur untuk bonus
    public void setBonus(double bonus) {
        this.bonus = bonus;
    }
    
    Pengambil untuk bonus
    public double getBonus() {
        return bonus;
    }
    
   Override cetakInfo untuk menambahkan bonus
    @Override
    public void cetakInfo() {
        super.cetakInfo();
        System.out.println("Bonus: " + bonus); 
    
    
    Method untuk mencetak bonus
    public void cetakBonus() {
        System.out.println("Bonus Programmer: " + bonus);
    }


```

Berikut adalah penjelasan implementasinya :

1. Kelas `Pegawai`:
   - Berisi informasi dasar pegawai (nama dan gajiPokok)
   - Memiliki pengatur (setter) dan pengambil (getter) untuk semua field
   - Memiliki method `cetakInfo()` untuk mencetak informasi pegawai

2. Kelas `Manager`:
   - Mewarisi dari kelas `Pegawai`
   - Menambahkan field tunjangan dengan pengatur dan pengambil
   - Menimpa (override) method `cetakInfo()` untuk menambahkan informasi tunjangan
   - Menambahkan method `cetakTunjangan()` untuk mencetak khusus tunjangan

3. Kelas `Programmer`:
   - Mewarisi dari kelas `Pegawai`
   - Menambahkan field bonus dengan pengatur dan pengambil
   - Menimpa (override) method `cetakInfo()` untuk menambahkan informasi bonus
   - Menambahkan method `cetakBonus()` untuk mencetak khusus bonus

  Berikut adalah Hasil dari code program diatas :
  ![alt text](https://github.com/Habibsuprayoga325/Inheritance/blob/main/ss1.png?raw=true)
![alt text](https://github.com/Habibsuprayoga325/Inheritance/blob/main/ss2.png?raw=true)
 ![alt text](https://github.com/Habibsuprayoga325/Inheritance/blob/main/ss3.png?raw=true)
![alt text](https://github.com/Habibsuprayoga325/Inheritance/blob/main/ss4.png?raw=true)
