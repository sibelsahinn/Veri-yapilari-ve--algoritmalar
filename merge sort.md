# PROJE 3
## MERGE SORT
**[16,21,11,8,12,22]**
## SORU 1
### Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
- CEVAP 1

Merge Sort, bölme ve birleştirme mantığıyla çalışır. Diziyi küçük parçalara böler ve dizi tek elemana ininceye kadar bu işleme devam eder, sonrasında ise birleştirme aşaması başlar.

1. BÖLME AŞAMASI: **[16,21,11,8,12,22]** sayı dizisini ortadan bölünerek şu şekile bürünür:

- **[16,21,11]** ve **[8,12,22]** 
- **[16,21,11]** ve **[8,12,22]** >> **[16]** , **[21,11]** ve **[8]**, **[12,22]** 

-  **[16]** , **[21,11]** ve **[8]**, **[12,22]** >> **[16]**, **[21]**, **[11]**, **[8]**, **[12]** ve **[22]** şeklinde tek bir dizi haline getirilir bu aşamadan sonra ise tek tek ayrılan elemanlar sayı dizisinde bir bütün olacak şekle gelene kadar birleştirilir ve sıralanır.
----------------------------------------------------------------

2. BİRLEŞTİRME AŞAMASI: **[16]**, **[21]**, **[11]**, **[8]**, **[12]** ve **[22]** son hali küçükten büyüğe sıralanacak şekle gelene kadar birleştirilir.
- **[16]**, **[21]**, **[11]**, **[8]**, **[12]** ve **[22]** >> **[16]**, **[11,21]** ve **[8]**, **[12,22]**

- **[16]**, **[11,21]** ve **[8]**, **[12,22]**>> **[11,16,21]** ve **[8,12,22]**
- **[11,16,21]** ve **[8,12,22]** >> SONUÇ= **[8,11,12,16,21,22]**

## SORU 2
### Big- O gösterimini yazınız.
- CEVAP 2

Merge Sort "Böl ve Birleştir" mantığıyla hareket ettiği için her seferinde diziyi yarıya böler (n/2, n,4 .... 1) ve bu da logaritmik zamanı ifade eder. 
Birleştirme aşamasında ise en kötü senaryoda tüm sayıları birbiriyle karşılaştırması gerekmektedir ve bu da bize n zamanı ifade eder. Bu iki aşama sonrası, Merge Sort'un, "Big- O Notationu"  O(nlogn) olarak karşımıza çıkar.
