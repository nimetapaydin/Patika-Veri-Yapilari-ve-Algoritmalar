# Patika-Veri-Yapilari-ve-Algoritmalar
Patika-Veri Yapıları ve Algoritmalar Dersine ait Projeler kısmında yer alan ödevlerin çözümlerini içermektedir.

## Insertion Sort Projesi - Proje 1

```
[22,27,16,2,18,6] -> Insertion Sort

1.Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
2.Big-O gösterimini yazınız.
3.Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.
4.Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.


[7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.
```

## Insertion Sort Projesi - Proje 1- Çözüm

```

22 27 16 2 18 6  

İlk sıralamada sadece 22 sayısı sıralanmış oluyor. Çünkü o ilk sayı ve bu sebeple yer değiştirme yapmıyoruz.

İşaretin “|” solundaki sayılar sıralanmış sayılar. Ve her sıralamada bir sağındaki sayıyı alıyoruz)

sıradaki sıralamada sıralayacağımız sayı 27. 22 ile 27’yi karşılaştırıyoruz 22 küçük bu sebeple yer değiştirme işlemi yapmıyoruz

22 27 | 21 83 56 73 22

Sıradaki sayı 16. 16 ile 27 karşılaştırılıyor ve 16 küçük olduğu için 27 ile yer değiştiriyorlar :

22 16 27 | 2 18 6 (sıralamamız henüz bitmedi çünkü 16, 22’den de küçük)

16 22 27 | 2 18 6 (şimdi 3. sıralamayı tamamladık ve bir sonraki sayı 2’yi alabiliriz )

16 22 2 27 | 18 6

16 2 22 27 | 18 6

2 16 22 27 | 18 6

sıradaki sıralamada 18 var:

2 16 22 27 18 | 6 

2 16 22 18 27 | 6 

2 16 18 22 27 | 6 

sıradaki sıralamada 6’yı sıralayacağız:

2 16 18 22 27 | 6 

2 16 18 22 6 27 |

2 16 18 6 22 27 |

2 16 6 18 22 27 |

2 6 16 18 22 27 |

2.Big-O gösterimini yazınız

İnsert Sort Big-O gösterimi O(n^2)’dir. Bunun sebebi dizideki eleman sayısı kadar sıralama için yer değiştirme gerekmesi ve her geçişte en kötü ihtimalle eleman sayısı kadar kaydırma gerekmesidir.


3.Time Complexity: 
Average case: Aradığımız sayının ortada olması,
Worst case: Aradığımız sayının sonda olması,tersten sıralı bir liste
Best case: Aradığımız sayının dizinin en başında olması.

4.Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? 
2 6 16 18 22 27 |
Average case: Aradığımız sayının ortada olması,

[7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

7 | 3 5 8 2 9 4 15 6

7 3 | 5 8 2 9 4 15 6

3 7 | 5 8 2 9 4 15 6

3 7 5 | 8 2 9 4 15 6

3 5 7 | 8 2 9 4 15 6

```

## Merge Sort Projesi - Proje 2

```
[16,21,11,8,12,22] -> Merge Sort

Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
Big-O gösterimini yazınız.


1. adım dizi ikiye bölünür:

16,21,11 ve 8,12,22

2. adım dizinin yeni halini de ikiye böl:

16,21 ; 11,8 ; 12,22

3. adım elde edilen parçalar 2 veya daha küçük eleman sayısına ulaştığı için duruyoruz (yoksa bölme işlemi devam eder)

4. adım her parçayı kendi içinde sıralanır

16,21 ; 8,11 ; 12,22

5. Bölünmüş parçaları sıraya dikkat ederek birleştiriyoruz 

8,16,21 ve 11,12,22

6. adım, tek bir bütün parça haline gelene kadar birleştiriyoruz

8,11,12,16,21,22

Big-O gösterimini yazınız.

Big-O gösterimi O(nlog(n))’dir.

```



## Binary Search Tree Projesi - Proje 3

```
[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

```

![figure](https://raw.githubusercontent.com/nimetapaydin/Patika-Veri-Yapilari-ve-Algoritmalar/main/figure/binarysearchtree.png)

```
Root 7

İkici elemanımız "5". 5, 7'den küçük sola ekledik

üçüncü elemanımız "1". 1, 7'den ve 5 ten küçük. Bu sebeple 5 in soluna ekledik

dördüncü elemanımız "8". 8, 7'den büyük 7'nin sağına ekledik.

beşinci elemanımız "3". 3, 7 den küçük solda olmalı. Aynı zamanda 5 ten de küçük ama 1 den büyük bu sebeple 1'in sağında olmalı

altıncı elemanımız "6". 6, 7 den küçük solda olmalı. Aynı zamanda 5 ten büyük bu yüzden beşin sağında olmalı

yedinci elemanımız "0" . 0, 7 den küçük solda olmalı. Aynı zamanda 5 ten de ve 1 dende küçük bu sebeple 1'in solunda olmalı

sekizinci elemanımız "9". 9, 7'den büyük 7'nin sağına ekledik. Aynı zamanda 8 den de büyük bu sebeple 8'in sağında olmalı

dokuzuncu elemanımız "4". 4, 7den küçük solda olmalı. Aynı zamanda 5 ten de küçük ama 1 den büyük ayrıca 3 den de büyük bu sebeple 3'ün sağında olmalı

onunca elemanımız "2". 2, 7 den küçük solda olmalı. Aynı zamanda 5 ten de küçük ama 1 den büyük aynı şekilde 3 dende küçük yani 3'ün solunda olmalı

```



# Proje içi Patika linki

[Patika](https://www.patika.dev/tr)

# License

[MIT](https://choosealicense.com/licenses/mit/)


