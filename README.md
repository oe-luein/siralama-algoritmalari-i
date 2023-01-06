[22,27,16,2,18,6]

Soru 1: Dizinin insertion sort türüne göre aşamalarını.

Dizinin ikinci elemanından başlanarak tek tek kontroller yapılır. Seçilen eleman, kendinden önceki elemanlardan büyük mü küçük mü diye kıyaslanır. Bu karşılaşmanın sonucuna bağlı olarak elemanların yerleri değişir.

Dizide ilk kontrol edilecek eleman 27'dir. En küçükten en büyüğe sıralama, aşama aşama şöyle olur.

27 > 22 olduğu için yer değişimi olmayacak.
[22,27,16,2,18,6]

Dizinin 3. elemanı 16 ele alınır.
16 < 27 olduğu için her iki elemanın yeri değişir.
Daha sonra 16 ile 22 karşılaştırılır. 16 < 22 olduğu için dizinin ilk elemanı artık 16 olur.
[16,22,27,2,18,6]

Dizinin 4. elemanı 2 kontrol edilir.
2 < 27: Yer değişikliği yapılır.
2 < 22: Yer değişikliği yapılır.
2 < 16: Yer değişikliği yapılır.
Kendinden önceki tüm elemanlardan küçük olduğu için en başa eklenir 2.
[2,16,22,27,18,6]

Dizinin 5. elemanı 18 kontrol edilir.
18 < 27: Yer değişikliği yapılır.
18 < 22: Yer değişikliği yapılır.
18 > 16: Yer değişikliği yapılmaz.
16'ya kadar olan elemanlar arasından en küçük olduğu tespit edilir.
[2,16,18,22,27,6]

Dizinin 6. elemanı 6 kontrol edilir.
6 < 27: Yer değişikliği yapılır.
6 < 22: Yer değişikliği yapılır.
6 < 18: Yer değişikliği yapılır.
6 < 16: Yer değişikliği yapılır.
6 > 16: Yer değişikliği yapılmaz.
İlk eleman dışındaki tüm elemanlardan daha küçük olduğu için dizinin ikinci elemanı 6 olur. Böylece dizi, son halini almış olur.
[2,6,16,18,22,27]


Soru 2: Dizinin Big-O gösterimi nedir?

Insertion sort algoritmasının worst case time complexity değeri O(n)'dir. Selection sort algoritmasının ise O(n^2)'dir

Soru 3: Dizi sıralandıktan sonra 18 sayısı, time complexity bakımından hangi case'e girer?

18 sayısı, average case'e dahil olur.

Soru 4: [7,3,5,8,2,9,4,15,6] dizisinin selection sort algoritmasına göre ilk 4 adımı nedir?

Dizinin en küçük elemanı tespit edilir ve 0. indisteki eleman ile yeri değiştirilir. Bu durumda 7 ve 2 yer değiştirir.
[2,3,5,8,7,9,4,15,6]

İlk eleman dışındaki sayılar arasındaki en küçük değer olan 3, dizinin 1. indisine taşınır. Zaten orada bulunduğu için bir değişim olmaz.
[2,3,5,8,7,9,4,15,6]

İlk iki eleman dışındaki sayılar arasındaki en küçük değer olan 4, dizinin 2. indisine taşınır. Bu durumda 5 ve 4 yer değiştirir.
[2,3,4,8,7,9,5,15,6]

İlk üç eleman dışındaki sayılar arasındaki en küçük değer olan 5, dizinin 3. indisine taşınır. Bu durumda 8 ve 5 yer değiştirir.
[2,3,4,5,7,9,8,15,6]
