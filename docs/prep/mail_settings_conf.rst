Mail Ayarları Yapılandırması
============================
Uygulama üzerinde yer alan bir takım işlemler (bilgilendirmeler, mutabakat sistemi, vs..) mail gönderimine ihtiyaç duymaktadır. ProWPS üzerinden mail gönderebilmek için yapmanız gereken ayarlamalar ise şöyle:

  * ProWPS dizininde yer alan prowps_server klasörünü açıyoruz.
  * livserver.exe.config isimli dosyayı notepad ile açıyoruz.
  * appSettings içinde yer alan "smtp" ile başlayan parametreleri girip, dosyayı kaydediyoruz.

Bu işlemler sonrası sunucu uygulamayı yeniden çalıştırdığınızda mail ayarlarınız geçerli olacaktır.
