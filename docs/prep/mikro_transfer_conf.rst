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
  * Uygulamanın sol menüsünü kullanarak Veritabanı sunucusu > Security > Logins adımlarını takip ediyoruz, Logins menü adımı üzerinde iken     farenin sağ tuşunu kullanarak işlem menüsünün gelmesini sağlıyoruz. Gelen menüden New Login seçeneğini seçiyoruz.
  * Yapılan seçim sonucu karşımıza gelen yeni kullanıcı tanımlama diyaloğunda entegrasyonda kulllanmak üzere yeni bir kullanıcı tanımı yapıyoruz. Genel sekmesinde kullanıcı doğrulama seçeneği olarak SQL Server autantication 'ı seçtikten sonra yeni bir kullanıcı adı ve şifresi belirliyoruz. Ardından User Mapping sekmesine geçerek ilgili kullanıcı için Mikro veritabanlarına db_owner yetkisi tanımlıyoruz. Diğer seçenekler varsayılan ayarlarında kalabilir, resimleri takip edebilirsiniz.
