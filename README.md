# İnternet Protokolü ve Alt Ağlara Ayırma: Herkes İçin Basit Bir Rehber

## Giriş: İnternet'in Gizli Dili ve Adresleri

Bugün hepimizin kullandığı ama arka planında işlerin nasıl yürüdüğünü bilmediği internetin aslında nasıl çalıştığını, cihazların birbirini nasıl tanıdığını ve bu dijital dünyayı düzenleyen kuralları konuşacağız.

**İnternet üzerinde bir web sitesine tıkladığınızda veriler size nasıl ulaşıyor?**

Bu makalede, internetin 'alfabesi' diyebileceğimiz **IP** ve ağları daha düzenli hale getiren **alt ağlara ayırma** (diğer adıyla *subnetting*) kavramlarından bahsedeceğiz.

## İnternet Nedir ve IP Nasıl Ortaya Çıktı?

### İnternet Nedir?

İnternet, dünya genelindeki bilgisayarların birbirine bağlı olduğu dev bir ağdır. Tıpkı şehirler arası yollar gibi, bu ağ da bilgilerin bir yerden bir yere gitmesini sağlar.

### Nasıl Ortaya Çıktı?

- 1960'lı yıllarda bilgisayarların birbiriyle iletişim kurabilmesi için bir yol arayışı başladı.
- Bilgi paylaşımını güvenli ve hızlı yapmak amacıyla çeşitli iletişim protokolleri geliştirildi.
- İnternet henüz yokken, bilgisayarlar genellikle tek başına çalışır, veri transferi fiziksel yollarla (örneğin manyetik bant ya da disketlerle) yapılırdı.
- Bu konuda ilk çalışmalar ARPA (İleri Düzey Araştırma Projeleri Ajansı) tarafından başlatıldı.
- 1969'da ARPANET projesi başlatıldı. Bu sistem,



internetin temelini oluşturan ilk geniş alan ağı (WAN) olarak kabul edilir.

  

### Protokol Ne Demek?

- Protokol, iki cihazın birbiriyle anlaşmasını sağlayan kurallar bütünüdür.
- Örneğin, SMTP (Simple Mail Transfer Protocol) e-posta sistemlerinin mesajı nasıl ileteceğini belirler.
- Eğer iki sistem aynı protokolü kullanmazsa, iletişim mümkün olmaz.

### IP Nasıl Ortaya Çıktı?

IP (Internet Protocol), verinin internet üzerinden nasıl ve nereye gideceğini belirleyen bir adresleme sistemidir.

## İnternet Fiziksel Bir Şey Mi? (TCP/IP'nin Büyük Resmi)

### İnternet Fiziksel Mi?

Evet! Fiber kablolar, Wi-Fi sinyalleri, uydular, veri merkezleri gibi fiziksel altyapılardan oluşur.

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
