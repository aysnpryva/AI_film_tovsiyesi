CineMatch-AI: Film Tövsiyə Sistemi

Bu layihə, istifadəçinin bəyəndiyi filmə əsasən ona ən yaxın 5 filmi tövsiyə edən süni intellekt (AI) əsaslı bir sistemdir. Sistem **Content-Based Filtering** (Məzmun əsaslı filtrləmə) məntiqi ilə işləyir.

 Xüsusiyyətlər
Ağıllı Axtarış:Böyük-kiçik hərf həssaslığı yoxdur.
Dəqiq Tövsiyə:Janrlar  əsasında hesablanan oxşarlıq.
İnteraktiv İnterfeys: İstifadəçidən giriş alan və nəticəni dərhal göstərən funksiya.
Təmiz Data: Stop-words (lazımsız sözlər) təmizlənməsi və mətni rəqəmlərə çevirmə (Vectorization).

 İstifadə Olunan Texnologiyalar
Python 3.x
Pandas: Data manipulyasiyası üçün.
Scikit-learn:'CountVectorizer' və 'Cosine Similarity' hesablamaları üçün.

 İşləmə Məntiqi
Sistem aşağıdakı mərhələlərlə işləyir:
1.  Data Ingestion: Kaggle-dan IMDb datasetinin yüklənməsi.
2.  Preprocessing: Janrların birləşdirilməsi, boşluqların silinməsi və mətnin kiçik hərflərə çevrilməsi.
3.  Vectorization: Mətn məlumatlarının 'CountVectorizer' vasitəsilə 5000 ölçülü rəqəmsal vektorlara çevrilməsi.
4.  Similarity Calculation: Vektorlar arasındakı "bucaq" məsafəsinin 'Cosine Similarity ilə ölçülməsi.
