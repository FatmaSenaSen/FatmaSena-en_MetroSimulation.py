Sürücüsüz Metro Simülasyonu (Rota Optimizasyonu)
BFS ve A* algoritmalarını kullanarak en kısa ve en hızlı rotayı belirlemek amacıyla python dili ile yazılmış bir projedir.
Kullanılan collections.defaultdict değer atanabilen bir dictionary türüdür.
Collection.deque double-ended queue veri yapısıdır.
BFS algoritmasında hızlı ekleme ve çıkarma işlemleri ile en az aktarmayı bulmak için kullanırız.
Heapq, A* algoritmasında en hızlı rotayı bulmak için kullanırız.
BFS(Breadth First Search) en yakın komşuları önce ziyaret eder , daha sonra derinlerdeki düğüme gider. 
Buradaki temel amaç iki hedef arasındaki en kısa mesafayi bulmaktır.
BFS ilk giren ilk çıkar mantığı olan FIFO mantığına sahiptir.
Kuyruk(queue) yapısını kullanarak istasyonları ziyaret eder.
A* algoritması, sezgisel bir yol bulma algoritmasıdır. 
Hem gidilen yolun maliyetini hem de hedefe olan tahimini uzaklığı ele alarak yolu bulur. 
Öncelikli kuyruk (heapq) kullanılır.
Heuristic(sezgisel fonksiyon) ile daha hızlı çalışır.

Kodu çalıştırınca çıkan sonuç budur :
=== Test Senaryoları ===

1. AŞTİ'den OSB'ye:
En az aktarmalı rota: AŞTİ -> Kızılay -> Kızılay -> Ulus -> Demetevler -> OSB
En hızlı rota (25 dakika): AŞTİ -> Kızılay -> Kızılay -> Ulus -> Demetevler -> OSB

2. Batıkent'ten Keçiören'e:
En az aktarmalı rota: Batıkent -> Demetevler -> Gar -> Keçiören
En hızlı rota (21 dakika): Batıkent -> Demetevler -> Gar -> Keçiören

3. Keçiören'den AŞTİ'ye:
En az aktarmalı rota: Keçiören -> Gar -> Gar -> Sıhhiye -> Kızılay -> AŞTİ
En hızlı rota (19 dakika): Keçiören -> Gar -> Gar -> Sıhhiye -> Kızılay -> AŞTİ

Kaynakça :
https://tr.wikipedia.org/wiki/A*_arama_algoritmas%C4%B1
https://medium.com/tapu-com-bak%C4%B1%C5%9F-a%C3%A7%C4%B1s%C4%B1/bfs-breath-first-search-geni%C5%9F-%C3%B6ncelikli-arama-algoritmas%C4%B1n%C4%B1-tan%C4%B1yal%C4%B1m-ec7050a41af
https://www.btkakademi.gov.tr/portal/course/yapay-zeka-ve-algoritmalarina-giris-17500
https://www.btkakademi.gov.tr/portal/course/sifirdan-ileri-seviye-python-programlama-5877
