Mikro Aktarım Yapılandırması
============================
PROWPS programımı üzerinde yer alan "Mikro Veri Aktarım Şemaları" kullanılarak Mikro veritabanından portal için gerekli olan verileri çekebilmek mümkündür.

Veri aktarım işlemi için birkaç ön kurulum adımını yerine getirmek gerekecektir. Bunlar:

Mikro veritabanı üzerinde bir kullanıcı tanımlamak.
Mikro veritabanına ağ üzerinden erişimi aktive etmek.
PROWPS üzerinde Mikro veritabanı erişim bilgilerini tanımlamak.

Şimdi üstte yer alan adımların üzerinden sırasıyla geçerek PROWPS' in Mikro veritabanına erişiminin nasıl sağlanacağını öğrenelim.

**1. Mikro veritabanı üzerinde bir kullanıcı tanımlamak**

  * Mikronun kurulu bulunduğu sunucu makinada Microsoft SQL Server Management Studio uygulamasını başlatıyoruz.
  * Uygulamanın sol menüsünü kullanarak Veritabanı sunucusu > Security > Logins adımlarını takip ediyoruz, Logins menü adımı üzerinde iken farenin sağ tuşunu kullanarak işlem menüsünün gelmesini sağlıyoruz. Gelen menüden New Login seçeneğini seçiyoruz.
  * Yapılan seçim sonucu karşımıza gelen yeni kullanıcı tanımlama diyaloğunda entegrasyonda kulllanmak üzere yeni bir kullanıcı tanımı yapıyoruz. Genel sekmesinde kullanıcı doğrulama seçeneği olarak SQL Server autantication 'ı seçtikten sonra yeni bir kullanıcı adı ve şifresi belirliyoruz. Ardından User Mapping sekmesine geçerek ilgili kullanıcı için Mikro veritabanlarına db_owner yetkisi tanımlıyoruz. Diğer seçenekler varsayılan ayarlarında kalabilir, resimleri takip edebilirsiniz.
  
  .. image:: img/mssql_int_1.png
     :align: center
  .. image:: img/mssql_int_2.png
     :align: center  
  .. image:: img/mssql_int_3.png
     :align: center  
  
**2. Mikro veritabanına ağ üzerinden erişimi aktive etmek**

  * Yine Mikronun kurulu bulunduğu sunucu makinada SQL Server Configuration Manager uygulamasını başlatıyoruz.
  * Uygulamanın sol menüsünü kullanarak SQL Server Network Configuration > Protocols for .. adımlarını takip ediyoruz. İlgili menü adımının seçimi ardından sağ tarafta beliren listede yer alan TCP/IP seçeneğinin üzerini çift tıklıyoruz. Gelen diyalog üzerinde Protocol sekmesinde yer alan Enabled opsiyonunu Yes yaptıktan sonra IP Addresses sekmesine geçerek TCP Port seçeneklerinin tümüne 1433 yazıyoruz. Ardından Uygula butonu ile diyalog dan çıkıyoruz.
  * Son olarak yine aynı uygulama üzerinde sol menüden SQL Server Services seçimine bağlı sağ tarafta açılan liste üzerinde SQL Server servisini sağ tıklayarak yeniden başlatıyoruz.
  
  .. image:: img/mssql_int_4.png
  
  .. image:: img/mssql_int_5.png
  
  .. image:: img/mssql_int_6.png  
  
  .. image:: img/mssql_int_7.png
  
**3. PROWPS üzerinde Mikro veritabanı erişim bilgilerini tanımlamak**

  * PROWPS sunucu programının bulunduğu klasörde (prowps_server) yer alan livserver.exe.config isimli dosyayı metin editörü ile açıyoruz.
  * Dosya içerisinde configuration > connectionStrings tag'i altında yer alan mssql, connectionString parametresini mikro kurulumuna uygun şekilde ayalıyoruz. İlgili parametre değerinde sunulan örnek ifade: Server=[IPADRESS],[PORT];Network Library=DBMSSOCN;Database=[DATABASE];User Id=[USERNAME];Password=[PASSWORD]; şeklindedir. Bu ifadede köşeli parantezler içine doğru değerler vererek dosyayı kaydediyoruz.
