# Qulay-Kuryer-
Kichik biznes uchun
<!DOCTYPE html>
<html lang="uz">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Qulay Kuryer</title>

<style>
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
}

body {
    background: #f2f8f2;
    color: #243328;
}

header {
    background: #13863d;
    color: white;
    padding: 16px;
    text-align: center;
}

header h1 {
    margin-bottom: 14px;
}

nav {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 8px;
}

nav button {
    border: none;
    padding: 11px 14px;
    border-radius: 8px;
    cursor: pointer;
    background: white;
    color: #13863d;
    font-weight: bold;
}

nav button:hover {
    background: #d8f5df;
}

.page {
    display: none;
    padding: 24px 16px;
    max-width: 1150px;
    margin: auto;
}

.page.active {
    display: block;
}

.hero {
    background: linear-gradient(#0006, #0007),
    url("https://images.unsplash.com/photo-1526367790999-0150786686a2?auto=format&fit=crop&w=1400&q=80");
    background-size: cover;
    background-position: center;
    min-height: 340px;
    border-radius: 16px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: white;
    padding: 25px;
}

.hero h2 {
    font-size: 34px;
    margin-bottom: 15px;
}

.hero p {
    font-size: 18px;
    margin-bottom: 20px;
}

.btn {
    border: none;
    border-radius: 8px;
    background: #13863d;
    color: white;
    padding: 12px 18px;
    cursor: pointer;
    font-size: 15px;
    font-weight: bold;
    margin: 10px 0 0 15px;
}

.btn:hover {
    background: #09652b;
}

.cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
    gap: 18px;
    margin-top: 20px;
}

.card {
    background: white;
    border-radius: 13px;
    overflow: hidden;
    box-shadow: 0 4px 14px #00000012;
    padding: 18px;
}

.card h3 {
    padding: 8px 0;
    color: #13863d;
}

.card p {
    padding: 5px 0;
    line-height: 1.6;
}

.section-title {
    color: #13863d;
    margin-bottom: 15px;
}

.form-box {
    max-width: 700px;
    margin: 18px auto;
    background: white;
    padding: 22px;
    border-radius: 14px;
    box-shadow: 0 4px 15px #00000010;
}

label {
    display: block;
    font-weight: bold;
    margin-top: 14px;
    margin-bottom: 6px;
}

input, select, textarea {
    width: 100%;
    padding: 12px;
    border: 1px solid #cbd8ce;
    border-radius: 8px;
    font-size: 16px;
    background: white;
}

textarea {
    min-height: 110px;
    resize: vertical;
}

.form-box .btn {
    width: 100%;
    margin: 20px 0 0;
}

.notice, .result {
    background: #e0f6e5;
    padding: 16px;
    border-radius: 10px;
    margin: 15px 0;
    line-height: 1.7;
    overflow-wrap: anywhere;
}

footer {
    margin-top: 35px;
    padding: 22px;
    text-align: center;
    background: #126b32;
    color: white;
}

@media(max-width: 600px) {
    .hero h2 {
        font-size: 26px;
    }

    nav button {
        flex: 1 1 42%;
    }

    .page {
        padding: 17px 12px;
    }
}
</style>
</head>

<body>

<header>
    <h1>🟢 Qulay Kuryer</h1>
    <p>Yuk tashish va yetkazib berish xizmatlari</p>
    <br>

    <nav>
        <button onclick="openPage('home')">🏠 Bosh sahifa</button>
        <button onclick="openPage('transport')">🚚 Transport</button>
        <button onclick="openPage('order')">📦 Buyurtma berish</button>
        <button onclick="openPage('courier')">🏍️ Kuryer</button>
        <button onclick="openPage('logistics')">🚛 Logistika</button>
        <button onclick="openPage('taxi')">🚕 Taksi xizmatlari</button>
        <button onclick="openPage('tracking')">🔎 Kuzatuv</button>
    </nav>
</header>

<!-- BOSH SAHIFA -->
<section id="home" class="page active">
    <div class="hero">
        <h2>Qulay Kuryer xizmatiga xush kelibsiz!</h2>
        <p>Yukingizni ishonchli va qulay tarzda manzilga yetkazamiz.</p>
        <button class="btn" onclick="openPage('order')">
            📦 Buyurtma berish
        </button>
    </div>

    <h2 class="section-title" style="margin-top:28px;">
        Bizning xizmatlarimiz
    </h2>

    <div class="cards">
        <div class="card">
            <h3>🚚 Yuk tashish</h3>
            <p>Yuklaringiz uchun mos transport tanlang.</p>
            <button class="btn" onclick="openPage('transport')">Transport tanlash</button>
        </div>

        <div class="card">
            <h3>🚕 Taksi xizmati</h3>
            <p>O‘zingizga mos avtomobil va xizmat turini tanlang.</p>
            <button class="btn" onclick="openPage('taxi')">Taksi tanlash</button>
        </div>

        <div class="card">
            <h3>📦 Buyurtma berish</h3>
            <p>Manzillar va qo‘shimcha izohingizni kiriting.</p>
            <button class="btn" onclick="openPage('order')">Buyurtma berish</button>
        </div>
    </div>
</section>

<!-- TRANSPORT -->
<section id="transport" class="page">
    <h2 class="section-title">🚚 Transport turlari</h2>
    <p>Kerakli transportni tanlab, buyurtma formasini to‘ldiring.</p>

    <div class="cards">
        <div class="card">
            <h3>🚗 Sedan</h3>
            <p>Yengil yuklar va yo‘lovchilar uchun.</p>
            <button class="btn" onclick="chooseTransport('Sedan')">Tanlash</button>
        </div>

        <div class="card">
            <h3>🛻 Labo</h3>
            <p>Kichik va o‘rta hajmdagi yuklar uchun.</p>
            <button class="btn" onclick="chooseTransport('Labo')">Tanlash</button>
        </div>

        <div class="card">
            <h3>🚐 Damas</h3>
            <p>Mayda yuklar va buyumlarni tashish uchun.</p>
            <button class="btn" onclick="chooseTransport('Damas')">Tanlash</button>
        </div>

        <div class="card">
            <h3>🚛 Yuk mashinasi</h3>
            <p>Katta hajmdagi yuklarni tashish uchun.</p>
            <button class="btn" onclick="chooseTransport('Yuk mashinasi')">Tanlash</button>
        </div>

        <div class="card">
            <h3>🏍️ Motokuryer</h3>
            <p>Hujjatlar va kichik buyumlarni yetkazish uchun.</p>
            <button class="btn" onclick="chooseTransport('Motokuryer')">Tanlash</button>
        </div>

        <div class="card">
            <h3>🚐 Miniven</h3>
            <p>Bir nechta yo‘lovchi yoki ko‘proq buyumlar uchun.</p>
            <button class="btn" onclick="chooseTransport('Miniven')">Tanlash</button>
        </div>
    </div>
</section>

<!-- BUYURTMA BERISH -->
<section id="order" class="page">
    <h2 class="section-title">📦 Buyurtma berish</h2>

    <div class="notice">
        Ma’lumotlaringizni kiriting. Buyurtma berganingizdan so‘ng sizga
        buyurtma raqami beriladi. Qo‘shimcha izoh yozishingiz mumkin.
    </div>

    <form class="form-box" id="orderForm">
        <label for="customerName">👤 Ismingiz</label>
        <input id="customerName" type="text"
               placeholder="Ismingizni kiriting" required>

        <label for="customerPhone">📞 Telefon raqamingiz</label>
        <input id="customerPhone" type="tel"
               placeholder="+998 90 123 45 67"
               pattern="[+0-9 ()-]{9,20}" required>

        <label for="pickup">📍 Yuk olinadigan manzil</label>
        <input id="pickup" type="text"
               placeholder="Masalan: Chilonzor, 5-mavze" required>

        <label for="delivery">🏁 Yetkazib beriladigan manzil</label>
        <input id="delivery" type="text"
               placeholder="Masalan: Yunusobod, 10-mavze" required>

        <label for="transportType">🚚 Transport yoki xizmat turi</label>
        <select id="transportType" required>
            <option value="">Transportni tanlang</option>
            <option>Sedan</option>
            <option>Labo</option>
            <option>Damas</option>
            <option>Yuk mashinasi</option>
            <option>Motokuryer</option>
            <option>Miniven</option>
            <option>Komfort taksi</option>
            <option>Biznes klass</option>
            <option>Krossover</option>
            <option>Oilaviy taksi</option>
            <option>Aeroport taksisi</option>
            <option>Shaharlararo taksi</option>
            <option>Buyum yetkazish</option>
            <option>Soatbay avtomobil</option>
            <option>SAS maxsus buyurtmasi</option>
        </select>

        <label for="cargo">📦 Yuk yoki buyurtma turi</label>
        <input id="cargo" type="text"
               placeholder="Masalan: oziq-ovqat, mebel, hujjat" required>

        <label for="distance">📏 Taxminiy masofa (km)</label>
        <input id="distance" type="number" min="1" max="1000"
               value="5" required>

        <label for="orderComment">📝 Buyurtma haqida qo‘shimcha izoh</label>
        <textarea id="orderComment" maxlength="1000"
            placeholder="Haydovchi uchun qo‘shimcha ko‘rsatma yoki boshqa izohingizni yozing..."></textarea>

        <button class="btn" type="submit">✅ Buyurtma berish</button>
        <div id="orderResult" aria-live="polite"></div>
    </form>
</section>

<!-- KURYER -->
<section id="courier" class="page">
    <h2 class="section-title">🏍️ Kuryer xizmati</h2>

    <div class="cards">
        <div class="card">
            <h3>⚡ Tezkor kuryer</h3>
            <p>Hujjatlar, oziq-ovqat va kichik buyumlarni yetkazish xizmati.</p>
            <button class="btn" onclick="chooseTransport('Motokuryer')">Buyurtma berish</button>
        </div>

        <div class="card">
            <h3>📦 Oddiy yetkazib berish</h3>
            <p>Buyurtmangiz uchun manzil va ko‘rsatmalarni kiriting.</p>
            <button class="btn" onclick="chooseTransport('Buyum yetkazish')">Buyurtma berish</button>
        </div>
    </div>

    <div class="notice">
        Eslatma: bu demo sayt haqiqiy kuryerning GPS lokatsiyasiga ulanmagan.
    </div>
</section>

<!-- LOGISTIKA -->
<section id="logistics" class="page">
    <h2 class="section-title">🚛 Logistika va SAS xizmati</h2>

    <div class="cards">
        <div class="card">
            <h3>📦 Yuk tashish</h3>
            <p>Yukni qabul qilish va kerakli manzilga yetkazish.</p>
            <button class="btn" onclick="chooseTransport('Labo')">Buyurtma berish</button>
        </div>

        <div class="card">
            <h3>🚚 SAS — maxsus buyurtma</h3>
            <p>Maxsus talab va ko‘rsatmalaringizni izoh maydoniga yozing.</p>
            <button class="btn" onclick="chooseTransport('Yuk mashinasi', 'SAS maxsus buyurtmasi')">SAS buyurtmasi</button>
        </div>

        <div class="card">
            <h3>📍 Hududiy yetkazib berish</h3>
            <p>Yuk olinadigan va yetkaziladigan manzillarni belgilang.</p>
            <button class="btn" onclick="openPage('order')">Manzillarni kiritish</button>
        </div>
    </div>
</section>

<!-- TAKSI XIZMATLARI -->
<section id="taxi" class="page">
    <h2 class="section-title">🚕 Taksi xizmatlari</h2>
    <p>O‘zingizga mos xizmatni tanlang va buyurtma bering.</p>

    <div class="cards">
        <div class="card">
            <h3>🚗 Sedan taksi</h3>
            <p>Shahar ichida kundalik safarlar uchun.</p>
            <button class="btn" onclick="chooseTransport('Sedan', 'Taksi xizmati')">Tanlash</button>
        </div>

        <div class="card">
            <h3>🚕 Komfort taksi</h3>
            <p>Qulay avtomobilda safar qilish uchun.</p>
            <button class="btn" onclick="chooseTransport('Komfort taksi', 'Taksi xizmati')">Tanlash</button>
        </div>

        <div class="card">
            <h3>🚘 Biznes klass</h3>
            <p>Ish uchrashuvlari va maxsus safarlar uchun.</p>
            <button class="btn" onclick="chooseTransport('Biznes klass', 'Taksi xizmati')">Tanlash</button>
        </div>

        <div class="card">
            <h3>🚙 Krossover</h3>
            <p>Shahar va uzoq yo‘llarda safar qilish uchun.</p>
            <button class="btn" onclick="chooseTransport('Krossover', 'Taksi xizmati')">Tanlash</button>
        </div>

        <div class="card">
            <h3>🚐 Miniven</h3>
            <p>Bir nechta yo‘lovchi uchun keng avtomobil.</p>
            <button class="btn" onclick="chooseTransport('Miniven', 'Taksi xizmati')">Tanlash</button>
        </div>

        <div class="card">
            <h3>👨‍👩‍👧‍👦 Oilaviy taksi</h3>
            <p>Oila bilan safar qilish uchun.</p>
            <button class="btn" onclick="chooseTransport('Oilaviy taksi', 'Taksi xizmati')">Tanlash</button>
        </div>

        <div class="card">
            <h3>✈️ Aeroport taksisi</h3>
            <p>Aeroportga borish yoki aeroportdan olib ketish.</p>
            <button class="btn" onclick="chooseTransport('Aeroport taksisi', 'Taksi xizmati')">Tanlash</button>
        </div>

        <div class="card">
            <h3>🛣️ Shaharlararo taksi</h3>
            <p>Boshqa shahar yoki tumanlarga safar.</p>
            <button class="btn" onclick="chooseTransport('Shaharlararo taksi', 'Taksi xizmati')">Tanlash</button>
        </div>

        <div class="card">
            <h3>🛻 Labo yuk xizmati</h3>
            <p>Kichik va o‘rta hajmdagi yuklarni tashish.</p>
            <button class="btn" onclick="chooseTransport('Labo', 'Yuk tashish')">Tanlash</button>
        </div>

        <div class="card">
            <h3>🚐 Damas yuk xizmati</h3>
            <p>Mayda yuklar va buyumlarni tashish.</p>
            <button class="btn" onclick="chooseTransport('Damas', 'Yuk tashish')">Tanlash</button>
        </div>

        <div class="card">
            <h3>📦 Buyum yetkazish</h3>
            <p>Hujjatlar va kichik buyumlarni yetkazib berish.</p>
            <button class="btn" onclick="chooseTransport('Motokuryer', 'Buyum yetkazish')">Tanlash</button>
        </div>

        <div class="card">
            <h3>⏰ Soatbay avtomobil</h3>
            <p>Avtomobildan bir necha soat davomida foydalanish.</p>
            <button class="btn" onclick="chooseTransport('Soatbay avtomobil', 'Taksi xizmati')">Tanlash</button>
        </div>
    </div>
</section>

<!-- BUYURTMANI KUZATISH -->
<section id="tracking" class="page">
    <h2 class="section-title">🔎 Buyurtmani kuzatish</h2>

    <div class="form-box">
        <label for="trackingId">Buyurtma raqami</label>
        <input id="trackingId" type="text" placeholder="Masalan: QK12345678">
        <button class="btn" onclick="trackOrder()">Buyurtmani tekshirish</button>
        <div id="trackingResult" aria-live="polite"></div>
    </div>
</section>

<footer>
    <p>© 2026 Qulay Kuryer</p>
    <p>Qulay, tezkor va ishonchli xizmat.</p>
</footer>

<script>
function openPage(pageId) {
    document.querySelectorAll('.page').forEach(function(page) {
        page.classList.remove('active');
    });

    const target = document.getElementById(pageId);

    if (target) {
        target.classList.add('active');
        window.scrollTo({ top: 0, behavior: 'smooth' });
    }
}

function chooseTransport(type, cargoType) {
    openPage('order');

    document.getElementById('transportType').value = type;

    if (cargoType) {
        document.getElementById('cargo').value = cargoType;
    }

    document.getElementById('customerName').focus();
}

function getOrders() {
    try {
        return JSON.parse(localStorage.getItem('qulayKuryerOrders') || '[]');
    } catch (error) {
        return [];
    }
}

function saveOrders(orders) {
    localStorage.setItem('qulayKuryerOrders', JSON.stringify(orders));
}

function escapeHTML(value) {
    return String(value).replace(/[&<>"']/g, function(char) {
        return {
            '&': '&amp;',
            '<': '&lt;',
            '>': '&gt;',
            '"': '&quot;',
            "'": '&#39;'
        }[char];
    });
}

document.getElementById('orderForm').addEventListener('submit', function(event) {
    event.preventDefault();

    const name = document.getElementById('customerName').value.trim();
    const phone = document.getElementById('customerPhone').value.trim();
    const pickup = document.getElementById('pickup').value.trim();
    const delivery = document.getElementById('delivery').value.trim();
    const transport = document.getElementById('transportType').value;
    const cargo = document.getElementById('cargo').value.trim();
    const distance = Number(document.getElementById('distance').value);
    const comment = document.getElementById('orderComment').value.trim();

    if (!name || !phone || !pickup || !delivery || !transport || !cargo) {
        alert('Iltimos, barcha majburiy maydonlarni to‘ldiring.');
        return;
    }

    if (!Number.isFinite(distance) || distance < 1 || distance > 1000) {
        alert('Masofani 1 dan 1000 km gacha kiriting.');
        return;
    }

    const orderId = 'QK' + Date.now().toString().slice(-8);

    const order = {
        id: orderId,
        name: name,
        phone: phone,
        pickup: pickup,
        delivery: delivery,
        transport: transport,
        cargo: cargo,
        distance: distance,
        comment: comment,
        status: 'Buyurtma qabul qilindi',
        createdAt: new Date().toLocaleString('uz-UZ')
    };

    const orders = getOrders();
    orders.unshift(order);

    try {
        saveOrders(orders);
    } catch (error) {
        alert('Buyurtmani saqlab bo‘lmadi. Brauzer xotirasini tekshiring.');
        return;
    }

    document.getElementById('orderResult').innerHTML =
        '<div class="result">' +
        '<h3>✅ Buyurtmangiz saqlandi!</h3>' +
        '<p><b>Buyurtma raqami:</b> ' + escapeHTML(order.id) + '</p>' +
        '<p><b>Ism:</b> ' + escapeHTML(order.name) + '</p>' +
        '<p><b>Telefon:</b> ' + escapeHTML(order.phone) + '</p>' +
        '<p><b>Transport:</b> ' + escapeHTML(order.transport) + '</p>' +
        '<p><b>Yuk:</b> ' + escapeHTML(order.cargo) + '</p>' +
        '<p><b>Olinadigan manzil:</b> ' + escapeHTML(order.pickup) + '</p>' +
        '<p><b>Yetkazish manzili:</b> ' + escapeHTML(order.delivery) + '</p>' +
        '<p><b>Masofa:</b> ' + escapeHTML(order.distance) + ' km</p>' +
        '<p><b>Qo‘shimcha izoh:</b> ' +
        (order.comment ? escapeHTML(order.comment) : 'Izoh yozilmagan') + '</p>' +
        '<p><b>Holati:</b> ' + escapeHTML(order.status) + '</p>' +
        '<p>Buyurtmani kuzatish uchun raqamingizni saqlab qo‘ying.</p>' +
        '</div>';

    document.getElementById('trackingId').value = orderId;

    this.reset();
    document.getElementById('distance').value = 5;
});

function trackOrder() {
    const id = document.getElementById('trackingId').value.trim();
    const result = document.getElementById('trackingResult');

    if (!id) {
        result.innerHTML = '<div class="result">Buyurtma raqamini kiriting.</div>';
        return;
    }

    const order = getOrders().find(function(item) {
        return item.id.toLowerCase() === id.toLowerCase();
    });

    if (!order) {
        result.innerHTML =
            '<div class="result">Bu raqam bo‘yicha buyurtma topilmadi. ' +
            'Raqamni tekshiring yoki buyurtma bergan brauzerdan foydalaning.</div>';
        return;
    }

    result.innerHTML =
        '<div class="result">' +
        '<h3>📦 Buyurtma ma’lumotlari</h3>' +
        '<p><b>Raqami:</b> ' + escapeHTML(order.id) + '</p>' +
        '<p><b>Mijoz:</b> ' + escapeHTML(order.name) + '</p>' +
        '<p><b>Transport:</b> ' + escapeHTML(order.transport) + '</p>' +
        '<p><b>Yuk:</b> ' + escapeHTML(order.cargo) + '</p>' +
        '<p><b>Olinadigan manzil:</b> ' + escapeHTML(order.pickup) + '</p>' +
        '<p><b>Yetkazish manzili:</b> ' + escapeHTML(order.delivery) + '</p>' +
        '<p><b>Izoh:</b> ' +
        (order.comment ? escapeHTML(order.comment) : 'Izoh yozilmagan') + '</p>' +
        '<p><b>Holati:</b> ' + escapeHTML(order.status) + '</p>' +
        '<p><b>Buyurtma vaqti:</b> ' + escapeHTML(order.createdAt) + '</p>' +
        '</div>';
}
</script>

</body>
</html>
