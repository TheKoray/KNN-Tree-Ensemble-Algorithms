# KNN-Tree-Ensemble-Algorithms
KNN,Decision Tree ve Ensemble Algoritmalarını kullanarak kategorik değişken sınıflandırılması yaptım.Modellerin önemli parametrelerini optimize ederek model için en iyi optimum değerler ile yeni modeler oluşturup bu modellerin başarılarını karşılaştırdık

## KNN
- İlk sınıflandırma yaptığımız algoritma, KNN algoritmasıdır.
- Tahminler gözlem benerliğine göre yapılır.KNN algoritması sınıflandırma yaparken, sınıflandırma yapacağımız yeni verimizin çevresindeki en yakın , bizim belirlediğimiz k sınıf sayısının sıklığına göre sınıflandırma yapar.
- Çevresindeki en yakın verileri bulabilmek için uzaklık hesabı yapar.Uzaklık hesabı yapmak için 3 tip uzaklık fonksiyonu kullanılır.Bunlar ;
    
    - **"Euclidean" Uzaklık**
    - **"Manhattan" Uzaklık**
    - **"Minkowski" Uzaklık**    

## KNN Basamakları

   1- İlk olarak komşu sayısı(**k değeri**) belirlenir.KNN Algoritmamızda bu değerin belirlendiği parametre **n_neighbors** parametresidir.
   2- Bilinmeyen nookta ile diğer tüm noktalar arasındak- ki uzaklık hesaplanır.(Yukarıdaki uzaklık hesabı ile). Algoritmamızda uzaklık hesabının belirtildiği parametre **metric** parametresidir.
   3- Hesaplanan Uzaklıklar sıralanır ve belirlenen k sayısına göre en yakın(uzaklık hesabına göre) olan k gözlemi seçer
   
     --> **Sınıflandırma yaparken** ; En sık sınıf tahmin değeri olarak verilir
     --> **Regresyon'da** ; En yakında bulunan k kadar gözlemin ortalama Değeri tahmin değeri olarak verilir
