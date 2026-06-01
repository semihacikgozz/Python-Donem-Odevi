# Python Programlama Dönem Sonu Ödevi 🐍

Proje yönergelere uygun olarak iki temel kısımdan oluşuyor:

### 1. Kısım: Veri Yapıları ve Temel Mantık
İlk aşamada sadece tek bir müşterinin profili üzerinden temel yapıları kullandım.
* Müşteri bilgilerini alt alta listelemek yerine bir Sözlük (Dictionary) içinde topladım. Böylece verilere indeks numaralarıyla değil, `ad_soyad` veya `aylik_ucret` gibi daha anlaşılır isimlerle erişebildim.
* İf-Else bloklarıyla müşterinin faturasına ve sadakat ayına (bizde kaldığı süreye) bakarak "VIP Müşteri" olup olmadığına karar verdiren bir yapı kurdum.
* Son olarak `random` kütüphanesiyle her müşteriye özel rastgele bir ID ürettim.

### 2. Kısım: Fonksiyonlar, Döngüler ve Kütüphaneler
Burada işi biraz daha büyüterek birden fazla müşteriyi sisteme dahil ettim.
* 5 farklı müşteriyi ana bir liste içinde sözlükler (dictionary) halinde tuttum.
* `for` döngüsü ile bu listede gezerek her müşterinin faturasına KDV ekleyen ayrı bir fonksiyon çağırdım.
* **Churn (Ayrılma) Riski Tespiti:** Döngü içine ufak bir mantık ekledim. Eğer müşteri aktif değilse veya 6 aydan daha kısa süredir aboneyse, iptal ihtimali yüksek olduğu için bu müşterileri "Yüksek Churn Riskli" olarak işaretledim.
* `math` kütüphanesiyle küsuratlı fatura tutarlarını yuvarlayıp, `datetime` ile günün tarihini çektim. 
* Son olarak şirket hizmetlerindeki tekrar eden kayıtları temizlemek için `set()` metodunu kullandım.

** Semih Açıkgöz
