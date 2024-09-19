Bu projede 2016-2023 yılları arasında gerçekleşen trafik kazalarının kayıtlarından oluşan bir Kaggle veri seti üzerinde EDA(Keşifsel Veri Analizi), veri ön işleme, çeşitli gözetimli ve gözetimsiz makine öğrenmesi modelleri geliştirme ve bu modelleri değerlendirme işlemleri yaptım. Veri seti oldukça büyük, kirli ve karmaşıktı. Keşfi ve analizinde zorlandığım birçok nokta oldu. Bazen verinin büyüklüğünden dolayı yetersiz RAM sorunlarıyla karşılaştım ve veri ön işlememi bunu da göz önünde bulundurarak tekrar yaptım.

Bu projede bir tanesi gözetimsiz bir tanesi de gözetimli olmak üzere 2 adet makine öğrenmesi modeli üzerinde çalıştım. 

Gözetimsiz olan makien öğrenmesi modelim bir K-Means Clustering (K-Ortalama Kümeleme) modeliydi. Bu modeli eğitmeden önce veri ön işleme kısmında gerekli encoding ve standardization işlemleri uyguladım. Gözetimsiz bir model olduğu için verime etiketleme işlemleri uygulamadım doğal olarak. Gerekli veri ön işleme adımlarını tamamladıktan sonra modelimi eğittim. Model eğitimden sonra model değerlendirme başlığı altında K-Means dağılım ve kümeleme grafiğini çizdirip merkez noktalarını grafik üzerinde göstererek veri setim e modelim hakkında çıkarımlarda bulunmuş oldum.

Gözetimli olan makine öğrenmesi modelim ise bir Lojistik Regresyon (Logistic Regression) modeliydi. Bu model için de gerekli olan encoding ve standardization işlemlerine ek olarak gözetimli bir model olmasından kaynaklı verime etiketleme işlemini de uyguladım. Bu modelde tahmin edilecek Target Variable (Hedef Değişken) 'Fault At Driver' değişkeniydi. Kazanın sürücüden kaynaklı olup olmadığını tahminleyen bu modelim beklentimin üzerinde bir performans sergileyerek 0.86 Accuracy Score (Doğruluk Puanı) ile çalıştı. Aslında modelimin başarısını bir metrik açısından görmüştüm. Ancak model değerlendirme aşaması kapsamında Cross Validation (Çapraz Doğrulama), Accuracy (Doğruluk), Standart Sapma, precision (kesinlik),  recall (duyarlılık),  f1-score (F1 puanı) , support gibi model değerlendirme metriklerini de inceleyerek modelimi detaylıca değerlendirmiş oldum.

Projemdeki bulunan yorum satırlarını ingilizce olarak yazdım. İlerleyen zamanlarda full ingilizce halini de paylaşmayı düşünüyorum.

Ayrıca projemi ilgili Kaggle veri seti altında da paylaştım. Linkini aşağıya ekliyorum.

Kaggle Linki: https://www.kaggle.com/code/ahmetcantak/eda-ml-models
