# Mixed_StepWise_Selection_Method
Bu proje, Python kullanarak basit bir uygulama ile 'Karma Kademeli Seçim Yöntemi' hakkında bilgi sağlamaktadır.

**Selection Methods Nedir ?**

- Gerçek hayatta bir makine öğrenimi modeli oluştururken, veri kümesindeki tüm değişkenlerin bir model oluşturmak için yararlı olması nadirdir. Gereksiz değişkenlerin eklenmesi, modelin genelleme yeteneğini azaltır ve ayrıca bir sınıflandırıcının genel doğruluğunu da azaltabilir. Ayrıca, bir modele daha fazla değişken eklemek, modelin genel karmaşıklığını artırır. Makine öğreniminde seçim yöntemlerinin amacı, birinin yararlı modeller oluşturmasına olanak tanıyan en iyi özellik kümesini bulmaktır. 

**Selection Methods Türleri:**

- Veri seçimi için en önemli ve bilinen yöntemlerden biri 'Aşamalı Seçim Yöntemi' dir. 

Üç tür Aşamalı Yöntem vardır:
- İleri (Step-Up) Seçimi. |  Forward (Step-Up) Selection
- Geri (Adım Aşağı) Seçimi. | Backward (Step-Down) Selection
- Karışık Aşamalı Seçim (adı: Çift Yönlü Seçim). | Mixed Stepwise Selection ( called : Bidirectional Selection)

Bugün "Karma Aşamalı Seçim" tartışılacaktır. 

Mixed Stepwise Selection Method: 
------------------------------------------------------------------------------------------------------------------------

- İleri seçim, modelde hiçbir değişken olmadan başlar, modele eklendikçe her değişkeni test eder, ardından istatistiksel olarak en önemli kabul edilenleri tutar - sonuçlar optimal   olana kadar süreci tekrarlamaktaır
- Geriye doğru eleme, bir dizi bağımsız değişkenle başlar, birer birer silinir, ardından kaldırılan değişkenin istatistiksel olarak anlamlı olup olmadığını test etmektedir.
- Çift yönlü eliminasyon, hangi değişkenlerin dahil edilmesi veya hariç tutulması gerektiğini test eden ilk iki yöntemin birleşimidir. 

Mixed Stepwise Selection, ileri ve geri seçim tekniklerinin bir kombinasyonudur. İleri seçimin bir modifikasyonudur, böylece bir değişkenin eklendiği her adımdan sonra, modeldeki tüm aday değişkenler, önemlerinin belirtilen tolerans seviyesinin altına düşüp düşmediğini görmek için kontrol edilir. Önemsiz bir değişken bulunursa modelden kaldırılmaktadır.

Bu nedenle, iki anlamlılık düzeyi gerektirir: biri değişken eklemek ve diğeri değişkenleri kaldırmak için. Prosedürün sonsuz döngüye girmemesi için değişkenlerin eklenmesi için kesme olasılığı, değişkenleri kaldırmak için kesme olasılığından daha düşük olmalıdır. 


Peki bir veri seti örneğine Mixed Stepwise Selection uygulayalım .. Kod ve sonuçlar kod bölümünde tartışılacaktır. 



