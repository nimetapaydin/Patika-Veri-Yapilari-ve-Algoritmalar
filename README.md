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

22 16 27 | 2 18 6 (sıralamamız henüz bitmedi çünkü 21, 33’ten de küçük:)

16 22 27 | 2 18 6 (şimdi 3. sıralamayı tamamladık ve bir sonraki sayı 2’yi alabiliriz:)

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


Sokma sıralamasının (insert sort) performansı O(n2)’dir. Bunun sebebi dizideki eleman sayısı kadar geçiş gerekmesi ve her geçişte en kötü ihtimalle elemsan sayısı kadar kaydırma gerekmesidir. Yani insertion sort’un en kötü durumu tersten sıralı bir listedir. Yukarıdaki örneği düşünecek olursak:

83 73 56 44 33 22 21 sıralamasındaki bir dizi en uzun sürede sıralanan dizidir. Buna karşılık sıralı bir dizi verildiğinde diziye 2n sayıda erişim erişim yeterlidir.
```
