# Öğrenci Kayıt Uygulaması

Bu proje, C# Windows Forms ve MS SQL Server veritabanı kullanılarak geliştirilmiş bir öğrenci kayıt sistemidir.

## Proje Hakkında

Uygulama, öğrencilerin kişisel bilgilerini, ders kayıtlarını ve notlarını yönetmek için tasarlanmış bir masaüstü yazılımıdır. Temel CRUD (Create, Read, Update, Delete) işlemlerini içerir.

## Kullanılan Teknolojiler

*   **Arayüz:** C# Windows Forms (.NET Framework)
*   **Veritabanı:** Microsoft SQL Server

## Kurulum ve Başlangıç

Projeyi yerel makinenizde çalıştırmak için aşağıdaki adımları izleyebilirsiniz:

1.  **Repoyu Klonlayın:**
    ```sh
    git clone https://github.com/KeremOgzhn/ogrenciKayitUygulamasi.git
    ```

2.  **Veritabanını Ayarlayın:**
    - Proje dosyaları arasında bulunan `.sql` script'ini kullanarak veritabanını ve ilgili tabloları oluşturun.
    - `app.config` dosyasındaki veritabanı bağlantı cümlenizi (`connectionString`) kendi MS SQL Server yapılandırmanıza göre güncelleyin.

3.  **Projeyi Çalıştırın:**
    - `ogrenciKayitUygulamasi.sln` çözüm dosyasını Visual Studio ile açın.
    - Projeyi derleyin ve başlatın.

## Katkıda Bulunma

Projeye katkıda bulunmak isterseniz, lütfen bir "issue" açın veya "pull request" gönderin.

## Yazar

*   **KeremOgzhn** - *Proje Sahibi* - [KeremOgzhn](https://github.com/KeremOgzhn)
