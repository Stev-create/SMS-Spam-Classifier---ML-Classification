<h1> SMS-Spam-Classifier---ML_Classification </h1>

<h3>Source Dataset: https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection </h3>

<p>http://www.dt.fee.unicamp.br/~tiago/smsspamcollection/</p>

## Overview

<p>Project ini bertujuan untuk membuat model yang dapat menentukan mana SMS spam dan mana SMS ham. Kemudian di project ini, saya akan mengevaluasi dua model, yaitu <b>Multinomial Naive Bayes dan Xtreme Gradient Boosting Classifier.</b> Kemudian model terbaik dipilih berdasarkan dari akurasi terbaik.

## Results

### EDA

Pada eksplorasi data, kita seharusnya sudah dapat <i>insight</i> dan tahu bagaimana model akan membedakan mana SMS ham dan spam. Karena jumlah kata dan karakter umumnya ham lebih panjang atau banyak daripada spam. Mengingat kebanyakan SMS spam adalah pesan-pesan yang mengarah ke seolah-olah menang undian atau sesuatu yang penting. Sedangkan SMS ham biasanya lebih mengarah ke perbincangan yang lebih ke pesan singkat. 

![GitHub Logo](/images/1.png)

![GitHub Logo](/images/2.png)

### Words Cloud

WordCloud juga menunjukkan <i>insight</i> yang menarik, untuk SMS spam:

![GitHub Logo](/images/3.png)

Sedangkan untuk SMS ham:

![GitHub Logo](/images/4.png)

Menariknya, kita dapat melihat kalau SMS-SMS ham lebih berbau ajakan atau lebih mengarah ke seolah-olah yang mendapatkan pesan menang undian. Sedangkan ham, seperti yang tadi sudah dikatakan, kata-katanya lebih mengarah ke pesan singkat. Itu kenapa banyak kata-kata singkatan. 

### Evaluation Metrics

| Classifier  | Accuracy |
| :---: | :---: |
| Multinominal Naive Bayes  | 0.97  |
| XGBoost Classifier  | 0.96  |

Dapat dilihat bahwa, Multinominal Naive Bayes lebih baik dari XGBoost. Dan saya pikir tidak perlu lagi mencari model lainnya, mengingat kedua model ini sudah memiliki akurasi yang tinggi. Kemudian pada akhirnya, saya juga melakukan <i>sanity check</i> menggunakan Multinominal Naive Bayes yang dapat dilihat di notebook.





