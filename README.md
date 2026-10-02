<p align="center">
  <img src="assets/logo.png" alt="crk-pos logosu" width="160" />
</p>

<h1 align="center">crk-pos</h1>

**crk-pos** için herkese açık sürüm indirme sayfası. crk-pos; Windows, macOS ve Linux üzerinde çalışan bir satış noktası (POS) uygulamasıdır.

## crk-pos nedir?

crk-pos; küçük ve orta ölçekli işletmeler (market, büfe, bar gibi) için geliştirilmiş, kasa başında hızlı satış yapmayı ve günlük hesabı derli toplu tutmayı sağlayan bir satış noktası uygulamasıdır. Tablet ve masaüstünde çalışır.

### Hangi sorunları çözer?

- **Kuyruk yapmadan hızlı satış:** Barkod okutarak ya da favori ürünlere tek dokunuşla satış yapılır. Ürün bulunamazsa veya stok yetmezse sesli ve görsel uyarı verir. Nakit, kart, parçalı ödeme, veresiye ve bedelsiz satış desteklenir.
- **Defter yerine veresiye takibi:** Müşteri borçları, tahsilatlar ve alınan ürünler tek yerde tutulur. Eski defterdeki borçlar elle aktarılabilir, aynı kişinin farklı adlarla açılmış kayıtları birleştirilebilir, güvenilmez müşteriler işaretlenebilir.
- **Kasa farkını görünür kılmak:** Gün sonunda sayılan nakit ve kart, uygulamanın hesapladığı tutarla karşılaştırılır; eksik veya fazla varsa gösterilir.
- **Ciro ve satış görünürlüğü:** Günlük, aylık ve yıllık satışlar ödeme yöntemine göre, en çok satan ürünler ve önceki dönemle karşılaştırmalarla izlenir.
- **Stok ve ürün yönetimi:** Ürünler, kategoriler, fotoğraflar, stok sayımı ve favoriler tek ekrandan yönetilir.
- **Tedarikçi ödemeleri:** Bu hafta ödenecek, geciken ve ödenen tutarlar ödeme takvimiyle takip edilir.

➡️ **[Son sürüm](https://github.com/galaxisforge/crk-pos-releases/releases/latest)** · [Tüm sürümler](https://github.com/galaxisforge/crk-pos-releases/releases)

## İndirme

[Son sürüm](https://github.com/galaxisforge/crk-pos-releases/releases/latest) sayfasını açın ve **Assets** listesinden sisteminize uygun dosyayı seçin:

| İşletim sistemi | Önerilen dosya | Alternatifler |
|---|---|---|
| Windows 10/11 (64 bit) | `crk-pos_<sürüm>_x64-setup.exe` | `crk-pos_<sürüm>_x64_en-US.msi` |
| macOS (Intel ve Apple Silicon) | `crk-pos_<sürüm>_universal.dmg` | — |
| Linux, Debian/Ubuntu | `crk-pos_<sürüm>_amd64.deb` | `.AppImage` |
| Linux, Fedora/RHEL/openSUSE | `crk-pos-<sürüm>-1.x86_64.rpm` | `.AppImage` |
| Linux, herhangi bir dağıtım | `crk-pos_<sürüm>_amd64.AppImage` | — |

`<sürüm>`, sürüm numarasıdır (örn. `0.15.0`). `.sig`, `.tar.gz` ve `latest.json` dosyalarını indirmenize gerek yok; bunlar uygulamanın otomatik güncelleyicisi içindir.

## Kurulum

### Windows

1. `x64-setup.exe` kurulum dosyasını indirin.
2. Çift tıklayıp kurulum sihirbazını izleyin.
3. Windows SmartScreen "Windows bilgisayarınızı korudu" uyarısı gösterirse **Ek bilgi → Yine de çalıştır**'a tıklayın.
4. Başlat menüsünden **crk-pos**'u açın.

Kurumsal/IT yönetimli bilgisayarlarda `.msi` kullanılabilir, örn. `msiexec /i crk-pos_<sürüm>_x64_en-US.msi /qn`.

### macOS

1. `.dmg` dosyasını indirin (Intel ve Apple Silicon için tek, evrensel sürüm).
2. Dosyayı açıp **crk-pos**'u **Uygulamalar** klasörüne sürükleyin.
3. İlk açılışta macOS "geliştirici doğrulanamadığı için açılamıyor" derse uygulamaya sağ tıklayın (veya Control + tıklayın), **Aç**'ı seçin ve onaylayın. Alternatif olarak **Sistem Ayarları → Gizlilik ve Güvenlik** bölümünden **Yine de Aç**'a tıklayın.

### Linux

**Debian / Ubuntu (.deb)**

```bash
sudo apt install ./crk-pos_<sürüm>_amd64.deb
```

**Fedora / RHEL / openSUSE (.rpm)**

```bash
sudo dnf install ./crk-pos-<sürüm>-1.x86_64.rpm    # Fedora / RHEL
sudo zypper install ./crk-pos-<sürüm>-1.x86_64.rpm # openSUSE
```

**AppImage (her dağıtımda, kurulum gerektirmez)**

```bash
chmod +x crk-pos_<sürüm>_amd64.AppImage
./crk-pos_<sürüm>_amd64.AppImage
```

AppImage açılmazsa FUSE 2'yi kurun (Ubuntu 22.04+ için `sudo apt install libfuse2`) ya da `--appimage-extract-and-run` parametresiyle çalıştırın.

## Güncelleme

crk-pos güncellemeleri otomatik kontrol eder ve yeni sürümü kurmayı önerir. Ayrıca [sürümler sayfasından](https://github.com/galaxisforge/crk-pos-releases/releases/latest) en yeni kurulum dosyasını indirip mevcut sürümün üzerine kurabilirsiniz. Verileriniz korunur.

## Kaldırma

- **Windows:** Ayarlar → Uygulamalar → Yüklü uygulamalar → crk-pos → Kaldır
- **macOS:** **crk-pos**'u Uygulamalar klasöründen Çöp Sepeti'ne sürükleyin
- **Linux:** `sudo apt remove crk-pos` / `sudo dnf remove crk-pos` / AppImage dosyasını silin

## Sorun bildirimi

Hata mı buldunuz ya da bir isteğiniz mi var? [Issue açın](https://github.com/galaxisforge/crk-pos-releases/issues).
