# Görüntü İşleme ile Araç Takibi
##  Projenin genel tanımı ve amacı

Proje konum ise görüntü işleme ile video üzerindeki araç takibi.
Öncelikle bu projeyi seçmemin sebebi görüntü işleme üzerinde işlemler yapmayı öğrenmeye çalışmaktı. 
Bu proje tamamlandığında trafikte veya herhangi bir yere giren-çıkan araç sayısını bulmamızda bizlere yardımcı olacak.
Eğer projeme arayüz ekleyebilirsem kullanım açısından sadece seçilen videodaki araçları sayacağı için herkese kolaylık sağlayacaktır.

### Kullanılan teknolojiler
Projemde **Python** ile görüntü işleme yaparak araç takibi yapıyorum.
Kütüphane olarak opencv kütüphanesini python'a yüklemeniz gerekiyor

### Proje uygulama aşamaları
* Öncelikle gerekli python ve gerekli kütüphane ve yazılımlarını indirdim.
* Sonra opencv kütüphanesini araştırdım çünkü genellikle oradan çektiğimiz fonksiyonları kullanıyoruz.
* Kullanacağım araçların geçtiği videoyu araştırdım.
#### Kullanılan fonksiyonlar
* **imshow("Ana Görüntü",image)** fonksiyonu ile videoyu normal biçiminde gösteriyoruz.
* **imshow("Gray Görüntü", gray)** fonksiyonu ile videoyu gray şekile getiriyoruz.
* **imshow("fgmask", fgmask)** fonksiyonu ile hareket eden cisimleri belirliyoruz.
* **imshow("Bel_Nok_Giderme", closing)** fonksiyonu ile belirlenen cisimlerin içerisindeki noktaları gidermeye çalışıyoruz.
* **imshow("Cev_Nok_Giderme", opening)** fonksiyonu ile cisimlerin çevresindeki noktaları temizliyoruz.
* **imshow("Nesneleri kalinlastirma", dilation)** fonksiyonu ile belirlenen nesneleri kalınlaştırarak yerlerini tam olarak belirlemeye çalışıyoz.
* **imshow("retvalbin", retvalbin)** threshold fonksiyonu ile Binary koda çeviriyoruz.
* Bunların hepsini yaptıktan sonra **imshow("Sonuc", image)** fonksiyonu ile görüntüyü ekrana veriyoruz.

![GitHub Logo](/images/kapak.png)
