# 18 Kasım 2026 | Fonların 28 Ağustos sabit-pay MTM'si ve TLREF OIS ile Tera tasfiye PV

**Güncel merkez tahmin, zarar olarak:** 28 Ağustos 2026'ya göre **5.774,64 milyar TL**. Son eşleştirilmiş piyasa kapanışı 17 Kasım; 400 emeklilik fonunun en son veri etiketli fiyatı 18 Kasım 2026. Bu son veri fiyatı 17 Kasım borsa kapanışıyla eş zamanlı kesin bir müşteri MTM'si değil.

## İlkeler ve en büyük metodoloji düzeltmesi

Fonun **ara ödemesi**, müşterinin tüm başlangıç varlığına oranla tahsil ettiği nihai değer değildir. SPK 76/1903, fon başına ve kişi başına en çok 1 milyon TL ödemeyi, küçük hesaplara ve para piyasası fonlarına önceliği, net yatırım tutarına göre ödeme tavanını belirler. Bu nedenle 15 Kasım itibarıyla **Tera, Pusula, Atlas'taki 25 olağanüstü fonun toplam 93 milyar TL ödemesi**, **830 milyar TL 16 Eylül fon büyüklüğünün %11,2'si** olmasına rağmen, kendiliğinden nihai tahsilat %11,2 demek değildir. Ayrı bir varsayım olarak Tera'ya **75 milyar TL**, Pusula + Atlas'a **18 milyar TL** ara ödeme atandı. İstisnaen hisse ayni dağıtımları da ayrıca piyasa değeriyle yeniden ölçülür; ödeme ve kalan hak **iki kere sayılmaz**.

**Ekonomik tezim:** İlk modeldeki Tera için **%53,83 nihai tahsilat**, TL fon yatırımcısı açısından PV olarak yüksek. TP2 para piyasası fonunun geri kazanım kapasitesi önemli olmakla birlikte ters repo ve ilişkili şirket kıymetleri, fonlara yapılan yatırımlar ve hissenin fiili blok satış maliyeti ayrı ayrı dikkate alındığında bu eski oranı tüm Tera pozisyonuna teşmil etmek gereksiz iyimser. **16 Eylül NAV'a göre brüt nihai tahsilat %43,77; nakde dönüş süresini 17 Kasım OIS ile iskonto edince bugünkü değer %38,01.** 28 Ağustos fon dağılımıyla ağırlıklandırılınca aynı PV oranı **%39,08**.

## Gözlenen 28 Ağustos fon tabanı — yeni yüklenen 2.027 YAT fonu

28.08.2026 tarihli `Pasted text(20261118-101052).txt` içindeki 2.027 kodun NAV toplamı **9.801,64101 milyar TL**. Bu toplam tarihli günlük YAT fon özetindeki **9.801,64** milyar TL ile yuvarlama düzeyinde tutarlı. İlk SPK 17 Eylül Tera tasfiye kapsamındaki 6 fonun 28 Ağustos NAV'ları aşağıdaki gibi.

| Kod | Fon / tür | 28 Ağustos fon NAV, milyar TL |
|---|---|---:|
| TP2 | Tera para piyasası | **205,06945** |
| TLY | Tera birinci serbest / yoğun hisse | **273,00196** |
| THF | Tera hisse senedi | **59,35456** |
| T3B + DOH + TLV | Diğer ilk Tera fonları | **27,63475** |
| **Altı fon** | | **565,06072** |

Bu NAV, eski HTML modelinin Tera 565,06 milyar TL başlangıç maruziyetini bağımsız olarak doğrular. Aynı dosyada Pusula kuruculu 19 fon toplam **431,03** milyar TL, bunların 26 Ekim genişlemesi öncesindeki **12 ilk tasfiye fonu 375,65793** milyar TL; fark tasfiye kapsamının zaman içinde genişlemesinden kaynaklanıyor. Pusula'nın 16 Eylül ilk 12 fon NAV'ı ikincil taramalarda **64–72 milyar TL**, Eylül 1–16 tahmini net akımı **−132 milyar TL** bildiriliyor. Yalnızca fon değeri farkından −300 milyar TL MTM çıkarmak, öncesindeki yatırımcı satışlarını ve fonlar arası işlemleri hasara yazmak olacağından yapılmadı. Şimşek 6 Kasım TBMM görüşmesinde 1–16 Eylül'de gözlenen 401 milyar TL fon hareketinin **306 milyar TL'sinin fon içi/grup içi** olduğunu belirtti. Tüzel kesim ve fonlar arası payların **çifte sayımını** önlemek zorunlu.

## 28 Ağustos — 18 Kasım EMK ve BYF, kod bazlı sabit pay miktarı

`Fon_Verileri_EXCEL_Tum_Veri_2026-11-18 (4).xlsx` 400 adet EMK fonunun 28 Ağustos fiyat/pay/FTD'sini, `(1).xlsx` 400 adet EMK fonunun 18 Kasım fiyat/pay/FTD'sini içeriyor. **400 fonun tamamı kod bazında eşleşiyor.** Sabit 28 Ağustos pay adedi için `Σ q_28 × p_18 − Σ NAV_28 = −145,02224` milyar TL. `Σ NAV_28 = 2.652,94992`, `Σ q_28 p_18 = 2.507,92767`, güncel raporlanan toplam 18 Kasım fon NAV'ı `2.540,55633` milyar TL. Aradaki **+32,62866** milyar TL **pay adedi/fon stoğu** değişiminin 18 Kasım fiyatıyla karşılığı, piyasa kazancı değil. Ağustos sabit pay getirisi **−%5,46645**. Bu gerçekten tek tek fiyatlardan hesaplanan fiyat etkisi, eski kategorik beta simülasyonu değildir.

`(5).xlsx` 28 Ağustos **30 BYF**, `(2).xlsx` 18 Kasım **36 BYF** içeriyor. Eşleşen 30 fon için eski toplam `381,08127`, sabit eski payın yeni fiyat değeri `336,12967`, **fiyat etkisi −44,95160 milyar TL (−%11,79580)**. Yeni 6 kod **EOZ, EYZ, OAK, ODY, ZBY, ZKL**. 18 Kasım bütün 36 fonun toplamı `375,80560` milyar TL. Mevcut fonların ihraç/itfaları ve altı yeni fonun toplam etkisi **+39,67593** milyar TL; bu tutara net müşteri nakit akımı deme. BYF'ler başka fonlar tarafından tutulabilir; bu **−44,95 milyar TL** ana hanehalkı zararı üzerine ayrıca eklenmiyor.

**EMK güncellemesi:** Eski 17 Kasım modelinde EMK fon kaybı `−107,3182 − 24,8560 = −132,1742` milyar TL idi. Yeni 400-fon sabit pay değerlemesi **−145,02224**, fark **−12,84804** milyar TL, hanehalkı toplamına aşağı yönlü düzeltme.

## 17 Kasım piyasa gözlemli TLREF OIS eğrisi ve PV yöntemi

Kaynak: https://cbonds.com/indexes/219565/ (17.11.2026 close, TRY OIS quarterly fixed vs TLREF). Repo'nun önceki sürümünde 3 yıl OIS'ten tek iskonto yapılmıyor; **tahsilatın kendi vadesindeki eğri** kullanılıyor.

| Vade | Yıllık sabit OIS (%) | ACT/365, üç aylık ödeme üzerinden approx. iskonto faktörü |
|---|---:|---:|
| 1 ay | 36,16 | 0,970 (ilk kupon için basit faiz yaklaşımı) |
| 3 ay | **36,56** | **0,916254** |
| 6 ay | **35,97** | **0,841898** |
| 9 ay | **35,48** | **0,775284** |
| 12 ay | **35,16** | **0,714506** |

Üç aylık düğümler için sabit ödeme basit 0,25 yıl varsayıldı. Spot par OIS oranlarından bootstrap yaklaşımı `DF_n = (1 − r_n × 0.25 × Σ_(j<n) DF_j) / (1 + r_n × 0.25)`. Bir yıllık `DF_1Y` 0,7145, yıllık tek ödeme varsayarak hesaplanan `1/(1+0,3516)=0,7399` **değildir**. Tam iş-günü takvimi ve OIS ödeme lag'iyle yapılan gerçek Bloomberg sıfır eğrisiyle küçük fark çıkabilir. **Ek risk primi bağımsız olarak tekrar eklenmiyor**, varlık tahsilat saç tıraşı farklı alacak türlerinde zaten uygulanıyor.

## Tera 16 Eylül fon türüne göre tahsilat ve fon başına varsayılan ara ödemeler

| Fon | 16 Eylül NAV | Şimdiye kadar ödendiği varsayılan | Nominal nihai geri kazanım | Kalan nominal tahsilat | Kalan vade | PV tüm hak | NAV'a PV oranı |
|---|---:|---:|---:|---:|---|---:|---:|
| TP2 | 224,39 | 65,00 | **%75** | 103,29 | 3 ay | **159,64** | **%71,14** |
| TLY | 243,62 | 5,00 | **%27** | 60,78 | 12 ay | **48,43** | **%19,88** |
| THF | 142,08 | 3,00 | **%30** | 39,62 | 9 ay | **33,72** | **%23,73** |
| Diğer Tera (T3B/DOH/TLV) | 70,31 | 2,00 | **%30** | 19,09 | 9 ay | **16,80** | **%23,90** |
| **Tera toplam** | **680,40** | **75,00** | **%43,77 ağırlıklı** | **222,79** | | **258,59** | **%38,01** |

**Birim milyar TL.** PV `paid_i + (NAV_16Sep_i × nominal_recovery_i − paid_i) × DF(t_i)`. Buradaki ödeme **75 milyar TL'nin fonlar arası dağılımı açıklanmış değildir**, para piyasası fonuna önce ödeme ilkesi kullanılarak bir dağılım simüle edilmiştir. Nihai tahsilatlar da belirsiz, fakat her oran açık varsayım; bu tutarlar gerçekleşmiş alacak olarak sunulmuyor. TP2 %75'in dayanağı son geçerli fon portföyünde yoğun repo/kısa araç olsa da Tera ilişikli GSYF ve kira sertifikası dahil konsantre bilanço kalemleri bulunması. TLY/THF'de %27–30 nihai varsayımı yoğun ve piyasa derinliği kısıtlı hisselerin geri alımında marjinal fiyat riskine karşı haircut. SPK 15 Kasım'da fonların sahip olduğu yoğun hisseleri ilgili ihraççıların önceki kapanış fiyatından geri almasına imkan tanıdığını açıkladı; bu iflas halinde sıfır geri kazanım değil, ancak ihraççının sermayesine taşınan likidite riski demek.

Tera'nın 28 Ağustos ilk altı fonunun fiyatı ve fondaki eski pay stoğu bu 16 Eylül fon NAV'larından farklıdır. 28 Ağustos fon **dağılımına** dört PV oranı uygulandığında `205,06945×%71,14497 + 273,00196×%19,87760 + 59,35456×%23,73301 + 27,63475×%23,89774 = 220,85354 milyar TL`. **Bu, 28 Ağustos 565,06072 milyar TL toplam başlangıç stoğunun %39,08492'si**. Sep16 fon-bazlı pay değişiminden arındırılmış bireysel fiyat serisi bulunmadığından bu işlem, baz pay sahiplerinin elde kalma katsayısını fon bazında aynı varsayar. Bu tutar kimseye ödenmiş gerçek 220,85 milyar TL değildir.

## Eski ana tahmini yeni ölçümlere köprüleme

Eski modelde 28 Ağustos Tera **hanehalkı başlangıç yatırımı 423,06** milyar TL ve hanehalkı Tera kaybı **−195,34**, dolayısıyla örtülü tahsilat `(423,06−195,34)/423,06 = %53,828`. Yeni 28 Ağustos ağırlıklı **%39,08492** PV ile hanehalkı Tera ekonomik değeri **165,35267**, ek kayıp **−62,36733 milyar TL**. Eski modelin Tera hanehalkı dışı **142,00072** milyar TL portföyüne, eski örtülü oranın aynı olduğu ve yeni oranın aynı uygulanacağı *varsayımı* ile **−20,93369** milyar TL ek Tera değerleme zararı. Bu grubun %88,84'ü yerli kurumlara, %11,16'sı yabancılara ayrılır. Bu son paylaşım **yeniden ölçülmüş MKK sahiplik bilgisi değildir**.

| Köprü | Toplam kayıp, milyar TL |
|---|---:|
| 17 Kasım önceki model | **−5.678,48795** |
| EMK 400-fon sabit-pay fiyat güncellemesi | **−12,84804** |
| Tera tüm fon PV aşağı revizyonu | **−83,30101** |
| **Revize 18 Kasım araştırma merkezi** | **−5.774,63701** |

| Kesim | Güncel revize MTM, milyar TL |
|---|---:|
| Hanehalkı | **−4.586,58672** |
| Yerli kurumlar ve tüzel | **−575,25099** |
| Yabancı | **−612,79930** |
| **Toplam** | **−5.774,63701** |

Aynı açık PV hesabıyla nihai tahsilat **stres** (TP2 %60, TLY %18, THF %20, diğer %22) olarak alınırsa toplam model kaybı **−5.826,69 milyar TL**. **İyimser** (TP2 %90, TLY %45, THF %50, diğer %50) halde toplam kayıp **−5.697,85 milyar TL**. Bu aralık sadece **Tera nihai tahsilat duyarlılığı**dır, Türkiye'nin altın stoku ve yabancı yatırımcı fiyat/akım belirsizliğini kapsamaz.

**Tezi kıran veri:** TP2, TLY, THF, T3B, DOH ve TLV için fon bazında açıklanmış toplam nakit+ayni ödemeler ile ihraççıların geri aldığı hisselerin TL karşılığı, 2027 ilk çeyreğine kadar modelde belirtilen payda ve fiyatlarla uyumlu olarak %60'ın üzerinde tahsilat PV'si yaratırsa %39 merkez varsayımı yanlıştır. Tersine, küçük hesapların ödemeleri bittikten sonra yeni tahsilat akışı durursa ve geri alınan hisse değeri hızla düşerse %39 dahi yüksek kalır.

## Kaynaklar
- Yüklenen kullanıcı dosyaları: 28 Ağustos 2.027 YAT fonu metni, 28 Ağustos 400 EMK (4), 28 Ağustos 30 BYF (5), 18 Kasım 400 EMK (1), 18 Kasım 36 BYF (2). Ham satırların tamamı kamu GitHub'ına konmadı.
- OIS: https://cbonds.com/indexes/219565/
- 15 Kasım ödeme: https://www.cnbce.com/haberler/simsekten-fon-tasfiyesi-aciklamasi-yatirimcilar-anaparalarinin-yani-sira-nemalarini-da-aldi-h41846
- SPK 76/1903 ödeme önceliği: https://www.trthaber.com/haber/ekonomi/tasfiye-edilen-fonlarda-odeme-esaslari-belli-oldu-961324.html
- SPK 15 Kasım ihraççı geri alım: https://spk.gov.tr/data/6af9d0e68f95db0bf0bea384/Bas%C4%B1n%20Duyurusu_15112026.pdf
- Tera TP2 tahmini portföy riskleri: https://fon.org.tr/fon/TP2
- SPK/Tera fon kapsamı ve fon büyüklüğü ayrımları: https://www.adnandereli.av.tr/fon/TP2.html , https://www.teradosya.com/fonlar
- TBMM fonlar arası 401/306 milyar TL düzeltmesi: https://tbmm.gov.tr/Haber/hazine-ve-maliye-bakani-simsek-tbmm-20261106021743
