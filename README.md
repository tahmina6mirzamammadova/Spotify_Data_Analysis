# Spotify_Data_Analysis

Sondan-uca Spotify Trend Analizi layihəsi, fərqli Spotify CSV satış məlumatları və dinləyici demoqrafiya məlumatlarını SQL-ə inteqrasiya edir, ardınca Python (Pandas, NumPy, Scikit-learn) ilə məlumatların təmizlənməsi, EDA, regressiya (ML) proqnozlaşdırılması və son interaktiv Power BI paneli təqdim olunur.

## Layihəyə Ümumi Baxış

Bu layihənin məqsədi iki müxtəlif məlumat dəstini (musiqi xüsusiyyətləri və dinləyici demoqrafiyası) analiz etmək və birləşdirərək ümumi musiqi trendlərini, yaş qrupları üzrə dinləmə vərdişlərini və müxtəlif musiqi xüsusiyyətləri ilə dinləmə müddəti arasındakı əlaqələri anlamaqdır.

Layihə həmçinin tarixi səs xüsusiyyətləri (`energy`, `danceability`) və sənətçi məlumatlarına əsaslanaraq mahnıların potensial dinlənmə sayını (`streams`) proqnozlaşdırmaq üçün sadə maşın öyrənməsi modelini də əhatə edir. Modelin əsas məqsədi hansı xüsusiyyətlərin mahnının populyarlığına təsir etdiyi barədə məlumat verməkdir.

## Layihə İş Axını Diaqramı

<!-- BURA SİZİN ŞƏKİL KODUNUZ GEDİR -->
**![İş Axını Diaqramı](https://github.com/tahmina6mirzamammadova/Spotify_Data_Analysis/blob/main/diagram%20.jpg)** 
<!-- Yuxarıdakı "diaqraminizin_adi.png" hissəsini yüklədiyiniz faylın dəqiq adı ilə əvəz edin! -->

## Layihə İş Axını

**Məlumatların Toplanması və Saxlanması**

*   Spotify musiqi xüsusiyyətləri məlumatları lokal CSV faylından SQL verilənlər bazasına yüklənir.
*   Dinləyici demoqrafiya məlumatları da (yaş, janr üstünlükləri) eyni SQL verilənlər bazasında saxlanılır.
*   Hər iki cədvəl ortaq sütun üzrə birləşdirilir (`JOIN`).

**SQL → Python Processing**

*   Məlumatlar SQL-dən Python-a yüklənir.
*   İlkin məlumatların əvvəlcədən işlənməsi həyata keçirilir.
*   Eksplorativ Məlumat Analizi (EDA) nümunələri (məsələn, yaş vs. janr) və tendensiyaları aşkar etmək üçün aparılır (Matplotlib, Seaborn).

**Maşın Öyrənməsi**

*   Sadə Reqressiya modeli səs xüsusiyyətləri və sənətçi populyarlığına əsaslanaraq mahnıların dinlənmə sayını proqnozlaşdırmaq üçün hazırlanır.
*   Model hansı musiqi xüsusiyyətlərinin hit mahnı yaratdığı barədə məlumat verməyə kömək edir.

**Power BI Dashboard**

*   Bütün məlumatlar, EDA nəticələri və ML proqnozları interaktiv Power BI panelində təqdim olunur.
*   İstifadəçilər yaş kateqoriyası, janr, və ya sənətçi üzrə musiqi tendensiyalarını araşdıra və müxtəlif xüsusiyyətlərin populyarlığa təsirini görə bilərlər.
