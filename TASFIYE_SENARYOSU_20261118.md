# 18 Kasım 2026 — Tera fonları için ödeme ve risk-ayarlı tahsilat simülasyonu

**Bu belge, 17 Kasım piyasa eğrisi ve 28 Ağustos pay bazlı güncelleme ile yeniden hesaplandı.** Önceki sürümdeki **%53,57 nihai tahsilat** modeli, iskonto süresini ve TLY/THF varlık riski yoğunlaşmasını doğru yansıtmadığı için **merkez görüş olmaktan çıkarıldı**.

Tam hesap, grup ağırlıkları, SPK nakit ödeme kuralları, 17 Kasım OIS bootstrap ve 28 Ağustos yeni fon verileri için [OIS_PV_YENIDEN_DEGERLEME_20261118.md](OIS_PV_YENIDEN_DEGERLEME_20261118.md) esas alınır.

**Merkez, 16 Eylül Tera fon stokuna göre %43,77 nominal nihai tahsilat, OIS'e göre %38,01 PV; 28 Ağustos portföy karışımıyla %39,08 PV.** İlk altı Tera fonunun 28 Ağustos toplamı **565,06072 milyar TL**. SPK 15 Kasım'a kadar Tera/Pusula/Atlas'a **toplam 93 milyar TL** ödeme açıklandı. Tera payı burada **75 milyar TL model varsayımı**.

| Fon | 16 Eylül NAV (mlr TL) | Nihai nominal % | Ara ödenen varsayım (mlr TL) | Kalan ödeme vadesi | OIS'le PV (mlr TL) |
|---|---:|---:|---:|---:|---:|
| TP2 | 224,39 | %75 | 65 | 3 ay | 159,64 |
| TLY | 243,62 | %27 | 5 | 12 ay | 48,43 |
| THF | 142,08 | %30 | 3 | 9 ay | 33,72 |
| Diğer Tera | 70,31 | %30 | 2 | 9 ay | 16,80 |
| **Toplam** | **680,40** | **%43,77** | **75** | | **258,59** |

Bu rakamlar gelecekte yapılacağı garanti edilmiş ödemeler değildir. Geçmiş ara ödemeler PV'ye zaten dahil; ikinci kez eklenmedi. SPK'nın kişi başı 1 milyon TL tavanı ve küçük yatırımcılara/para piyasası fonlarına öncelik verdiği ödeme mekanizması nedeniyle, **93/830 = %11,2** ilk tahsilat oranı **nihai tahsilat oranı değildir**. Ancak uzun ve belirsiz kalan tahsilatın bugünkü değeri çok daha düşük.

**Ana tahmine etkisi.** 28 Ağustos portföy ağırlığına uygulanan **%39,08492 PV** ile eski Tera **%53,83** varsayımından **83,30 milyar TL** ek tüm-kesim tahmini zarar hesaplandı; bunun hanehalkı **62,37 milyar TL**. Yeni 400 emeklilik fonunun ölçülmüş −12,85 milyar TL fiyat düzeltmesiyle Türkiye modeli **−5.774,64 milyar TL**. Bu, özgül Tera kurtarma riskini fiyatlayan ve 18 Kasım BES NAV'ını kullanan **koşullu** tahmindir.

**Vade sınaması:** Resmî tasfiye süresi altı ay ile sınırlı olsa da tahsilat/geri kazanım hakkının müteakip nakde dönüşüne ilişkin 9–12 ay senaryoları modele kondu. TLY, THF ve diğerlerinin bütün kalan tahsilatı 6 ayda tamamlansa model kaybı yalnız 10,28 milyar TL azalır, **5.764,36 milyar TL** olur. Nominal tahsilat saç tıraşı OIS iskonto etkisinden daha büyüktür. Endeksli net yatırım tutarı, garantili gelecekteki faiz getirisi değil dağıtım tavanı/ölçüsüdür.

**Kırılma noktası** TP2/TLY/THF için hisse geri alım bedelleri, nakit dağıtımlar ve bakiyelerin ayrı açıklanması. Kaynaklar [SPK 15 Kasım](https://spk.gov.tr/data/6af9d0e68f95db0bf0bea384/Bas%C4%B1n%20Duyurusu_15112026.pdf), [Şimşek 15 Kasım](https://www.cnbce.com/haberler/simsekten-fon-tasfiyesi-aciklamasi-yatirimcilar-anaparalarinin-yani-sira-nemalarini-da-aldi-h41846), [Cbonds 17 Kasım TL OIS](https://cbonds.com/indexes/219565/).
