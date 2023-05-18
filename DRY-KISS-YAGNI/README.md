Yazılım geliştirme sürecinde, başarılı ve etkili bir kod oluşturmanın en temel yollarından biri, tasarım prensiplerine uygun bir yaklaşımda ilerlemektir. Bu prensipler, kodun daha okunabilir, sürdürülebilir ve genel olarak daha iyi hale gelmesini sağlar.

Bu makalede, `"DRY"` (Don't Repeat Yourself - Kendini Tekrar Etme), `"KISS"` (Keep It Simple, Stupid - Basit Tut, Aptal!) ve `"YAGNI"` (You Ain’t Gonna Need It - Buna İhtiyacın Olmayacak) tasarım prensibini ele alacağız. İlk olarak DRY prensibiyle başlayalım.

## DRY - Don't Repeat Yourself

Don't Repeat Yourself, yani Kendini Tekrar Etme, yazılım geliştirme sürecinde sıkça kullanılan bir tasarım prensibidir. DRY prensibi, kodun tekrarlanmasını en aza indirerek, kodun daha okunabilir, sürdürülebilir ve yeniden kullanılabilir olmasını hedefler. DRY prensibinin temel özellikleri aşağıdadır.

- Tek Bir Kaynak: DRY prensibi, kodda bir bilginin tek bir yerde bulunmasını savunur. Yani, aynı bilginin birden fazla yerde tekrarlanması yerine, bu bilgi tek bir kaynaktan alınmalıdır. Bu sayede, bilgiyi güncellemek veya değiştirmek gerektiğinde sadece tek bir yerde düzenleme yapmak yeterli olur.

- Tekrarların Kaldırılması/Düzenlenmesi: DRY prensibi, kodun tekrarlanmasını önlemeyi amaçlar. Benzer veya aynı işlemler için tekrarlanan kod blokları yerine, bu kod blokları bir fonksiyon veya sınıf içinde yeniden kullanılabilir hale getirilmelidir. Böylelikle, hem kodun boyutu azalır hem de bakım ve iyileştirme süreci kolaylaşır.

- Bağımlılıkların Yönetimi: DRY prensibi, bağımlılıkların kontrol edilmesini ve en aza indirilmesini de amaçlar. Kodun farklı bölümlerinde aynı bağımlılıkları tekrar etmek yerine, bu bağımlılıklar ortak bir kaynaktan yönetilmelidir. Örneğin, harici bir kütüphane kullanılıyorsa, bu kütüphane yalnızca bir kez dahil edilmeli ve ilgili tüm bölümler tarafından kullanılmalıdır.

- Okunabilirlik ve Sürdürülebilirlik: DRY prensibi, kodun okunabilirliği ve sürdürülebilirliği üzerinde olumlu bir etkiye sahiptir. Tekrarlanan kod blokları yerine yeniden kullanılabilir fonksiyonlar veya sınıflar kullanmak, kodun anlaşılabilirliğini artırır. Bu, developer'ların işini kolaylaştırı, hata ayıklama, bakım ve iyileştirme süreçlerini de kolaylaştırır.

## KISS - Keep It Simple, Stupid

Keep It Simple, Stupid, yani Basit Tut, Aptal prensibi, bir yazılımın tasarım ve geliştirme sürecinde basitliğe odaklanmayı önerir. KISS prensibi, karmaşık veya gereksiz özelliklerden kaçınarak, bir yazılımın basit, anlaşılır ve sürdürülebilir olmasını sağlamayı hedefler.

Fazla karmaşıklık, yazılımın anlaşılmasını zorlaştırabilir, hatalara yol açabilir ve bakım maliyetlerini artırabilir. Bu nedenle, KISS prensibi, genel gereksinimleri ve tasarımı mümkün olduğunca basit tutmayı teşvik eder. KISS tasarım prensibinin temel özellikleri;

- Basitlik: KISS prensibi, yazılımın olabildiğince basit ve anlaşılır olması gerektiğini savunur. Karmaşık ve gereksiz detaylardan kaçınarak kodun okunabilirliğini artırır. Basitlik, hem kodun başkaları tarafından daha kolay anlaşılmasını sağlar hem de bakım ve geliştirme süreçlerini kolaylaştırır.

- İşlevsellik: KISS prensibi, kodun sadece gerekli işlevleri yerine getirmesini amaçlar. Gereksiz veya kullanılmayan özelliklerin eklenmesinden kaçınılmalıdır. Bu, gereksiz karmaşıklığı önler ve hatalı kod yapısı olma olasılığını azaltır.

- Okunabilirlik: KISS prensibi, kodun okunabilirliğine büyük önem verir. Basit ve anlaşılır bir kod, diğer geliştiricilerin kodu daha hızlı anlamasını ve üzerinde çalışmasını kolaylaştırır. İyi ve mantıklı adlandırılmış değişkenler, düzenli bir kod yapısı ve açıklayıcı yorumlar, kodun okunabilirliğini artıran unsurlardır.

- Minimal Bağımlılıklar: KISS prensibi, yazılımın dışa bağımlılıklarını en aza indirgemeyi hedefler. Karmaşık veya gereksiz bağımlılıklar yerine, daha basit ve doğrudan çözümler tercih edilir. Bu, projenin yönetimini kolaylaştırır ve yazılımın genel karmaşıklığını azaltır.

## YAGNI - You Ain’t Gonna Need It

You Ain’t Gonna Need It, yani Buna İhtiyacın Olmayacak prensibi gereksiz karmaşıklığı önlemek ve kaynakları boşa harcamamak için basit ve sade bir yaklaşım önerir. YAGNI prensibi, "Belki gelecekte ihtiyaç duyarız" gibi varsayımlar üzerine dayalı özellik eklemelerinden kaçınmayı teşvik eder. Kısaca bu prensibin genel olarak dikkat çektiği şey; ihtiyacımız olmayan şeylerin sisteme dahil edilmemesi gerektiğidir.

Bu prensip, yazılımın basit, anlaşılır ve bakımı kolay olmasını sağlar. Gereksiz özelliklerin eklenmemesi, geliştirme sürecini hızlandırabilir ve kaynakların etkin kullanımını sağlayabilir.

Ancak, YAGNI prensibini uygularken dikkatli olunmalıdır. Önemli işlevselliği atlamamak ve gelecekteki gereksinimleri tamamen görmezden gelmemek önemlidir. Büyük projelerde, gelecekteki ihtiyaçları tahmin etmek ve buna göre tasarım yapmak önemli olabilir.

## Özet

Özet geçmek gerekirse, DRY (Don't Repeat Yourself) prensibi, yazılım geliştirme sürecinde tekrarlamalardan kaçınmayı vurgular. Kodun tekrar eden parçalarının ortak bir yerde tutulması ve birden fazla kez yazılmaması gerektiğini vurgular. KISS (Keep It Simple, Stupid) prensibi, yazılım tasarımının ve kodun basit ve anlaşılır olması gerektiğini vurgular. Karmaşık çözümler yerine basit çözümler tercih edilmelidir. Kodun okunabilir, anlaşılabilir ve bakımı kolay olmalıdır. Bu prensibe göre, gereksiz karmaşıklıktan kaçınılmalı, sade ve anlaşılır bir tasarım benimsenmeli ve gereksiz özellikler eklenmemelidir. YAGNI (You Ain't Gonna Need It) prensibiyse sadece ihtiyaç duyulan şeylere odaklanmayı ve yazılım geliştirme sürecinde gelecekteki ihtiyaçlar üzerine varsayımlar yapmak yerine, sadece şu anda ihtiyaç duyulan özellikleri uygulamayı önerir.
