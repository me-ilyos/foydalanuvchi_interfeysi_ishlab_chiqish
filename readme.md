# Universitet veb-sahifasini yaratish darsligi

Bugun biz universitet uchun oddiy veb-sahifa yaratamiz. Keling, bosqichma-bosqich o'rganib chiqamiz.

## 1-bosqich: HTML asosiy tuzilishi

Avvalo, biz HTML hujjatimizning asosiy tuzilishini yaratishimiz kerak. HTML hujjati `<!DOCTYPE html>` bilan boshlanadi - bu brauzerga hujjat HTML5 formatida ekanligini bildiradi. Keyin `<html>` tegi keladi, u butun sahifani o'rab turadi va `lang="en"` atributi orqali sahifa tilini belgilaydi.

`<head>` qismida sahifa haqidagi meta-ma'lumotlar, sarlavha va uslublar joylashadi. `<body>` qismida esa sahifaning asosiy mazmuni bo'ladi.

Keling, kodga qaraylik:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Turan International University</title>
    <style>
        /* CSS kodlar keyinroq yoziladi */
    </style>
</head>
<body>
    <!-- Sahifa tarkibi shu yerda bo'ladi -->
</body>
</html>
```

## 2-bosqich: Universitet logotipi va sarlavhasi

Endi sahifamizning birinchi `div` elementini yaratamiz. `div` (division) - bu HTML-dagi konteyner element. U sahifani mantiqiy bo'limlarga ajratish uchun ishlatiladi. Har bir `div` o'zining alohida mazmun va uslublariga ega bo'lishi mumkin.

Birinchi `div`da universitet logotipi, asosiy sarlavha va shiori joylashadi:

```html
<div>
    <img src="" alt="Turan International University Logo">
    <h1>Turan International University</h1>
    <p>Shaping Tomorrow's Leaders Since 1992</p>
</div>
```

Bu yerda:
- `<img>` - rasm joylashtirish uchun teg. `src` atributi rasm manzilini, `alt` esa rasm yuklanmaganda ko'rsatiladigan matnni bildiradi
- `<h1>` - eng katta sarlavha tegi. Sahifada odatda bitta `h1` bo'ladi
- `<p>` - paragraf tegi, oddiy matn uchun ishlatiladi

## 3-bosqich: Navigatsiya paneli

Navigatsiya paneli - bu foydalanuvchilar sayt bo'limlari orasida harakatlanishi uchun havolalar to'plami. Biz uni tartibsiz ro'yxat (`<ul>`) ko'rinishida yaratamiz:

```html
<div>
    <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#programs">Programs</a></li>
        <li><a href="#admissions">Admissions</a></li>
        <li><a href="#research">Research</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</div>
```

Bu yerda:
- `<ul>` - tartibsiz ro'yxat (unordered list)
- `<li>` - ro'yxat elementi (list item)
- `<a>` - havola tegi. `href` atributi havola manzilini ko'rsatadi. `#` belgisi sahifaning ichki bo'limlariga havolani bildiradi

## 4-bosqich: Asosiy ma'lumot bo'limi

Keyingi `div`da universitetning qisqacha tavsifi va kampus rasmi joylashadi:

```html
<div>
    <h2>Welcome to Turan International University</h2>
    <img src="" alt="Turan University Campus">
    <p>Join us at Turan International University, where tradition meets innovation. Our commitment to academic excellence, cultural diversity, and groundbreaking research has established us as a leading institution in Central Asia.</p>
</div>
```

Bu yerda:
- `<h2>` - ikkinchi darajali sarlavha
- Kampus rasmi
- Universitet haqida tavsif

## 5-bosqich: O'quv dasturlari

Bu bo'limda biz ichma-ich ro'yxatlardan foydalanamiz. Bu fakultetlar va ularning yo'nalishlarini ko'rsatish uchun juda qulay:

```html
<div>
    <h3>Our Programs</h3>
    <ul>
        <li>Engineering and Technology
            <ul>
                <li>Information Systems</li>
                <li>Computer Engineering</li>
                <li>Robotics</li>
            </ul>
        </li>
        <li>Business School
            <ul>
                <li>Finance and Banking</li>
                <li>International Business</li>
                <li>Digital Marketing</li>
            </ul>
        </li>
        <li>Law and International Relations</li>
        <li>Social Sciences and Humanities</li>
    </ul>
</div>
```

Ichma-ich ro'yxatlar bir ro'yxat ichida boshqa ro'yxat yaratish imkonini beradi. Bu ierarhik ma'lumotlarni ko'rsatish uchun juda foydali.

## 6-bosqich: Qabul jarayoni

Qabul jarayonini ko'rsatish uchun tartibli ro'yxat (`<ol>`) ishlatamiz, chunki bu yerda qadamlar ketma-ketligi muhim:

```html
<div>
    <h3>Admission Process</h3>
    <ol>
        <li>Fill out the online application form</li>
        <li>Submit high school transcripts</li>
        <li>Provide language proficiency certificate</li>
        <li>Pass entrance examinations</li>
        <li>Complete the interview process</li>
    </ol>
</div>
```

`<ol>` (ordered list) avtomatik ravishda elementlarni raqamlaydi.

## 7-bosqich: Tadbirlar jadvali

Jadval ma'lumotlarni ustun va qatorlarda ko'rsatish uchun ishlatiladi:

```html
<div>
    <h3>Upcoming Events</h3>
    <table>
        <tr>
            <th>Date</th>
            <th>Event</th>
            <th>Location</th>
        </tr>
        <tr>
            <td>February 15</td>
            <td>International Students Day</td>
            <td>Main Hall</td>
        </tr>
        <tr>
            <td>March 5</td>
            <td>Spring Career Fair</td>
            <td>Student Center</td>
        </tr>
        <tr>
            <td>March 20</td>
            <td>Research Symposium</td>
            <td>Conference Center</td>
        </tr>
    </table>
</div>
```

Bu yerda:
- `<table>` - jadval konteyneri
- `<tr>` - jadval qatori (table row)
- `<th>` - jadval sarlavha katakchasi (table header)
- `<td>` - oddiy katakcha (table data)

## 8-bosqich: Kampus hayoti

Bu bo'limda kampus hayotini aks ettiruvchi rasmlar joylashgan:

```html
<div>
    <h3>Campus Life</h3>
    <img src="" alt="Modern Library">
    <img src="" alt="Innovation Center">
    <img src="" alt="Student Life Center">
</div>
```

## 9-bosqich: Aloqa ma'lumotlari

Aloqa ma'lumotlari bo'limida havolalar va manzil ma'lumotlari bor:

```html
<div>
    <h3>Contact Us</h3>
    <p>For more information, please visit our <a href="#contact">contact page</a> or email us at <a href="mailto:info@turan.edu">info@turan.edu</a></p>
    <p>
        45 Namangan Avenue<br>
        Namangan, Uzbekistan<br>
        Phone: +998 (91) 123-4567
    </p>
</div>
```

Bu yerda:
- `mailto:` havola elektron pochta manzilini ochadi
- `<br>` - qator tashlash tegi

## 10-bosqich: Mualliflik huquqi

Sahifaning oxirgi qismida mualliflik huquqi haqida ma'lumot:

```html
<div>
    <p>© 2025 Turan International University. All rights reserved.</p>
</div>
```

## 11-bosqich: CSS uslublari

Endi sahifamizni chiroyli ko'rinishga keltiramiz. CSS (Cascading Style Sheets) veb-sahifaning ko'rinishini boshqaradi. Keling, har bir elementning uslublarini bosqichma-bosqich o'rganamiz.

### Body uslublari

Avvalo, butun sahifaning asosiy ko'rinishini belgilaymiz:

```css
body {
    font-family: Arial, sans-serif;
    width: 80%;
    margin: 0 auto;
    padding: 20px;
    background-color: #f5f5f5;
}
```

Bu CSS kodda:
- `font-family` butun sahifa uchun shrift turini belgilaydi. Agar Arial topilmasa, tizimning istalgan sans-serif shrifti ishlatiladi
- `width: 80%` sahifani ekran kengligining 80 foiziga sozlaydi
- `margin: 0 auto` sahifani markazga joylashtiradi. Bu yerda "0" tepadan va pastdan, "auto" esa chapdan va o'ngdan masofa avtomatik hisoblanishini bildiradi
- `padding: 20px` sahifa chetlaridan 20 piksel ichkari surilishini ta'minlaydi
- `background-color: #f5f5f5` sahifa fonini och kulrang qiladi

### Sarlavha uslublari

Sarlavhalarni ajratib ko'rsatish uchun maxsus uslublar beramiz:

```css
h1 {
    color: darkblue;
    text-align: center;
}

h2, h3 {
    color: darkblue;
}
```

Bu yerda biz:
- `h1` sarlavhani markazga tekislaymiz va to'q ko'k rangga bo'yaymiz
- `h2` va `h3` sarlavhalarni ham xuddi shunday rangga bo'yaymiz, lekin chapga tekislangan holda qoldiramiz

### Rasm uslublari

Rasmlarni responsiv (moslashuvchan) qilish uchun:

```css
img {
    max-width: 100%;
    height: auto;
}
```

Bu uslublar:
- `max-width: 100%` rasmning maksimal kengligini ota-elementining kengligiga bog'laydi
- `height: auto` rasm balandligini proporsional ravishda o'zgartiradi

### Navigatsiya ro'yxati uslublari

Navigatsiya panelidagi ro'yxatni chiroyli ko'rinishga keltiramiz:

```css
ul {
    list-style-type: none;
    padding: 0;
    margin: 20px 0;
}

ul li {
    margin: 10px 0;
}

ul ul {
    margin-left: 20px;
    list-style-type: disc;
}
```

Bu uslublar:
- Asosiy ro'yxatdan nuqtalarni olib tashlaydi (`list-style-type: none`)
- Ichki ro'yxatlarda nuqtalarni qoldiradi (`list-style-type: disc`)
- Har bir element orasida masofa qo'shadi
- Ichki ro'yxatlarni chapdan surib qo'yadi

### Havola uslublari

Havolalarni interaktiv qilish uchun:

```css
a {
    color: blue;
    text-decoration: none;
    padding: 5px;
}

a:hover {
    color: darkblue;
    background-color: #e0e0e0;
}
```

Bu yerda:
- Havolalar ko'k rangda bo'ladi
- Tagiga chiziq bo'lmaydi (`text-decoration: none`)
- Sichqoncha ustiga borganda (`hover`) rang to'qlashadi va fon rangi o'zgaradi

### Jadval uslublari

Jadvalimizni professional ko'rinishga keltiramiz:

```css
table {
    width: 100%;
    border-collapse: collapse;
    margin: 20px 0;
}

th, td {
    border: 1px solid black;
    padding: 10px;
    text-align: left;
}

th {
    background-color: darkblue;
    color: white;
}

tr:hover {
    background-color: #e0e0e0;
}
```

Bu uslublar:
- Jadvalni to'liq kenglikka cho'zadi
- Katakchalar orasidagi chegaralarni birlashtiradi
- Sarlavha qatorini ajratib ko'rsatadi
- Sichqoncha ustidagi qator rangini o'zgartiradi

### Konteyner (div) uslublari

Har bir bo'limni alohida ajratib ko'rsatish uchun:

```css
div {
    margin: 20px 0;
    padding: 10px;
    background-color: white;
}
```