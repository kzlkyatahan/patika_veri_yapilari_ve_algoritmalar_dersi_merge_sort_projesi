# Patika Veri Yapıları ve Algoritmalar Dersi Merge Sort Projesi
Patika Veri Yapıları ve Algoritmalar Dersi Merge Sort Projesi

## Merge Sort Aşamaları

Başlangıç Dizisi: [16, 21, 11, 8, 12, 22]

Merge Sort, diziyi sürekli olarak ikiye bölerek ve daha sonra bu bölünmüş parçaları birleştirerek çalışan bir algoritmadır. İşte adım adım nasıl çalıştığı:

1. **Diziyi Bölme**:
   - [16, 21, 11] ve [8, 12, 22]
   - [16] ve [21, 11] | [8] ve [12, 22]
   - [21] ve [11] | [12] ve [22]

2. **Alt Dizileri Sıralama ve Birleştirme**:
   - [21] ve [11] birleştirildiğinde: [11, 21]
   - [12] ve [22] birleştirildiğinde: [12, 22]
   - [16] ve [11, 21] birleştirildiğinde: [11, 16, 21]
   - [8] ve [12, 22] birleştirildiğinde: [8, 12, 22]

3. **Son Birleştirme**:
   - [11, 16, 21] ve [8, 12, 22] birleştirildiğinde: [8, 11, 12, 16, 21, 22]

## Big-O Gösterimi

Merge Sort algoritmasının zaman karmaşıklığı her durumda (en iyi, ortalama, en kötü) O(n log n)'dir. Bu karmaşıklık, diziyi sürekli olarak ikiye bölme işlemi ve ardından bu bölünmüş parçaları birleştirme işlemlerinden kaynaklanmaktadır. 

### Özet Aşamalar:

1. Bölme:
   - [16, 21, 11, 8, 12, 22] -> [16, 21, 11] ve [8, 12, 22]
   - [16, 21, 11] -> [16] ve [21, 11]
   - [8, 12, 22] -> [8] ve [12, 22]
   - [21, 11] -> [21] ve [11]
   - [12, 22] -> [12] ve [22]

2. Birleştirme:
   - [21] ve [11] -> [11, 21]
   - [12] ve [22] -> [12, 22]
   - [16] ve [11, 21] -> [11, 16, 21]
   - [8] ve [12, 22] -> [8, 12, 22]
   - [11, 16, 21] ve [8, 12, 22] -> [8, 11, 12, 16, 21, 22]

Sonuç olarak sıralanmış dizi: [8, 11, 12, 16, 21, 22]

Bu adımlar, Merge Sort algoritmasının nasıl çalıştığını ve diziyi nasıl sıraladığını göstermektedir.
