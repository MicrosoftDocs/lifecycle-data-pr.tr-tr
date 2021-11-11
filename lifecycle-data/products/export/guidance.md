---
title: Yaşam döngüsü verilerini dışa aktarma kılavuzu
description: Ürün yaşam döngüsü verilerini dışarı aktarma kılavuzu
ms.date: 12/16/2020
layout: ContentPage
ms.openlocfilehash: 5e9dddbff5fac32e6d3cf8ef0943151d2dfe5e35
ms.sourcegitcommit: 6ea3221fd5475440480515f04f33988656d71748
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/02/2021
ms.locfileid: "3546988"
---
# <a name="lifecycle-data-export-guidance"></a>Yaşam döngüsü verilerini dışa aktarma kılavuzu
Bu belge, ürün dışarı aktarma dosyasının nasıl kullanılacağını açıklar.

## <a name="query-information"></a>Sorgu Bilgileri
Excel belgesinde, ürün tablosunda doldurulan verileri belirlemeye yardımcı olacak alanlar vardır.

### <a name="end-of-support"></a>Destek Bitişi
Destek bitişi değeri ürünleri, destek sonu tarihi veya sürüm bitiş tarihlerine göre filtreleyecektir.

Olası değerler: Tüm (filtre uygulanmadı), Yıl ve bir Aralık.

### <a name="family"></a>Aile
Aile değeri, aile olarak bilinen hiyerarşi içinde ürünleri üst düzeyine göre filtreler.

Olası değerler: Tüm (filtre uygulanmadı), Aile Adı

### <a name="group"></a>Grup
Grup değeri, üst düzeyindeki (aile) ürünleri belirli bir grup olarak filtreler.

Olası değerler: Tüm (filtre uygulanmadı), Grup Adı

## <a name="table-columns"></a>Tablo Sütunları
Ürün tablosu, ürünü, sürümleri, yayınları ve ilgili destek tarihlerini tanımlayan sütunlardan oluşur.

> [!NOTE]
> Her ürün, sürüm ve yayın bileşimi için bir satır olacaktır.

### <a name="product"></a>Ürün
Ürün adı.

### <a name="edition"></a>Edition
Sürüm sütunu, üründe sürümler olduğunda doldurulur. Ürün sürümü olmadığında, bu alan boş olacaktır.

### <a name="release"></a>Sürüm
Ürün birden çok yayın içeriyorsa, yayın sütunu doldurulur.
Ürünün yalnızca bir yayını olduğunda, bu alan boş olacaktır.

### <a name="support-policy"></a>Destek İlkesi
Bu alan, ürünün hangi destek ilkesini izlediğini tanımlar.

Olası değerler: [Sabit](/lifecycle/policies/fixed), [Modern](/lifecycle/policies/modern), Bileşen

### <a name="start-date"></a>Başlangıç Tarihi:
Ürün için desteğin başlangıç tarihi.

### <a name="mainstream-date"></a>Temel Tarih
Destek İlkesi **Sabit** veya **Bileşen** olduğunda bu, ürünün temel bitiş tarihidir.
  
Destek İlkesi **Modern** olduğunda, bu alan boş olacaktır.

### <a name="extended-end-date"></a>Genişletilmiş Bitiş Tarih
Destek İlkesi **Sabit** veya **Bileşen** olduğunda bu, ürünün genişletilmiş bitiş tarihidir.

Destek İlkesi **Modern** olduğunda, bu alan boş olacaktır.

### <a name="retirement-date"></a>Kullanımdan Kaldırılma Tarihi
Destek İlkesi **Sabit** veya **Bileşen** olduğunda bu boş olur.

Destek İlkesi **Modern** olduğunda bu, ürünün kullanımdan kaldırılma tarihi olur.

### <a name="release-start-date"></a>Yayın Başlangıç Tarihi
Yayın için desteğin başlangıç tarihi. Ürünün yalnızca bir yayını olduğunda, bu alan boş olacaktır.
 
### <a name="release-end-date"></a>Yayın Bitiş Tarihi
Yayın için desteğin bitiş tarihi.
Ürünün yalnızca bir yayını olduğunda, bu alan boş olacaktır.

### <a name="docs-url"></a>Belgeler Url'si
Genişletilmiş belgelemenin URL'si.
