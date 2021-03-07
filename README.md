# KNN-Tree-Ensemble-Algorithms
KNN,Decision Tree ve Ensemble Algoritmalarını kullanarak kategorik değişken sınıflandırılması yaptım.Modellerin önemli parametrelerini optimize ederek model için en iyi optimum değerler ile yeni modeler oluşturup bu modellerin başarılarını karşılaştırdık

# K-Nearest Neighbors
- İlk sınıflandırma yaptığımız algoritma, KNN algoritmasıdır.
- Tahminler gözlem benerliğine göre yapılır.KNN algoritması sınıflandırma yaparken, sınıflandırma yapacağımız yeni verimizin çevresindeki en yakın , bizim belirlediğimiz k sınıf sayısının sıklığına göre sınıflandırma yapar.
- Çevresindeki en yakın verileri bulabilmek için uzaklık hesabı yapar.Uzaklık hesabı yapmak için 3 tip uzaklık fonksiyonu kullanılır.Bunlar ;
    
    - **"Euclidean" Uzaklık**
    - **"Manhattan" Uzaklık**
    - **"Minkowski" Uzaklık**    

## KNN Basamakları

- İlk olarak komşu sayısı(**k değeri**) belirlenir.KNN Algoritmamızda bu değerin belirlendiği parametre **n_neighbors** parametresidir.
- Bilinmeyen nookta ile diğer tüm noktalar arasındak- ki uzaklık hesaplanır.(Yukarıdaki uzaklık hesabı ile). Algoritmamızda uzaklık hesabının belirtildiği parametre **metric** parametresidir.
- Hesaplanan Uzaklıklar sıralanır ve belirlenen k sayısına göre en yakın(uzaklık hesabına göre) olan k gözlemi seçer
   
   - **Sınıflandırma yaparken** ; En sık sınıf tahmin değeri olarak verilir
   - **Regresyon'da** ; En yakında bulunan k kadar gözlemin ortalama Değeri tahmin değeri olarak verilir

# Destek Vektör Makineleri - SVM 

- Amacımız iki sınıf arasındaki marjinin maximum olmasını sağlayacak doğruyu ortaya çıkarmaya çalışmaktır
- SVM bizim için max marjin bulur 
- Marjini max marjin yapacak iki point bizim support vektörümüzdür
- Support Vector Machine , Logistic Regression ile benzer bir sınıflandırma algoritmasıdır
- SVM , aynı zamanda **"doğrusal"** ve **"doğrusal olmayan"** verileride sınıflandırabilir ancak genellikle verileri **doğrusal** olarak sınıflandırmaya çalışır
## Kernel Trick
- SVM , verileri doğrusal olarak sınıflandıramadiği zaman **Kernel Trick(Çekirdek Hilesi)** yöntemine ile bu durumu çözer
# Decision Tree Classifier 
