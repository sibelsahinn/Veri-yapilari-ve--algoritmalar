# PROJE 1
## İnsertion Sort 
*[22,27,16,2,18,6]*
## SORU 1
###  Yukarıda verilen dizinin sort türüne göre aşamalarını yazınız.

- CEVAP 1

lnsertion Sort sıralama algoritmasının temel mantığı, sayı öbeğini en küçükten en büyüğe doğru sıralamaktır. 

**DİPNOT;** "/" sembolü sıralamanın ayrım noktasını göstermek için kullanılmıştır. Sembolün solunda kalan elemanlar sıralanmış kabul edilir ve sayı dizisinde sırası gelen eleman hemen yan tarafında bulunan elemanla karşılaştırılır. Sıralama işlemine en küçükten en büyüğe olacak şekilde devam edilir.

- 1. ADIM: 22 ve 27 sayısı karşılaştırılır 22<27 olduğu için 22 yerinde kalmaya devam eder.

- 2. ADIM: 27 İle 16 karşılaştırılır. 27>16 olduğu için 16 önce 27 yerine gelir ve 22 ile karşılaştırılır, 22>16 olduğu için sıralama **[16,22,27/2,18,6]**  şeklinde güncellenir.
16'nın solunda sayı olmadığı için 16 yerinde şimdilik yerinde kalır.
- 3. ADIM: 27 sayısı ile 2 karşılaştırılır. 27> 2 olduğu için 2 sayısı 27'nin soluna geçer ve solundaki diğer elemanlarla tek tek karşılaştırılmaya devam eder. 22>2, 16>2 olduğu için 2 sıralamanın en başına gelir ve güncel sıralama **[2,16,22,27/18,6]** halini alır.
- 4. ADIM: 18 sayısı (sıralanmış sayıların sağındaki ve sıradaki sayı olduğu için) 27 ile karşılaştırılır. 27>18 dolayısıyla bir sola geçer ve 22 ile karşılaştırılır. 22>18 bu sebeple yine sağa geçer ve 16<18 olduğu için sıralama şu şekilde değişir **[2,16,18,22,27/6]** 

- 5. ADIM: 6 sayısı 27 ve sağındaki diğer sayılarla karşılaştırılır karşılaştırma 6'nın en küçük olduğu yeri bulana kadar devam eder. 27>6, 22>6, 18>6, 16>6 ve en son eleman olan 2 ile karşılaştırılınca yerini bulur 2<6 ve sıralamanın son hali **[2,6,16,18,22,27]** şeklini alır.
 ## SORU 2
 ### Big- O gösterimini yazınız.
 - CEVAP 2

 Sayı dizimizin eleman sayılarına n dersek, en küçük sayıyı bulana kadar dizideki diğer elemanlarla karşılaştıracağımız için n, n-1, n-2, n-3 ..... ve 1 olana kadar sıralama işlemine devam edeceğiz.                      
 **n.(n+1)/2** =  **n<sup>2 </sup>+n/2'** yi bize verir. Big- O Notation'da bizim için katsayısı en yüksek olan önemli olduğu için Big- O gösterimi  **O(n<sup>2 </sup>)** şeklinde olacaktır.

 ## SORU 3
 ### Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisi kapsamına girer?
 1. Average Case: Aradığımız sayının ortada olması.
 2. Worst Case: Aradığımız sayının sonda olması.
 3. Best Case: Aradığımız sayının dizinin en başında olması.
 - CEVAP 3: Average Case, olması beklenen senaryo. Aradığımız sayının ortada olması.

## SORU 4
*[7,3,5,8,2,9,4,15,6]* dizisinin Selection Sort' a göre ilk 4 adımını yazınız.
- CEVAP 4

Selection Sort'ta Insertion Sort gibi sayı dizisini  en küçükten en büyüğe olacak şekilde sıralar. Sayı dizisinde en küçük sayıyı bulur ve dizinin başına yerleştirir, yerleştirdiği sayı ile  hangi sıradan sayı aldıysa aldığı sayı yer değiştirir.

- ADIM 1: 
Sayı dizisindeki en küçük sayıyı buluyoruz o da 2, 2 sayısı sıralamanın en başına gelicek ve 7 sayısı ile yer değiştirecek ve yeni sıralama *[2,3,5,8,7,9,4,15,6]* bu şekilde olacak.
- ADIM 2: Sayı dizisindeki 2'den sonra gelen en küçük sayıyı buluyoruz ve yine aynı mantıkta yer değiştiriyoruz fakat zaten en küçük sayı 3 olduğu için sıralamada yeri değişmiyor.
 - ADIM 3: Bir sonraki küçük sayı 4 dolayısıyla 5 ile yer değişir ve yeni sıra *[2,3,4,8,7,9,5,15,6]* olur.
 - ADIM 4: Bizden 4 aşamalı sıralama istediği için, son adımda 5 ile 8 sayısı yer değitirir ve sıralamamızın son hali *[2,3,4,5,7,9,8,15,6]* olur.