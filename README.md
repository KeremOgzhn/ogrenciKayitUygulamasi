# Öğrenci Kayıt Uygulaması / Student Registration Application

## Türkçe

### Proje Açıklaması
Bu proje, öğrenci bilgilerini kaydetmek, güncellemek, silmek ve sorgulamak için geliştirilmiş bir Windows Forms uygulamasıdır. C# programlama dili kullanılarak geliştirilmiş olup, SQL Server veritabanı ile çalışmaktadır.

### Özellikler
- 🔐 **Kullanıcı Girişi**: Güvenli giriş sistemi
- ➕ **Öğrenci Kayıt**: Yeni öğrenci bilgilerini sisteme ekleme
- 📋 **Öğrenci Listeleme**: Tüm öğrenci bilgilerini görüntüleme
- 🔍 **Öğrenci Arama**: Öğrenci numarasına göre arama yapma
- 🗑️ **Öğrenci Silme**: Mevcut öğrenci kayıtlarını silme
- 🏆 **En Yüksek Ortalama**: En yüksek ortalamaya sahip öğrenciyi bulma
- 📊 **Ders Yönetimi**: Ders bilgilerini yönetme

### Teknik Gereksinimler
- **Framework**: .NET Framework 4.8
- **IDE**: Visual Studio 2015 veya üzeri
- **Veritabanı**: SQL Server (LocalDB veya SQL Server Express)
- **Platform**: Windows

### Kurulum

#### 1. Projeyi İndirin
```bash
git clone https://github.com/KeremOgzhn/ogrenciKayitUygulamasi.git
cd ogrenciKayitUygulamasi
```

#### 2. Veritabanı Kurulumu
1. SQL Server Management Studio'yu açın
2. `veri tabanı/dbOgrenciKayit.sql` dosyasını çalıştırın
3. Bu işlem `dbOgrenciKayit` veritabanını oluşturacak ve örnek verilerle dolduracaktır

#### 3. Bağlantı Dizesini Kontrol Edin
Proje dosyalarında bulunan bağlantı dizesi:
```csharp
@"server = . ; initial catalog= dbOgrenciKayit; integrated security = true"
```

#### 4. Projeyi Çalıştırın
1. `ogrenciKayitUygulamasi.sln` dosyasını Visual Studio ile açın
2. Projeyi derleyin (Build → Build Solution)
3. F5 tuşuna basarak uygulamayı çalıştırın

### Kullanım

#### Giriş Bilgileri
Uygulama varsayılan olarak aşağıdaki kullanıcı hesapları ile gelir:
- **Kullanıcı Adı**: KeremOgzhn, **Şifre**: parola123
- **Kullanıcı Adı**: ahmet_y, **Şifre**: sifre456
- **Kullanıcı Adı**: zeynep_k, **Şifre**: gucluSifre!
- **Kullanıcı Adı**: ogretmen, **Şifre**: test1234
- **Kullanıcı Adı**: misafir, **Şifre**: 98765

#### Ana Menü Fonksiyonları
1. **Öğrenci Kayıt**: Yeni öğrenci ekleme formu
2. **Öğrenci Listele**: Tüm öğrencileri görüntüleme
3. **Öğrenci Sil**: Öğrenci numarasına göre silme işlemi
4. **Öğrenci Bul**: Öğrenci arama işlemi
5. **En Yüksek Ortalama**: En başarılı öğrenciyi bulma

### Veritabanı Yapısı

#### Tablolar
1. **login**: Kullanıcı giriş bilgileri
   - ID (Primary Key)
   - kullaniciAdi (varchar)
   - parola (varchar)

2. **tblDers**: Ders bilgileri
   - dersKodu (Primary Key)
   - dersAdi (varchar)

3. **tblOgrenci**: Öğrenci bilgileri
   - ogrNo (Primary Key)
   - ad (varchar)
   - soyad (varchar)
   - dogumTarih (date)
   - adres (varchar)
   - telefon (varchar)
   - dersID (Foreign Key)
   - Ortalama (int)

### Katkıda Bulunma
1. Bu repository'yi fork edin
2. Yeni bir branch oluşturun (`git checkout -b feature/yeniOzellik`)
3. Değişikliklerinizi commit edin (`git commit -am 'Yeni özellik eklendi'`)
4. Branch'inizi push edin (`git push origin feature/yeniOzellik`)
5. Pull Request oluşturun

### Lisans
Bu proje MIT lisansı altında lisanslanmıştır.

---

## English

### Project Description
This is a Windows Forms application developed for managing student information including registration, updating, deletion, and querying. Built with C# programming language and uses SQL Server database.

### Features
- 🔐 **User Authentication**: Secure login system
- ➕ **Student Registration**: Add new student information to the system
- 📋 **Student Listing**: View all student information
- 🔍 **Student Search**: Search by student number
- 🗑️ **Student Deletion**: Delete existing student records
- 🏆 **Highest Average**: Find student with highest grade average
- 📊 **Course Management**: Manage course information

### Technical Requirements
- **Framework**: .NET Framework 4.8
- **IDE**: Visual Studio 2015 or higher
- **Database**: SQL Server (LocalDB or SQL Server Express)
- **Platform**: Windows

### Installation

#### 1. Clone the Project
```bash
git clone https://github.com/KeremOgzhn/ogrenciKayitUygulamasi.git
cd ogrenciKayitUygulamasi
```

#### 2. Database Setup
1. Open SQL Server Management Studio
2. Execute the `veri tabanı/dbOgrenciKayit.sql` file
3. This will create the `dbOgrenciKayit` database and populate it with sample data

#### 3. Check Connection String
The connection string used in project files:
```csharp
@"server = . ; initial catalog= dbOgrenciKayit; integrated security = true"
```

#### 4. Run the Project
1. Open `ogrenciKayitUygulamasi.sln` with Visual Studio
2. Build the project (Build → Build Solution)
3. Press F5 to run the application

### Usage

#### Login Credentials
The application comes with the following default user accounts:
- **Username**: KeremOgzhn, **Password**: parola123
- **Username**: ahmet_y, **Password**: sifre456
- **Username**: zeynep_k, **Password**: gucluSifre!
- **Username**: ogretmen, **Password**: test1234
- **Username**: misafir, **Password**: 98765

#### Main Menu Functions
1. **Student Registration**: Form for adding new students
2. **List Students**: Display all students
3. **Delete Student**: Delete by student number
4. **Find Student**: Search for students
5. **Highest Average**: Find the most successful student

### Database Structure

#### Tables
1. **login**: User authentication information
   - ID (Primary Key)
   - kullaniciAdi (varchar)
   - parola (varchar)

2. **tblDers**: Course information
   - dersKodu (Primary Key)
   - dersAdi (varchar)

3. **tblOgrenci**: Student information
   - ogrNo (Primary Key)
   - ad (varchar)
   - soyad (varchar)
   - dogumTarih (date)
   - adres (varchar)
   - telefon (varchar)
   - dersID (Foreign Key)
   - Ortalama (int)

### Contributing
1. Fork this repository
2. Create a new branch (`git checkout -b feature/newFeature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/newFeature`)
5. Create a Pull Request

### License
This project is licensed under the MIT License.

---

## Ekran Görüntüleri / Screenshots

*Uygulama ekran görüntüleri burada yer alacaktır.*  
*Application screenshots will be placed here.*

## İletişim / Contact

Proje geliştiricisi: [@KeremOgzhn](https://github.com/KeremOgzhn)

---

**Not**: Bu uygulama eğitim amaçlı geliştirilmiştir.  
**Note**: This application was developed for educational purposes.