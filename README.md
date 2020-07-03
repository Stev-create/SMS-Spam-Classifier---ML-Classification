<h1> SMS-Spam-Classifier---ML_Classification </h1>

<h3>Source Dataset: https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection </h3>

<p>http://www.dt.fee.unicamp.br/~tiago/smsspamcollection/</p>

## Overview

<p>Project ini bertujuan untuk membuat model yang dapat menentukan mana SMS spam dan mana SMS ham. Kemudian di project ini juga, akan mengevaluasi dua model yaitu <b>Multinomial Naive Bayes dan Xtreme Gradient Boosting Classifier.</b> Kemudian model terbaik dipilih berdasarkan dari akurasi terbaik. Ringkasan hasil terdapat di bawah ini, namun untuk lebih lengkapnya dapat dilihat di 

## Results

### EDA

Pada eksplorasi data, kita seharusnya sudah mendapatkan <b>insight</b>-nya dan tahu bagaimana caranya model akan membedakan mana SMS ham dan spam. Karena dari visualisasi di bawah misalnya, ternyata jumlah kata dan karakter umumnya ham lebih panjang atau banyak daripada spam. Dan ini masuk akal, mengingat kebanyakan SMS spam adalah pesan-pesan yang mengarah ke seolah-olah menang undian atau sesuatu yang penting. Sedangkan SMS ham biasanya lebih mengarah ke perbincangan yang lebih ke pesan singkat. 

![GitHub Logo](/images/1.png)

![GitHub Logo](/images/2.png)

### Words Cloud

WordCloud juga menunjukkan <i>insight</i> yang menarik, untuk SMS spam:

![GitHub Logo](/images/3.png)

Sedangkan untuk SMS ham:

![GitHub Logo](/images/4.png)

<b>Insight</b> : Dari visualisai di atas, kita dapat melihat kalau SMS-SMS ham lebih berbau ajakan atau lebih mengarah ke seolah-olah yang mendapatkan pesan menang undian. Sedangkan ham, seperti yang tadi sudah dikatakan, kata-katanya lebih mengarah ke pesan singkat. Itu kenapa banyak kata-kata singkatan. 

### Evaluation Metrics

| Classifier  | Accuracy |
| :---: | :---: |
| Multinominal Naive Bayes  | 0.97  |
| XGBoost Classifier  | 0.96  |

Dapat dilihat bahwa, Multinominal Naive Bayes lebih baik dari XGBoost. Dan saya pikir tidak perlu lagi mencari model lainnya, mengingat kedua model ini sudah memiliki akurasi yang tinggi. Kemudian pada akhirnya, saya juga melakukan <i>sanity check</i> menggunakan Multinominal Naive Bayes yang dapat dilihat di [notebook ini](https://github.com/Stev-create/SMS-Spam-Classifier---ML-Text-Classification/blob/master/SMS%20Spam%20Classifier.ipynb).







