# Merge Sort
Bu README.md dosyası [Patika.dev-Insertion_Sort/Selection_Sort](https://app.patika.dev/courses/veri-yapilari-ve-algoritmalar/insertion-sort-proje) alıştırmaları kapsamında hazırlanmıştır.

### Alıştırma Sorusu :

    [16,21,11,8,12,22] -> Merge Sort

    Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
    Big-O gösterimini yazınız.

### Cevap :

Merge sort, verilen diziyi böl-sorgula-birleştir yöntemi kullanarak bölen ve sıralamak için kullanan bir sıralama algoritmasıdır. Aşağıda verilen dizi için uygulanan adımlar:

    1. [16,21,11,8,12,22] -> Dizi başlangıçta sıralı değil
    1. [16,21,11,8], [12,22] -> Dizi ikiye bölünür
    1. [16,21], [11,8], [12,22] -> Her alt-dizi ayrı ayrı ikiye bölünür
    1. [16], [21], [11], [8], [12], [22] -> Her alt-dizi daha da ikiye bölünür
    1. [16,21], [8,11], [12,22] -> Her alt-dizi sıralanır ve birleştirilir
    1. [8,11,16,21], [12,22] -> Birleştirilmiş diziler sıralanır ve birleştirilir
    1. [8,11,12,16,21,22] -> Son olarak, dizi sıralanmıştır.

    Sonuç: [8,11,12,16,21,22] -> Dizi sıralanmıştır.

Merge sort'un Big-O değeri, **O(nlogn)** 'dir. Çünkü dizi n elemandan oluştuğu için, her bölme işlemi log n adımda gerçekleşir ve her adımda n elemana karşı işlem yapılır.