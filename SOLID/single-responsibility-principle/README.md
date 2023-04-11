# Single Responsibility Principle - Tek Sorumluluk Prensibi

Selam arkadaşlar, bu yazımda sizlere yazılım geliştirmenin temeli olarak kabul edilen SOLID yazılım geliştirme presiplerinden birisi olan Single Responsibility Prensibini açıklamaya çalışacağım.

Öncelikle sizlere tek bir cümlede SOLID'i özetliyim: Eğer "iyi, temiz kod" yazmak istiyorsak SOLID presiplerine uygun olarak yazılım geliştirmeliyiz. Şimdi gelelim SOLID yazılım geliştirme presiplerinde ilki olan Single Responsibility Prensibine.

## Single Responsibility Prensibi Nedir?
Single Responsibility Prensibi sınıflarımızın(fonksiyonlarımızın) iyi tanımlanmış tek bir sorumluluğu olması gerektiğini anlatmaktadır. Bir sınıf yalnızca kendine yüklenen sorumluluk uğruna değiştirilmelidir, yani bir sınıfın(fonksiyonun) yapması gereken yalnızca bir işi olmalıdır.

Eğer yazdığımız bir sınıf(fonksiyon) birden fazla görevi yerine getiriyorsa, Single Responsibility Prensibine uymuyoruz demektir. Böyle bir durum farkettiğimizde amaçlarına uygun olarak ayırmamız gerekmektedir.

Neden Tek Bir Sorumluluk Yükleriz?
Bir sınıfa(fonksiyona) ne kadar fazla görev yüklersek o kadar değişime uğrar. Bu durumda yeniden yazmak zolaşır, test etmek zorlaşır ve çokça bağımlılıkla da uğraşırız. Ayrıca kodun okunabilirliği de düşer. Bunun tam tersi olarak ne kadar az görev yüklersek de bizim için o kadar iyi olur.

Eğer bir sınıfı(fonksiyonu) yazmadan önce sorumluluğunu, amacını iyice düşünerek tasarlarsak, herhangi bir değişim durumunda daha az şeyi düzenleyerek istenilen sonucu elde edebiliriz.

Bir örnek üzerinde inceleyelim.

<img src="https://tolgahantolu.vercel.app/_next/image?url=https%3A%2F%2Fmedia.graphassets.com%2F18vAraczRcG8sQRjj6x7&w=1920&q=75" />

Bu örnekte class hem hesaplama için bir fonksiyon içeriyor hem de kullanıcıya mesaj göstermek için bir fonksiyon içeriyor. Bu yüzden bizim <b> Single Responsibility Prensibimize </b> uymuyor.

Bu örneğimizi prensibimize uygun olarak düzenleyelim.

<img src="https://tolgahantolu.vercel.app/_next/image?url=https%3A%2F%2Fmedia.graphassets.com%2FHc07n6XLTV2Hd5LfQBAw&w=1920&q=75" />

Artık hem mesaj göstermek için hem de hesap yapmak için farklı iki sınıfımız var. Single Responsibility prensibine uyuyor.

## Sonuç
Single responsibility prensibi sınıflarımızın iyi tanımlanmış tek bir sorumluluğu olması gerektiğini anlatmaktadır. Bir sınıfın/fonksiyonun yalnızca bir işi olmalıdır, birden fazla amaca hizmet etmemelidir.
