# MTM Bilançosu — 18 Kasım 2026 Veri Eksikleri ve Kontrol Standardı

## Yayın durumu

- En son **tam model**: 6 Kasım 2026, 28 Ağustos başlangıcına göre toplam yaklaşık 4,69 trilyon TL. Hanehalkı -3.479, yerli şirket/kurum -559, yabancı -648 milyar TL. Bunlar gözlenen tüm nakit akımlarıyla uzlaştırılmış kesin zararlar değil, 9 Kasım'da yayımlanmış model tahminleridir.
- **Doğrulanmış güncel piyasa girdisi**: EVDS/BIST altın kapanışı 17 Kasım 2026, 6.314 TL/gr. EVDS zaman serisi CSV: [data/evds_20260828_20261117.csv](data/evds_20260828_20261117.csv).
- **Fon tasfiyesi**: SPK resmî listesi 131 fon; eski model 129 fiyatlanabilir fonu içerir. 15 Kasım açıklamasına göre 119 fon kapsamında 444.987 yatırımcıya 161 milyar TL ödenmiştir. 13 Kasım resmî açıklamasında aynı yaklaşık ödeme toplamı için 444.893 kişi açıklanmıştır; iki tarihli rakam birbiri yerine kullanılmamalıdır.
- **17 Kasım için üç kesimi içeren tam MTM toplamı henüz hesaplanmadı.** Güncellenmiş altın fiyatı, bütün risk varlıklarını ve nakit akımlarını güncellemez.

## Kullanıcıdan istenen ham dosyalar (öncelik sırası)

**P0 — Fon evreni ve ödemeler (kritik, toplam sonucu değiştirebilir).**
Tek bir Excel/CSV içinde SPK'nın 131 fonunun tümü için fon kodu, mümkünse ISIN, kurucu PYŞ, tasfiye türü, son kesin değerleme tarihi, 28.08.2026 ile 17.11.2026 arasında açıklanan her fiyat, dolaşımdaki pay sayısı, fon toplam değeri ve yatırımcıya yapılan **fon bazında tarihli** nakdi/ayni ara ve nihai ödemeler. Her ödeme için kümülatif tutar, kapanan pay miktarı ve varsa kalan alacak hakkı/varlığı ayrı sütun. MKK/SPK/KAP/Ziraat/İş Bankası/TMSF/YTM yayınlarındaki fon bazlı bilgiler kullanılabilir. Sadece 161 milyar TL genel toplamı fonlara dağıtmaya kalkmak yanlış olur. Gizli müşteri hesap bilgileri istenmiyor.

**P0 — TEFAS/KAP: 28 Ağustos–17 Kasım günlük yatırım fonu ve BES/OKS verisi.**
Tüm fon kodları, fon türleri, tarih, pay fiyatı, toplam fon değeri, dolaşımdaki pay, ihrac/redemption/dağıtım, tasfiye işaretleri, fiyatın yayımlanmadığı günlerin boş kaldığı işaretler. Özellikle 6 Kasım sonrası (7-17 Kasım) ve tasfiye fonlarının son gerçek NAV bilgisi. Fiyat yayımlanmaması sıfır değer anlamına gelmez.

**P0 — MKK VAP: yatırımcı türüne ve kıymet sınıfına göre portföy stokları.**
En az 31.08.2026, 30.09.2026, 31.10.2026 ve mevcut en son tarih, tercihen 28.08.2026 ile 17.11.2026 günlük. Boyutlar: yerli gerçek kişi, yerli tüzel kişi, yerli diğer (fon/ortaklık), yabancı gerçek kişi, yabancı tüzel kişi; pay, fon, DİBS, ÖST; yatırımcı sayısı, portföy TL değeri ve kıymet bazında adet. Çıktıda **uyruk ile yurt dışı yerleşiklik ayrı** tutulmalı. VAP'ta bu kırılım yoksa mevcut erişilebilir aylık tablolar gönderilir ve belirsizlik kayıt altına alınır.

**P1 — Bloomberg fiyat ve kurumsal işlem referansı.**
BIST'teki ilgili tüm hisseler ve varsa fonların taşımakta olduğu paylar için 28.08.2026–17.11.2026 günlük ISIN/ticker, düzeltilmiş PX_LAST, işlem günleri, temettü/nakit dağıtımı, bedelli/bedelsiz ve pay bölünmesi bilgisi. BIST 100/BIST TÜM kapanış tarihçesi. Bloomberg yalnızca fiyat ve şirket olayı kaynağıdır: sonradan değişen *yatırımcı türüne göre saklama adetlerini* tek başına sağlayamaz.

**P1 — BES/OKS EGM verisi ve fonların look-through yapısı.**
Her emeklilik fonunun 28 Ağustos ve 17 Kasım pay fiyatı, pay adedi/net varlığı, net giriş ve çıkışı, alt fon veya yatırım fonu tutuyorsa o varlığın değeri. Böylece yatırım fonu ile BES/OKS üzerinden aynı varlık iki kez sayılmaz.

**P2 — Altın stok ayrımı / senaryo aralığı.**
Eski raporun 3.700 ton yastık altı, 607 ton hanehalkı banka altını ve 60 ton şirket ticari altını stok tahminlerinin yeni resmî kaynakla test edilebildiği varsa dosyası. Bu stoklar EVDS fiyatları gibi günlük ölçülen veri değildir. 17 Kasım fiyat farkı 778 TL/gr olduğundan, 100 ton stok varsayımı yaklaşık **77,8 milyar TL** MTM sonucunu değiştirir.

## Hesaplama ilkeleri

1. **İşlem akışı ile MTM ayrımı:** Portföy stok değişimi = fiyat etkisi + net alım/satım + net ihraç/itfa + kur/yeniden sınıflama + kapsam farkı. Tek başına MKK stok farkına "zarar" denmez.
2. **Tasfiye fonları:** Fon sahibinin tarih sonu ekonomik varlığı = aldığı nakit/ayni dağıtımın değerlemesi + hâlen sahip olduğu fon paylarının *dağıtım sonrası* ekonomik değeri. Eğer NAV kalan alacak hakkını zaten içeriyorsa tekrar eklenmez. Ara ödeme sırasında katılma payı her zaman iade edilmediğinden hem ödemeyi hem eski brüt NAV'ı saymak çifte sayımdır.
3. **Anapara vs baz tarih değeri:** Hükümet açıklamasındaki "net yatırım tutarının tamamını alma" ölçüsü, 28 Ağustos portföy değerine göre MTM kaybı olmadığı anlamına gelmez. Nakit geri ödeme maliyet bazına veya usulde tarifli net yatırıma göre gerçekleşir.
4. **Çifte sayım:** Pay senetlerinin fon portföyündeki payları, fon katılma payı sahibinin portföy değeriyle aynı değer zincirine aittir. Toplamda yatırımcıların doğrudan hisseleri + fon payları sayılır; fonların altındaki hisseler tekrar eklenmez. Yerli diğer MKK hisseleri kullanılırken dikkat.
5. **Kapsam:** Borsa, fizikî/banka altını, yatırım fonları, BES/OKS (ilgili koşullarda) ve belirlenmiş diğer yatırım araçları. DTH kur kazancını hesaba katmadan bütün servetin MTM değişimi denmez; kur kazancı raporda ayrıca gösterilebilir.
6. **Tarih/hata payı:** Bütün gözlemler aynı kapanış tarihine getirilir. Tarih veya yatırımcı kesimi bazında serisi bulunmayan sonuç açıkça "model" olarak etiketlenir ve duyarlılık analizi verilir.
7. **Veri yayını:** Bloomberg Terminal lisansı veya kurum gizliliğine tabi ham veri kamusal GitHub'a kopyalanmaz. Kullanıcı tarafından erişimi uygun görülen özet istatistikler ve açık EVDS/TCMB/SPK/MKK/KAP kaynaklarına referanslar yayımlanır.

## Kaynaklar

- EVDS: TP.ALTINPIYASA.KAP02, TP.ALTINPIYASA.KAP03, TP.DK.USD.A.YTL, TP.MKNETHAR.M1.
- SPK fon sayısı: https://www.spk.gov.tr/duyurular/basin-duyurulari/2026/tasfiye-konusu-fonlardaki-yatirimci-sayisina-iliskin-aciklama
- SPK 27.10.2026 ödeme usulleri: https://www.spk.gov.tr/duyurular/basin-duyurulari/2026/basin-duyurusu_27102026
- SPK 15.11.2026 pay geri alımı: https://spk.gov.tr/duyurular/basin-duyurulari/2026/olaganustu-tasfiyede-halka-acik-ortakliklarin-geri-aldigi-paylara-iliskin-basin-duyurusu
- 13.11.2026 Fon Koordinasyon Kurulu: https://www.aa.com.tr/tr/gundem/iletisim-baskanligi-444-bin-893-yatirimciya-yaklasik-161-milyar-lira-odeme-yapilmistir/4124180
- 15.11.2026 Bakan Şimşek açıklaması: https://www.cnbce.com/haberler/simsekten-fon-tasfiyesi-aciklamasi-yatirimcilar-anaparalarinin-yani-sira-nemalarini-da-aldi-h41846
- TCMB reel sektör fon yatırımları: https://tcmb.gov.tr/wps/wcm/connect/blog/tr/main%20menu/analizler/fon_tasfiyeleri_ve_reel_sektor_firma_verileri_ne_soyluyor
