# API
## API nedir, Winform’dan farkları nelerdir detaylı açıklayınız.
API, istemci ve sunucu arasında veri alışverişini sağlayan aracıdır. Farklı yazılımların birbiriyle doğrudan iletişim kurarak veri alışverişi yapabilmrsini sağlar.  Winform, masaüstü uygulama geliştirmek için kullanılır, kullanıcı arayüzü oluşturur. API ve Winform birlikte kullanılabilirler.

| Özellik              | API                             | WinForms                   |
| -------------------- | ------------------------------- | -------------------------- |
| Amaç                 | Sistemler arası veri alışverişi | Masaüstü arayüz geliştirme |
| Çalışma Ortamı       | Sunucu (Server)                 | Kullanıcı bilgisayarı      |
| Arayüz Var mı?       | Hayır                           | Evet                       |
| İnternet Gerekir mi? | Genellikle evet                 | Hayır                      |
| Platform             | Web, mobil, masaüstü fark etmez | Sadece Windows             |
| Kullanım Amacı       | Veri sağlamak                   | Kullanıcı ile etkileşim    |
| Fronrend, Backend?   | Backend                         | Frontend                   |

## Client ve Server nedir? Winform bir client mıdır?
**Client (İstemci)**
Kullanıcı,Müşteri anlamına gelir. Sunucuya isteğini belirten taraftır. Bir client olarak serverdan istekte bulunduğumuzda Request(istek) göndermiş olunur.

**Server (Sunucu)**
Clientten gelen isteğin karşılığını veren taraftır. Clientin isteğine göre cevap döndürür yani Response(cevap) yapılmış olur.

-- Winform bir Clienttir çünkü kullanıcıdan veri alır ve API'ye istek gönderir sonra da server'dan gelen sonucu gösterir.

## HTTP nedir, GET, POST, PUT, DELETE ne işe yarar?
HTTP sunucuya istek gönderdiğimizde ne istedğimi belirtmemizi sağlar.

1. **GET**: Sunucudan veri almak için kullanılır
2. **POST**: Yeni veri eklemek ve oluşturmak için kullanılır
3. **PUT**: Veriyi güncellemek için kullanılır     
4. **DELETE**: Veriyi silmek için kullanılır

## Bir API nasıl test edilir ve kullanılır?
Yapılan veri alış verişinin test edilmesi hata var mı diye kontrol edilmesin işlemlerin gözlemlenmesi için yapılan bir testtir. API testleri, işlevsellik, performans, sürüm, güvenlik ve kullanılabilirlik güvencesi sağlar.
API kullanımında önce API bilgileri öğrenilir sonra HTTP isteği gönderilir dönen cevap alınır ve gelen veri işlenir.

## Swagger nedir ve nasıl kullanılır?
API'leri belgeler, test eder, görselleştirir. API'lerin hangi HTTP metodlarını kullandığını, hangi endpointlere sahip olduğunu, ne tür veri döndüğü ve hangi paremetleri kullandığını gösterir.
**Swagger**, Web API projelerinde endpoint’leri görüntülemek ve test etmek için kullanılan bir araçtır. ASP.NET Core projesine Swagger paketi eklendikten sonra gerekli ayarlar yapılır ve uygulama çalıştırıldığında genellikle `/swagger` adresi üzerinden arayüz açılır. Bu arayüzde API’nin tüm GET, POST, PUT ve DELETE endpoint’leri listelenir. Kullanıcı “Try it out” butonuna basarak parametre girer ve “Execute” ile isteği gönderir; Swagger da HTTP durum kodunu ve dönen JSON veriyi gösterir. Böylece API hem dokümante edilmiş olur hem de kolayca test edilebilir.

## Postman nedir ve nasıl kullanılır?
Postman API testlerini yapma, hataları hızlıca bulma, API belgelerini oluşturma paylaşma, işbirliği yapıldığında belgeleri paylaşabilmek için kullanılır.
**Postman**, öncelikle istek türü seçilir, API’nin URL adresi girilir ve gerekiyorsa Body kısmına JSON veri eklenir. Ardından “Send” butonuna basılarak istek gönderilir. Postman, sunucudan dönen HTTP durum kodunu (200, 404, 500 vb.) ve response içeriğini ekranda gösterir. Bu sayede API’nin doğru çalışıp çalışmadığı kolayca test edilir.

## Bir API nerede çalışır?
Sunucu(server) üzerinde çalışı. istemciden(client)den gelen isteğikarşılayan backend tarafıdır.




