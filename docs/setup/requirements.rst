Sistem Gereksinimleri
=====================

Uygulamada temelde 3 bileşenden oluşmaktadır. Bunlar:

1. Sunucu programı
2. İstemci programı
3. Veri tabanı

Uygulamanın çalışabilmesi için bu 3 bileşeninde konfigüre edilerek çalışır hale getirilmesi gerekmektedir.

Sunucu ve İstemci uygulamalar dotnet uygulamalarıdır, ve çalışabilmek için sisteminizde dotnet framework' ün yüklü olması gerekir. Veri tabanı konusunda ise uygulamamız veri tabanı bağımsız çalışmaktadır, tercih ettiğiniz veri tabanı sistemini konfigüre ettikten sonra birkaç küçük ayarlama yaparak uygulamayı aktive edebilirsiniz.

Sitemiz üzerinden dağıtılan çalıştırılabilir paketlerimizde Sqlite veri tabanı sistemi tercih edilmiştir. Bu veri tabanı sisteminin sağladığı avantajlar ise kullanıcı tarafından herhangi bir konfigürasyona ihtiyaç duyulmaması ve taşınabilir olmasıdır. Tabiki kullanıcıların bu veri tabanı sistemi dışında farklı bir sistemi kullanma şanslarıda her zaman bulunmaktadır.

Özetlersek:

1. LivServer Sunucu Programı ( Windows için dotnet framework / Linux, Mac için Mono Framework )
2. LivClient İstemci programı ( Web sunucuya ihtiyaç duymaktadır. Kurulum paketinde Windows için "cassini", Linux, Mac için "xsp" sunucu konfigure edilmiştir. )
3. Veritabanı ( default Sqlite, diğer veritabanı sistemleri tercihe bağlı )

Notlar:
Çalıştırılabilir paketimizi sorunsuz kullanmak için dotnet framework 4.5' i yüklemelisiniz.
Sunucu, Client uygulamamız Mono framework ile Linux üzerinde test edilmiştir.
