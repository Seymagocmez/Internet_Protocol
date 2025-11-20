# İnternet Protokolü (IP)

## Giriş: İnternetin Dili ve Adresleri

Bu makalede, internetin 'alfabesi' diyebileceğimiz **IP** ve ağları daha düzenli hale getiren **alt ağlara ayırma** (diğer adıyla *subnetting*) kavramlarından bahsedeceğiz.

### İnternet Nedir?

İnternet, dünya genelindeki bilgisayarların birbirine bağlı olduğu dev bir ağdır. Tıpkı şehirler arası yollar gibi, bu ağ da bilgilerin bir yerden bir yere gitmesini sağlar.Bu cihazların birbirlerini bulup veri alışverişi yapabilmesi için ortak bir dil ve adresleme sistemi gereklidir. İşte burada IP devreye girer.  Her cihazın kendine özgü bir adresi vardır ve bu adresler üzerinden veriler yönlendirilir.

Tanımından dolayı her ne kadar soyut bir kavram olarak algılansa da İnternet aslında fiber optik kablolar, uydu bağlantıları, Wi-Fi sinyalleri, veri merkezleri ve yönlendiriciler gibi birçok fiziksel bileşenden oluşur.

### Nasıl Ortaya Çıktı?

- 1960'lı yıllarda bilgisayarların birbiriyle iletişim kurabilmesi için bir yol arayışı başladı.
- Bilgi paylaşımını güvenli ve hızlı yapmak amacıyla çeşitli iletişim protokolleri geliştirildi.
- İnternet henüz yokken, bilgisayarlar genellikle tek başına çalışır, veri transferi fiziksel yollarla (örneğin manyetik bant ya da disketlerle) yapılırdı.
- Bu konuda ilk çalışmalar ARPA (İleri Düzey Araştırma Projeleri Ajansı) tarafından başlatıldı.
- 1969'da ARPANET projesi başlatıldı. Bu sistem,

internetin temelini oluşturan ilk geniş alan ağı (WAN) olarak kabul edilir.

  ## İnternet üzerinde bir web sitesine tıkladığınızda, veriler size nasıl ulaşıyor?

<div align="center">
  <img src="https://github.com/user-attachments/assets/dcfffaf0-ef6e-472e-9f11-c7d44397a857" alt="Kaynak görsel" width="600"/>
  <p><em>Kaynak: <a href="https://mocomi.com/how-the-internet-works/">https://mocomi.com/how-the-internet-works/</a> (Çevrildi)</em></p>
</div>

1. Tarayıcınıza www.example.com yazdığınızda, cihazınız önce DNS (Domain Name System) sunucularına sorgu gönderir ve ziyaret etmek istediğiniz sitenin alan adını, IP adresine çevirir. Örneğin, www.example.com → 93.184.216.34.
2. Bu IP adresi, sitenin sunucusunun internet üzerindeki konumudur. Daha sonra, internet servis sağlayıcınız (ISP) aracılığıyla veri paketleri, yönlendiriciler ve anahtarlar gibi ağ donanımları üzerinden bu IP adresine doğru yol alır.
3. İstek, birçok ağ geçidinden geçerek hedef sunucuya ulaşır.  
4.  Sunucu, talep edilen web sayfasının verilerini paketler halinde cihazınıza geri gönderir. 
5. Bu veri yolculuğu saniyenin çok küçük bir kısmında gerçekleşir ve veriler cihazınıza ulaştığında tarayıcınız sayfayı görüntüler.

### Protokol Ne Demek?

- Protokol, iki cihazın birbiriyle anlaşmasını sağlayan kurallar bütünüdür.
- Örneğin, SMTP (Simple Mail Transfer Protocol) e-posta sistemlerinin mesajı nasıl ileteceğini belirler.
- Eğer iki cihaz aynı protokolü kullanmıyorsa, iletişim kurulamaz.

### IP Nasıl Ortaya Çıktı?

IP (Internet Protocol), verinin internet üzerinden nasıl ve nereye gideceğini belirleyen bir adresleme sistemidir.


### Katmanlı Yapı: TCP/IP

Bu yapı 4 katmandan oluşur:

1. **Fiziksel Katman**: Kablolar, modemler, router'lar.
2. **İnternet Katmanı (IP)**: Paket yönlendirme.
3. **Taşıma Katmanı (TCP/UDP)**:
   - **TCP**: Güvenli, hataya dayanıklı (web, banka vs.)
   - **UDP**: Hızlı, kontrolsüz (video, oyun vs.)
4. **Uygulama Katmanı**: Web tarayıcıları, e-posta, mesajlaşma.

## IP Adresi: Cihazınızın İnternet'teki Ev Numarası

### IP Adresi Nedir?

İnternete bağlanan her cihazın sahip olduğu benzersiz bir kimlik numarasıdır.

### Kim Veriyor?

İnternet servis sağlayıcınız (ISS) veya yerel ağdaki yönlendirici (router).

### DNS’in Rolü

DNS (Domain Name System), `google.com` gibi adları IP adreslerine çevirir.  
İnsanlar için hatırlaması kolay, makineler için anlaşılır.

### IP Adresi ve Alan Adı Arasındaki İlişki

Eğer bir bilgisayara mesaj göndermek istiyorsanız, **hangi bilgisayar** olduğunu belirtmeniz gerekir.  
Bu nedenle, bir ağa bağlı olan her bilgisayarın kendine ait **benzersiz bir adresi** vardır.  
Bu adrese **IP adresi** denir (IP, *Internet Protocol* yani İnternet Protokolü anlamına gelir).

IP adresi, noktalı dört sayıdan oluşur:

```text
Örnek: 192.0.2.172

```

### Kaynaklar

https://www.cisco.com/c/en/us/support/docs/ip/routing-information-protocol-rip/13788-3.html

https://www.internetsociety.org/internet/history-internet/brief-history-internet/

https://learn.microsoft.com/en-us/previous-versions/windows/it-pro/windows-2000-server/cc940061(v=technet.10)

https://www.cloudflare.com/learning/dns/what-is-dns/

https://www.ibm.com/topics/ip-address

https://mocomi.com/how-the-internet-works/
