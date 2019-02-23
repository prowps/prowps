
Sevkiyat İşlemleri
===================

Programda yer alan Tedarikçi Uygulamaları > Sevkiyat İşlemleri menü adımı ile ilgili uygulamaya erişilebilir.

.. image:: img/shipping_operation_1.png
   :align: center
   
Uygulama başlatıldığında ekranın ortadan ikiye bölündüğünü göreceksiniz. Ekranın üst bölümü açık siparişlerinizi listeyelecek ve sevkiyata konu olan kalemleri seçmenizi sağlayacak , ekranın alt bölümü ile ilgili sevk belgesi için üzerinde çalıştığınız kalemleri gösterecek. İki bölme arasında ve ekranın en altında kalan fonksiyonel butonlar vasıtası ilede işlemlerimizi yapıyor olacağız.

Bu uygulama üzerinden gerçekleşen veya planlanan sevkiyat bilgilerini sisteme dahil edebilirsiniz. İşlem yapabilmek için irsaliye yada sevk numarası girişi gerekmektedir. Eğer planlanan bir sevkiyat düzenliyorsanız buraya önceden ayırdığınız irsaliye numarasını girebilirsiniz.

İşlem adımları:

1. Açık kalemler listesinden sevkiyata konu olan kalemlerin seçimi
2. Kutu ve palet barkodlarının düzenlenmesi
3. İrsaliye numrası girilerek sevk belgelerinin sisteme kaydı
4. **Asn çekimi**

Şimdi sırasıyla bu işlemlerin nasıl yapıldığını inceleyelim.

**1. Açık kalemler listesinden sevkiyata konu olan kalemlerin seçimi**

Giriş bölümünde ekranı üst/alt olacak şekilde iki gruba ayırmıştık. Bu bölümde üst grupta yer alan tablo vasıtasıyla sevkiyata konu olacak sipariş kalemlerini seçip alt gruba ekliyor olacağız.

.. image:: img/shipping_operation_2.png
   :align: center
   
Üst grupta bulunan tabloda işlem yapılacak satır seçili hale getirildikten sonra tablonun sonunda yer alan "Paket Tipi", "Paket İçi Miktar" ve "İşlem Miktarı" alanları doldurulur. Öncelikli olarak "Sağlayıcı" tarafından tanımlanmış paketleme tiplerinden birini seçerek işe başlıyoruz, paketleme tipi seçimi sonrası sistemde tanımlı paket içi miktar bilgisi tabloya eklenecek bizlerde son olarak işlem miktarını sistemin izin verdiği boyutta (sipariş açık miktarını aşmayacak şekilde) giriyor olacağız.

Bu üst grupta tüm giriş işlemlerini bitirdikten sonra "Yeni sevk referansı" numarasını giriyor ve "Paket Oluştur" yada "Karma Paket Oluştur" butonunu kullanarak seçimlerimizi alt gruba ekliyoruz.

:Paket: Aynı kodlu ürünlerin girdiği paketleme tipi
:Karma Paket: Farklı kodlu ürünlerin girebileceği paketleme tipi

**2. Kutu ve palet barkodlarının düzenlenmesi**

Üst grup yapılan seçimler alt gruba eklendiği esnada sistem üst grupta seçimi yapılan paketlerin her biri için paket barkodlarını oluşturacaktır. Alt grupta sevk belgesi kaydı öncesi Palet barkodu oluşturma opsiyonu sunulmaktadır.

Bu işlem için alt grup tablo üzerinden paletlenen kalemlerin seçimi yapıldıktan sonra "Palet barkod" butonuna basılır, gelen seçim ekranından Palet kodu seçilerek sistemin seçilen satırlar için barkod üretmesi sağlanabilir.

**3. İrsaliye numrası girilerek sevk belgelerinin sisteme kaydı**

Barkod düzenlemeleri sonrası irsaliye (sevk belge) numarası girilerek belgenin sisteme kaydı sağlanır. Önceden kaydedilmiş bir belge orta barda yer alan sevk belge no kutucuğuna irsaliye numarası girilerek ekrana alınabilir. Bu kayıtlı belge üzerinde yeni sipariş kalemi eklemi , palet barkod düzenleme ve yeniden kayıt işlemleri yapılabilir.

Tüm işlemler tamamlandıktan sonra ekranın alt barında yer alan barkod üret butonları ile kutu ve palet barkodları oluşturularak fiziksel ortamda ürünlerin bu barkodlarla etiketlenmesi sağlanır.

**4. Asn çekimi**

Detayları kendi uygulama konu başlığı altında anlatılacak olan uygulama hakkında özet bilgi vermek gerekirse, sisteme kaydı yapılmış olan sevk belgesi üzerinden Sağlayıcıya asn çekiminde kullanılan ekrandır diyebiliriz.

Sağlayıcının tercihine bağlı olarak belirlenen asn dosya formatı konusunda müdahale şansınız bulunmamaktadır. Sisteme dahil ettiğiniz sevk belgelerini Sağlayıcının tercihine bağlı asn formatında kapalı ortamda gönderdiğiniz uygulamadır.
