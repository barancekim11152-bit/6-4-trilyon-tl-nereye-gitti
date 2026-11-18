# 18 Kasım 2026 — Tera tasfiye nakit akımı ve kalan ekonomik hak modeli

Bu ek, ana araştırmadaki -5.678,49 milyar TL koşullu MTM modelinin **tasfiye bileşenini** ayrıntılandırır. 16 Eylül 2026 net fon büyüklüğü, 28 Ağustos model başlangıç pozisyonu ve 15 Kasım ödemeleri farklı tarihlere aittir. Ortak as-of verisi olmadığı için yüzde tahsilat bir **senaryo girdisidir**, gözlenen ödeme oranı değildir.

## Gözlenen büyüklükler ve zaman farkı

- 16 Eylül 2026 tarihli fon büyüklükleri: Tera'nın ilk 6 tasfiye fonunda toplam **680,40 milyar TL**. TP2 para piyasası **224,39**, TLY serbest **243,62**, THF hisse senedi yoğun **142,08**, diğer Tera fonları **70,31 milyar TL** (kalan). Kaynaklar: https://github.com/cberko/spk-tasfiye-fonlari , https://www.adnandereli.av.tr/fon/THF.html , https://www.adnandereli.av.tr/fon/TP2.html ve https://fonoloji.com/spk-tasfiye/aciklama/tera-portfoy-17-eylul-2026 .
- 15 Kasım 2026 itibarıyla 119 fonda toplam **161 milyar TL** ödeme açıklandı. Bunun yaklaşık **68 milyar TL** olağan tasfiyedeki A1/Bulls/Pardus/Hedef portföylerine, yaklaşık **93 milyar TL** ise olağanüstü tasfiyedeki **Tera, Pusula, Atlas** fonlarına ait. 93 milyar TL yalnızca Tera'ya yapılan ödeme değildir.
- Tera'da **%30 toplu ara ödeme** iddiası, 16 Eylül bazındaki 680,4 milyar TL için **204,12 milyar TL** nakit gerektirir. 15 Kasım'a kadarki üç şirketin tamamına yapılmış olağanüstü ödeme sadece 93 milyar TL olduğundan **Tera fonlarının bütün yatırımcılarına fon değerinin %30'u ödenmiş olamaz**. %30 bazı hesapların tahsilat oranı, belirli fonun kısmi tahsilatı veya asıl maliyet üzerinden sınırlı bir oran olabilir.
- SPK 76/1903'te önce para piyasası fonları ve net yatırımı küçük hesaplar gelir. **1 milyon TL ara ödeme tavanı**, maliyet bazına göre hesaplama ve hissenin henüz iade edilmiyor oluşu nedeniyle tekil hak sahibi bazında oranlarla toplam portföy oranı farklıdır. https://www.spk.gov.tr/duyurular/basin-duyurulari/2026/basin-duyurusu_27102026
- İlk 6 fonun 16 Eylül toplamıyla Eylül sonundaki/28 Ağustos sonundaki mevduat veya fon stoklarını aynı birim sanıp karşılaştırmak yanlış olur. Yatırımcı çıkışları ve fonlar arası yatırımlar paydayı değiştirebilir.

## Tera için seçilen sektör-spesifik **nihai** tahsilat senaryosu

Burada nihai geri kazanım, **fonun 16 Eylül nominal yayımlanmış varlık değeri üzerinden** fiyat/likidite kaybı sonrası yatırımcının eline geçebilecek ekonomik değer oranıdır; tarihte ödenen ara ödeme oranı değildir.

| Fon grubu | 16 Eylül NAV, milyar TL | Varsayılan nihai tahsilat | Nihai ekonomik değer, milyar TL | Neden |
|---|---:|---:|---:|---|
| TP2 para piyasası | 224,39 | **%85** | **190,73** | Para piyasasına ödeme önceliği; fonun geri dönüştürülmesi gereken yoğun/repo ve olası likit olmayan pozisyonları yüzünden %100 varsayılmıyor |
| TLY serbest, hisse yoğun maruziyet | 243,62 | **%35** | **85,27** | 16 Eylül TEFAS dağılımında yaklaşık %87 hisse; yoğun pozisyon, geri alım fiyatı ve tasfiye sürtünmesi |
| THF hisse senedi yoğun | 142,08 | **%40** | **56,83** | 1 Ekim dağılımında yaklaşık %85 hisse; fiyat, emir derinliği ve fon katılma paylarının çifte sayım riski |
| Diğer Tera fonları | 70,31 | **%45** | **31,64** | DOH/TLV/T3B ve diğerleri karışık; alt grup basitleştirmesi |
| **Toplam** | **680,40** | **%53,57 ağırlıklı** | **364,47** | Nihai geri kazanım senaryosu, teyit edilmiş tasfiye fiyatı değildir |

Tera, Pusula ve Atlas'ın 16 Eylül sırasıyla **680,4 / 71,8 / 78,0 milyar TL** stokları bazında, olağanüstü **93 milyar TL** ara ödemenin sadece kaba büyüklük-ağırlıklı tahsisi Tera için **76,2 milyar TL** üretir. Hesapları basitleştirmek ve küçük hesaplara önceliği dikkate almak için Tera'ya **75 milyar TL** ara ödeme payı *varsayıldı*. Böylece Tera'nın **nihai beklenen toplam ekonomik değeri 364,47 milyar TL** içinde **75 milyar TL'si ara ödenmiş, yaklaşık 289,47 milyar TL'si ileride tahsil edilebilecek bugünkü ekonomik değer** olarak modellenir. **289,47 milyar TL hukuken açıklanmış alacak, hesapta görülen NAV veya garantili ödeme değildir.** Gelecek tarihler için iskonto/finansman maliyeti ayrıca uygulanırsa bugünkü ekonomik değer daha düşüktür. 75 milyarı 364,47'ye tekrar **eklemek çifte sayım** olur.

Pusula ve Atlas'a birlikte kalan **18 milyar TL** bu basit tahsisin tamamlayıcısıdır. Özellikle Tera para piyasası fonunun önceliği nedeniyle gerçek ödeme payları bu oransal dağılımdan farklı olabilir. Seçilen tahsilat oranları yeni bir kayıp tutarı **doğrudan ana toplamın üzerine eklenmeden** eski modelle çapraz kontrol edildi.

## Eski MTM modeline uyum, çifte sayımı önleme ve stres

Önceki HTML'in gömülü modelinde 28 Ağustos Tera için **toplam 565,06**, bunun **hanehalkı payı 423,06 milyar TL**. Hanehalkı Tera MTM hesabı **-195,34 milyar TL**; dolayısıyla modelde zaten **227,72 milyar TL (%53,83) ekonomik değer korunmuş**. Yeni kompozisyon-ağırlıklı Tera **%53,57** nihai tahsilat varsayımı bu eski örtülü varsayımla hemen hemen aynıdır. **Dolayısıyla 93 milyar TL ara ödemeyi ana MTM toplamına eklemiyoruz; -5,68 trilyon TL merkez modelini koruyoruz.**

Bu oran nihai %30 olursa, sadece hanehalkının 423,06 milyar TL Tera başlangıç portföyünde beklenen kayıp **-296,14 milyar TL** olur (eski -195,34 yerine). Hanehalkı model kaybına **+100,80 milyar TL** olumsuz fark eklenir ve diğer yatırımcılar değiştirilmezse toplam kayıp **-5,779 trilyon TL** olur. Nihai %50 varsayımıyla hanehalkı ek kayıp **16,19 milyar TL**, toplam **-5,695 trilyon TL**; nihai %60 varsayımıyla hanehalkı beklenen kayıp 26,12 milyar TL azalır ve toplam **-5,652 trilyon TL**. Yatırımcı türüne göre farklı oransal tahsilat ve diğer Tera fonları için farklı değerlemeler ayrıca doğrulanmalıdır.

Bu stres, 16 Eylül Tera tam fon evreninin (680,4) 28 Ağustos hanehalkı alt kümesinin (423,06) üzerine toplanması değildir. Ayrıca ana fon MTM modelinin fonlar arası pay sahipliği ve fon fiyatları nedeniyle orijinalde hata payı vardır.

## Piyasada görünmeyen risk taşıyıcısı

SPK 15 Kasım açıklaması, tasfiye fonlarının yoğun hisse senedi varlıklarının doğrudan piyasaya sürülmesi yerine ilgili ihraççıların **önceki borsa kapanışından geri alım** yapabilmesine olanak tanındığını açıkça belirtti. Bu, satış baskısını ve tasfiyenin fiyat kaymasını azaltabilir ancak riski yok etmez: **illikit hissenin taşıma yükü ihraççıya ve mevcut ortaklara devredilir**, ihraççı geri alım kapasitesi zayıfsa nihai fon tahsilatı hâlâ düşer. Bu yüzden hisse yoğun fonlarda kamuya yansıyan ara ödeme tutarı piyasa fiyatından beklenebilecek nihai geri kazanım için tek başına doğru gösterge değildir.

Kaynak: https://spk.gov.tr/data/6af9d0e68f95db0bf0bea384/Bas%C4%B1n%20Duyurusu_15112026.pdf

**En ucuz stres testi:** İhraççılarca geri alınan fon hisselerinin **adet × son kapanış TL değeri** ile tasfiye bankalarının tuttuğu hisse adedi ayrı yayımlanırsa TLY/THF tahsilat oranları revize edilir. Tera'nın 16 Eylül fon büyüklüğü, nihai tahsilat senaryosu ve 15 Kasım ara ödeme toplamı tarih itibarıyla eşitlenmeden bir fonun bilançosu olarak birbirine eklenmez.
