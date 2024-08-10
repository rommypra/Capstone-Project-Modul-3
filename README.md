# CUSTOMER LIFETIME VALUE
## Business Problem
### Background
Customer lifetime value adalah pengukuran berapa potensi revenue seorang pelanggan bagi sebuah perusahaan. Dari pengukuran tersebut perusahaan bisa menentukan *treatment* yang tepat bagi setiap pelanggan. Hal ini bertujuan memaksimalkan profit dari pelanggan juga efisiensi sumber daya yang dialokasikan untuk pelanggan.

Pada kasus ini, terdapat perusahaan asuransi yang bergerak di bidang otomotif. Perusahaan ini ingin menjawab isu-isu berikut:
1. Efisiensi biaya dan waktu di aktivitas marketing dan sales.
1. Menentukan strategi marketing dan sales lebih tepat sasaran.
1. Uplift nasabah *low value* menjadi nasabah *high value*.
1. Menentukan *treatment* yang tepat bagaimana meng-handle nasabah *high value* dan *low value*.

### Goals
Sebagai data scientist kita akan membantu perusahaan menajawab isu-isu terserbut dengan menggunakan metode machine learning. Kita akan gunakan supervised machine learning model regresi.
### Metric Evaluation

Metode pengukuran machine learning yang digunakan menggunakan RSME, MAE, dan MAPE. Pada model regresi ketiga pengukuran tersebut mampu mengintrepretasikan ketepatan model dalam memprediksi. RSME dipilih metode optimalisasi. MAE dan MAPE dipilih karena mudah diinterpretasikan.

$$RMSE =   \sqrt{ \frac{ \sum\nolimits_{i=1}^{n} ( Y_i - \widehat{Y_i})^2 }{n} } $$

$$MAE =  \frac{\sum\nolimits_{i=1}^{n} |Y_i - \widehat{Y_i}|}{n}$$

$$MAPE =  \frac{1}{n}   \sum_{i=1}^{n} | \frac{Y_i - \widehat{Y_i}}{Y_i}|$$

Keterangan:<br>
$n$ = Jumlah data<br>
$i$ = Variabel i<br>
$Y_i$ = Data aktual<br>
$\widehat{Y_i}$ = Data Prediksi
