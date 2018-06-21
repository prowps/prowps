Geliştirme Ortamı
=================
Uygulama tasarım aracı olan "livdevelop" python programlama dili kullanılarak geliştirilmektedir. Uygulamayı çalıştırabilmek için sisteminizde python3 programı ile beraber gtksourceview ve lxml komponentlerininde yüklü olması gerekmektedir. Livdevelop programımızın arayüz tasarımında Gtk3 kullanılmaktadır.

Birçok Linux dağıtımda python3 ve gtk3 programları kurulu olarak gelmektedir. Linux kullanıcıları sistemlerinde iki ana programın haricinde gtksourceview ve lxml python kütüphanelerinin de kurulu olduğundan emin olduktan sonra kurulum paketinden çıkan kısayolu başlatarak geliştirme ortamına erişebilirler.

Windows kullanıcıları ise sırasıyla alttaki adımları izleyerek geliştirme aracımız olan Livdevelop' u kullanabilirler:

  * http://www.msys2.org/ adresinden msys2 programını download ediyoruz.
  * Programın kurulumunu yaptıktan sonra uygulamayı çalıştırıyoruz (karşınıza uygulamanın konsolu açılacak).
  * Konsolda sırasıyla alttaki komutları veriyoruz.
  ** pacman -Suy
  ** pacman -S mingw-w64-i686-gtk3 mingw-w64-i686-python2-gobject mingw-w64-i686-python3-gobject
  ** pacman -S mingw32/mingw-w64-i686-gtksourceview3 3.24.8-1
  ** pacman -S mingw32/mingw-w64-i686-python3-lxml 4.1.0-1
  * Msys2 programını kurduğunuz klasörün altında yer home/kullanıcı dizinine livdevelop klasörünü kopyalıyoruz.
  * Kurulum burada son bulmakta, kullanım içinse:
  ** Msys2 konsolunda alttaki komutları vererek Livdevelop' u başlatıyoruz.
  *** cd livdevelop
  *** python3 livdevelop.py
