## BİNARY SEARCH TREE
### PROJE 3
- SORU 1:   [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

- CEVAP 1: 
Binary search tree bir kök dizinin bulunmasıyla başlar, kök dizinin yanından sırayla başlayarak,  solunda kök değerinden düşük sayılar, sağ tarafta ise daha büyük sayılar dizilir.
[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin binary search tree aşamaları ise;

1-  Kök eleman olarak 7' yi alalım.

2-  Sıradaki elemanımız ise 5, 5<7 bu sebeple sol tarafa yazılır.

3- Üçüncü elemanımız 1<5'ten  bu sebeple 5'in sol tarafına yazılır.

4- Dördüncü elemanımız 8, kök sayıdan büyük olduğu için sağ tarafa yazılır.

5- Beşinci elemanımız 3, 3>1  fakat aynı zamanda 3<5 olduğu için 1'in sağ tarafına yazılır yani sağ çocuğu olur.

6- Altıncı elemanımız 6, 6>1 bir üst sıraya geçeriz ve bakarız 6, 5 sayısından da büyüktür, bir üst sıraya daha bakarız fakat burada 6<7 bu sebeple 6 sayısını 5'ten büyük olduğu için 5'in sağına yazarız.

7- Yedinci elemanımız 0, 0<1 olduğu için, 1'in sol tarafına yazılır, yani sol çocuğu olur.

8- Sekizinci elemanımız 9, kök sayıdan ve 8'den büyük olduğu için 8'in sağ tarafına yazılır.

9- Dokuzuncu elemanımız 4, 4>3 fakat aynı zamanda 4<5 bu sebeple 4, 3 sayısının sağ tarafında yer alır.

10- Ve son elemanımız 2, 1'den büyük fakat 3 sayısından küçük olduğu için 3 sayısının sol tarafına yazılır ve böylece ağacımızın son durumu şöyle şekillenir;

                      7
                    /   \
                   5     8
                  / \     \
                 1   6     9
                / \
               0   3
                  / \
                 2   4