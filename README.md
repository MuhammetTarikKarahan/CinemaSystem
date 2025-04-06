CinemaSystem Proje Aşamaları

Proje Konusu:
Konsolda çalışan, kullanıcıların film ve müşteri bilgilerini yönetebileceği bir Sinema Sistemi geliştirilmesi.

1. Proje Yapısının Planlanması
- Sistem içinde Film, Müşteri ve Bilet kavramlarının olması gerektiği belirlendi.
- Kullanıcıdan seçim almak için menü tabanlı bir arayüz oluşturulmasına karar verildi.
- Verilerin sadece program çalışırken tutulacağı (kalıcı veri saklamanın olmayacağı) not edildi.

2. Sınıf ve Değişkenlerin Tanımlanması
- CinemaSystem adında bir ana sınıf oluşturuldu.
- Filmler, müşteriler ve biletler için dizi (array) yapıları tanımlandı:
  - Film[] films = new Film[10];
  - Customer[] customers = new Customer[20];
  - Ticket[] tickets = new Ticket[50];
- Her kategori için sayaç değişkenleri (filmCount, customerCount, ticketCount) oluşturuldu.

3. Menü Sistemi Kurulması
- Sonsuz bir döngü (while (true)) içerisinde kullanıcıya her seferinde bir seçim menüsü sunuldu.
- Kullanıcının seçimine göre ilgili işlemler yapılacak şekilde switch yapısı kullanıldı.

4. Film Ekleme Özelliği
- Kullanıcıdan film bilgileri (film adı, süre, tür) alındı.
- Yeni bir Film nesnesi oluşturularak films dizisine eklendi.
- filmCount değişkeni artırıldı.

5. Müşteri Ekleme Özelliği
- Kullanıcıdan müşteri bilgileri (isim, email) alındı.
- Yeni bir Customer nesnesi oluşturularak customers dizisine eklendi.
- customerCount değişkeni artırıldı.

6. Bilet Oluşturma Özelliği
- Kullanıcıya mevcut müşteriler ve filmler listelendi.
- Kullanıcıdan, hangi müşteri için hangi filme bilet oluşturmak istediği seçmesi istendi.
- Seçilen müşteri ve film bilgileri kullanılarak bir Ticket nesnesi oluşturuldu ve tickets dizisine eklendi.
- ticketCount değişkeni artırıldı.

7. Listeleme Özellikleri
- Kullanıcı Filmleri Listele seçeneğini seçerse:
  - films dizisi üzerinde döngü ile ilerlenerek tüm filmler ekrana yazdırıldı.
- Kullanıcı Müşterileri Listele seçerse:
  - customers dizisi üzerinde döngü ile ilerlenerek tüm müşteriler ekrana yazdırıldı.
- Kullanıcı Biletleri Listele seçerse:
  - tickets dizisi üzerinde döngü ile ilerlenerek tüm biletler (müşteri ismi + film adı) ekrana yazdırıldı.

8. Çıkış Özelliği
- Kullanıcı 0 seçerse program "Çıkılıyor..." mesajı göstererek break ile döngüyü kırdı ve uygulama sonlandırıldı.

9. Hata Yönetimi
- Yanlış seçim yapıldığında kullanıcıya "Geçersiz seçim" uyarısı verildi.
- Film veya müşteri eklenmeden bilet oluşturulmak istenirse hata oluşmasını engellemek için kontroller eklendi.

Sonuç
Bu proje ile:
- Java'da sınıf, nesne, dizi, döngü ve koşullu ifadeler kullanımı tekrar edilmiş oldu.
- Konsolda çalışan bir menü tabanlı uygulama geliştirildi.
- Kullanıcı etkileşimi ve temel veri yönetimi sağlandı.
