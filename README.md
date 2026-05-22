Kod haqida qisqacha tavsif (O'zbek tilida)
🫁 X-Ray tasvir klassifikatori
Bu kod rentgen (X-ray) tasvirlarini tahlil qiluvchi sun'iy intellekt modeli bo'lib, tasvirlarni ikki sinfga ajratadi:

✅ Normal — sog'lom
❌ Pathology — patologiya (kasallik belgilari)



Asosiy qismlar
1. Model arxitekturasi
DenseNet121 — oldindan o'rgatilgan neyron tarmoq ishlatiladi. Faqat oxirgi klassifikator qatlami qayta o'rgatiladi, bu esa vaqt va resurslarni tejaydi.
2. Ma'lumotlarni tayyorlash
O'qitish jarayonida tasvirlar sun'iy ravishda ko'paytiriladi: burish, aks ettirish, yorqinlik o'zgartirish — bu modelni yanada mustahkam qiladi.
3. Sinf og'irliklari
Agar bir sinfda kam, ikkinchisida ko'p tasvir bo'lsa, model avtomatik ravishda muvozanatni saqlaydi.
4. O'qitish rejimi (train)
Model ./dataset/train va ./dataset/test papkalaridan o'rganadi, har bir davrda natija ko'rsatiladi va eng yaxshi model saqlanadi.
5. Test rejimi (test)
./images papkasidagi tasvirlarni tahlil qilib, har bir tasvir uchun sinf nomi va ishonch foizi chiqaradi, so'ng grafikda ko'rsatadi.




Tibbiy rentgen tasvirlarini avtomatik tahlil qiluvchi, GPU/CPU da ishlaydigan, o'zbek tibbiyotiga ham qo'llanishi mumkin bo'lgan deep learning loyihasi.
