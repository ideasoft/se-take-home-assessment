# Ideasoft Take-Home Assesment

## Prosedür
- Lütfen bu görev için bir github reposu açın ve adresini bizimle paylaşın.
- Görevin tamamlanacağı yazılım dili PHP'dir.
- Tercih ettiğiniz library veya framework'ü kullanabilirsiniz.
- Veritabanı, kuyruk vb. 3.ncü parti araçları gerektiren görevlerde ürün/teknoloji sınırlaması yoktur.
- Dilediğiniz dış kaynaklardan faydalanabilirsiniz. Lütfen kullandığınız dış kaynak ve kodları görev içerisinde yorum olarak belirtin.

Bu görevde herhangi bir zaman sınırlaması bulunmamaktadır.

## Docker
Görev geliştirmesi Docker platformu üzerinde ayağa kaldırılıp test edilebilmelidir.

## Veriler
Örnek JSON dosyalarına [example-data](./example-data) klasöründen ulaşabilirsiniz.

## Sorularınız Varsa
Eğer görevde net olmayan noktalar olduğunu düşünüyorsanız, lütfen bizimle iletişime geçmekten çekinmeyin.

---

## Görev 1 - Siparişler
Siparişler için, ekleme / silme / listeleme işlemlerinin gerçekleştirilebileceği bir **RESTful** API servisi oluşturun.

### Sipariş Kuralları Nedir?
- Yeni sipariş eklenirken, satın alınan ürünün stoğu yeterli değilse (**products.stock**) bir hata mesajı döndürün.
- Payload validasyonu gerçekleştirin.

### Örnek Data:
- [orders.json](./example-data/orders.json)
- [products.json](./example-data/products.json)
- [customers.json](./example-data/customers.json)

## Görev 2 - İndirimler
Verilen siparişler için indirimleri hesaplayan küçük bir **RESTful** API servisi oluşturun.

### İndirim Kuralları Nedir?
- Toplam 1000TL ve üzerinde alışveriş yapan bir müşteri, siparişin tamamından %10 indirim kazanır.
- **2** ID'li kategoriye ait bir üründen 6 adet satın alındığında, bir tanesi ücretsiz olarak verilir.
- **1** ID'li kategoriden iki veya daha fazla ürün satın alındığında, en ucuz ürüne %20 indirim yapılır.

Lütfen gelecekte daha fazla indirim kuralı eklenebileceğini göz önünde bulundurun.

### Örnek Cevap:
- [discount.response.json](./example-data/discount.response.json)
