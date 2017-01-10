Packager Windows Paket Yöneticisi 0.0.1
=================================

Packager sayesinde GNU/Linux tabanlı sistemlerde kullanılan paket yönetimi ile windows programlarınızı buradan yönetebileceksiniz.

Aktif Özellikler
----------------
1. Liste güncelleme
2. Kaldırma
3. Listeleme
5. Kurulum (özel dizin belirtme)
6. Nerede özelliği

Kullanımı
---------
>Not: Güncelleme işlemi için updateRepositories.js dosyasındaki url değişkeninin düzenlenmesi gerekmektedir. Sunucu dosyaları ana dizindeki server içindedir.


```
Usage: packager [options]
-h, --help                                 output usage information
-V, --version                              output the version number
guncelle                      [            Paket Listesini Günceller.
kur [paket_kodu[, kurulacak_dizin, sürüm]] Belirtilen Paketi Kurar.
kaldir [paket_kodu]                        Belirtilen Paketi Kaldırır.
listele                                    Kurulu Paketleri Gösterir.
nerede [paket_kodu]                        İstenilen Paketin Kurulum Dizinini Gösterir.
```

İleride Eklenecekler
====================
1. Spesifik sürüm belirtme
2. URI protokol ile programlar 'packager://calistir/npp' örneğindeki gibi çalıştırılacak ve kısayollar internet kısayolu formatında olacak (Steam gibi)
3. Paket Kurulumuna Kurulacak Dizini Belirtme
4. Aktif Sunucu (PHP)

Demo Kurulum Yönergeleri
------------------------
Server klasörü içindeki dosyaları sanal sunucunuzun ana dizine veya ayarladığınız herhangi bir dizine atın. updateRepositories.js dosyası içinde url stringindeki url'yi attığınız sunucu dosyaları ile aynı olarak değiştirin. İlk çalıştırmada oluşturulacak dizinler ve kaydedilecek ortam değişkenleri sebebiyle yönetici olarak çalıştırmak gerekebilir. Paket kurulumu için internete ihtiyaç duyar. Şu an sadece Notepad++ 6.0.9 sürümü mevcut (npp paket kodu ile).

Açıklamadaki komutlar ile paket kaldırma, kurma, listeleme depo güncelleme gibi işlemleri yapabilmektedir. 
