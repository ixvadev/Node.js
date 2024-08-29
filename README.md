

# Node.js

Node.js — bu JavaScript dasturlash tilida yozilgan server tomonida ishlaydigan muhit. Node.js asosan server tomonida ishlash uchun mo'ljallangan bo'lib, tez va samarali dasturlar yaratishga imkon beradi. Bu muhit asosan Google V8 JavaScript dvigateliga asoslangan.

## Asosiy xususiyatlari

- **Bitta ipli, asinxron va hodisa asoslangan (event-driven)**: Node.js asinxron kiritish/chiqarish (I/O) jarayonini samarali amalga oshirish uchun yaratilgan. Bu degani, bir vaqtning o'zida bir nechta I/O operatsiyalarini bloklanmasdan bajarish mumkin.

- **Tezlik**: Node.js V8 JavaScript dvigatelidan foydalanadi, bu esa uning tez va samarali ishlashini ta'minlaydi. Bu serverlar va mikroservislar uchun juda mos.

- **Node Package Manager (NPM)**: Node.js uchun paket menejeri bo'lib, u orqali minglab bepul kutubxonalar va modullarni osongina o'rnatish va ulardan foydalanish mumkin.

- **Platformadan mustaqil**: Node.js turli operatsion tizimlar, jumladan Windows, macOS va Linuxda ishlaydi.

## Foydalanish holatlari

- **Web-serverlar**: Node.js asosan real-vaqtli veb-ilovalar, API-lar va boshqa server tomonidagi dasturlarni yaratish uchun ishlatiladi.

- **Mikroservislar**: Node.js mikroservislar arxitekturasini yaratish uchun ideal, chunki u yengil va modullarga bo'linuvchi.

- **Reaktiv dasturlar**: Masalan, chat ilovalari, onlayn o'yinlar yoki boshqa ko'p foydalanuvchilarni qo'llab-quvvatlovchi real-vaqt dasturlarini yaratishda Node.js keng qo'llaniladi.

## Oddiy Misol

Quyida Node.js-da yozilgan oddiy "Hello, World!" veb-server misoli keltirilgan:

```javascript
const http = require('http');

// Server yaratish
const server = http.createServer((req, res) => {
    res.statusCode = 200;
    res.setHeader('Content-Type', 'text/plain');
    res.end('Hello, World!\n');
});

// Serverni 3000-portda ishlatish
server.listen(3000, '127.0.0.1', () => {
    console.log('Server http://127.0.0.1:3000 manzilida ishlamoqda');
});
