<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Мосты — экскурсии в Петербурге | Живые истории</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600&family=Playfair+Display:wght@400;500;600;700;800&family=Cormorant+Garamond:ital,wght@0,400;0,500;0,600;1,400;1,500&display=swap" rel="stylesheet">
                                     
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', 'Cormorant Garamond', 'Georgia', 'Times New Roman', serif;
            font-weight: 400;
            line-height: 1.55;
            color: #1e2f3d;
            background: #f5f2eb;
        }

        h1, h2, h3, .logo span, .hero h1, .section-block h2, .advantages-sidebar h3, .tour-card h3, .cta-button, .btn-book, .btn-submit {
            font-family: 'Playfair Display', 'Georgia', 'Times New Roman', serif;
            letter-spacing: 0.01em;
        }

        .site-header {
            background: #1f2c38;
            color: white;
            padding: 15px 30px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            border-bottom: 3px solid #b89a6b;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 10px;
            text-decoration: none;
            color: white;
            font-size: 1.5em;
            font-weight: 700;
        }

        .logo span {
            letter-spacing: 1px;
            text-shadow: 1px 1px 0 #2c3e4e;
        }

        .logo img {
            border-radius: 50%;
            border: 2px solid #b89a6b;
        }

        .main-nav ul {
            list-style: none;
            display: flex;
            gap: 20px;
            flex-wrap: wrap;
        }

        .main-nav a {
            color: #e9eef2;
            text-decoration: none;
            padding: 6px 14px;
            border-radius: 40px;
            font-family: 'Inter', sans-serif;
            font-weight: 500;
            transition: 0.2s;
        }

        .main-nav a:hover {
            background: #b89a6b;
            color: #1f2c38;
        }

        .hero {
            background: linear-gradient(97deg, #1f2c38 0%, #2e404f 100%);
            color: white;
            text-align: center;
            padding: 70px 25px;
            border-bottom: 1px solid #b89a6b;
        }

        .hero h1 {
            font-size: 3em;
            margin-bottom: 18px;
            font-weight: 700;
            letter-spacing: -0.5px;
        }

        .hero p {
            max-width: 750px;
            margin: 0 auto 25px;
            font-family: 'Cormorant Garamond', serif;
            font-size: 1.3rem;
            font-weight: 500;
            color: #e6eef5;
            line-height: 1.5;
        }

        .cta-button {
            display: inline-block;
            background: #b89a6b;
            color: #1f2c38;
            padding: 12px 34px;
            text-decoration: none;
            font-weight: 700;
            font-size: 1.1rem;
            border-radius: 50px;
            transition: 0.25s;
            box-shadow: 0 2px 6px rgba(0,0,0,0.2);
        }

        .cta-button:hover {
            background: #dbb87a;
            transform: scale(1.02);
            color: #111;
        }

        .section-block {
            background: #ffffffec;
            margin: 24px 32px;
            padding: 32px 36px;
            border-radius: 20px;
            border-left: 6px solid #b89a6b;
            box-shadow: 0 6px 18px rgba(0, 0, 0, 0.03);
        }

        .section-block h2 {
            font-size: 2.2rem;
            color: #1f2c38;
            margin-bottom: 24px;
            border-bottom: 2px solid #dccca8;
            padding-bottom: 8px;
            display: inline-block;
            letter-spacing: -0.3px;
        }

        .tours-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
        }

        .tour-card {
            background: #fffdf9;
            border-radius: 18px;
            padding: 18px;
            border: 1px solid #e7ded1;
            transition: 0.25s;
        }
        .tour-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 14px 28px rgba(0,0,0,0.08);
            border-color: #b89a6b;
        }

        .tour-card img {
            width: 100%;
            height: 190px;
            object-fit: cover;
            border-radius: 12px;
            margin-bottom: 14px;
        }

        .tour-card h3 {
            font-size: 1.45rem;
            font-weight: 700;
            margin-bottom: 10px;
        }

        .tour-card p {
            font-family: 'Inter', sans-serif;
            font-size: 0.95rem;
            color: #2c3e4e;
        }

        .tour-card ul {
            list-style: none;
            margin: 12px 0;
        }

        .tour-card ul li::before {
            content: "• ";
            color: #b89a6b;
            font-weight: bold;
        }
        .btn-book {
            background: #2c3e50;
            color: white;
            border: none;
            padding: 8px 24px;
            border-radius: 40px;
            cursor: pointer;
            font-weight: 600;
            font-size: 0.9rem;
            transition: 0.2s;
        }

        .btn-book:hover {
            background: #b89a6b;
            color: #1f2c38;
        }

        .about-container {
            display: flex;
            gap: 35px;
            flex-wrap: wrap;
        }

        .about-text {
            flex: 2;
            font-family: 'Cormorant Garamond', serif;
            font-size: 1.18rem;
            line-height: 1.55;
            color: #1e2b36;
        }

        .advantages-sidebar {
            flex: 1;
            background: #faf6ef;
            padding: 22px;
            border-radius: 24px;
            border: 1px solid #e3d5c0;
        }

        .advantages-sidebar h3 {
            font-weight: 700;
            font-size: 1.5rem;
            margin-bottom: 14px;
        }

        .advantages-sidebar ul {
            list-style: none;
            font-family: 'Inter', sans-serif;
        }

        .advantages-sidebar li::before {
            content: "✓ ";
            color: #b47c44;
        }

        .inspire-block {
            background: #f3efe8;
            margin-top: 30px;
            padding: 20px 26px;
            border-radius: 40px;
            text-align: center;
            border: 1px dashed #b89a6b;
        }
        .inspire-block p {
            font-size: 1.28rem;
            font-style: italic;
            font-family: 'Cormorant Garamond', serif;
            font-weight: 500;
            margin-bottom: 14px;
            color: #2f4050;
        }
        .random-gen-btn {
            background: #1f2c38;
            color: #f0ede8;
            border: none;
            padding: 8px 28px;
            border-radius: 40px;
            cursor: pointer;
            font-family: 'Inter', sans-serif;
            font-weight: 500;
            letter-spacing: 0.3px;
        }
        .random-gen-btn:hover {
            background: #b89a6b;
            color: #1f2c38;
        }

        .reviews-container {
            display: flex;
            flex-direction: column;
            gap: 22px;
        }
        .review-card {
            background: #fefcf8;
            padding: 20px 24px;
            border-radius: 28px;
            display: flex;
            gap: 22px;
            flex-wrap: wrap;
            border: 1px solid #e7dfd3;
            transition: 0.1s;
        }
        .review-card img {
            border-radius: 50%;
            object-fit: cover;
            border: 2px solid #dcc08c;
        }
        .review-card h3 {
            font-family: 'Playfair Display', serif;
            font-weight: 600;
            font-size: 1.2rem;
        }
        .review-card p {
            font-family: 'Inter', sans-serif;
            font-size: 0.96rem;
            margin: 8px 0 4px;
        }
        .review-card time {
            font-size: 0.75rem;
            color: #8b7a66;
        }

        .booking-form {
            max-width: 600px;
            display: flex;
            flex-direction: column;
            gap: 18px;
        }

        .form-group {
            display: flex;
            flex-direction: column;
            gap: 6px;
        }

        .form-group label {
            font-weight: 500;
            font-family: 'Inter', sans-serif;
        }

        .form-group input,
        .form-group select,
        .form-group textarea {
            padding: 12px 14px;
            border: 1px solid #cfc5b6;
            border-radius: 14px;
            font-family: 'Inter', sans-serif;
            background: #fffdf9;
        }
        .form-group input:focus,
        .form-group select:focus {
            border-color: #b89a6b;
            outline: none;
        }

        .consent-group {
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .btn-submit {
            background: #2c3e50;
            color: white;
            padding: 12px 28px;
            border: none;
            border-radius: 44px;
            font-weight: 600;
            font-size: 1rem;
            cursor: pointer;
            width: fit-content;
            transition: 0.2s;
        }

        .btn-submit:hover {
            background: #b89a6b;
            color: #1f2c38;
        }

        .form-message {
            padding: 12px 16px;
            margin-bottom: 18px;
            border-radius: 20px;
            display: none;
        }

        .form-message.success {
            background: #e0eedd;
            color: #1e4620;
            display: block;
        }

        .form-message.error {
            background: #fae1df;
            color: #a52216;
            display: block;
        }

        .error-field {
            border-color: #d95b4a !important;
        }

        .site-footer {
            background: #1f2c38;
            color: #ddd6cd;
            text-align: center;
            padding: 24px;
            margin-top: 28px;
            font-family: 'Inter', sans-serif;
            font-size: 0.9rem;
        }

        @media (max-width: 768px) {
            .site-header {
                flex-direction: column;
                gap: 12px;
                text-align: center;
            }
            .main-nav ul {
                flex-direction: column;
                align-items: center;
                gap: 10px;
            }
            .section-block {
                margin: 18px;
                padding: 22px;
            }
            .hero h1 {
                font-size: 2.2rem;
            }
            .hero p {
                font-size: 1.1rem;
            }
        }
    </style>
</head>
                          
<body>
<header class="site-header">
    <a href="#" class="logo">
        <img src="https://avatars.mds.yandex.net/i?id=7a55d20f9d1ed3681caf5271bd8390ca_l-4592723-images-thumbs&n=13" alt="Логотип компании Мосты" width="50" height="50">
        <span>Мосты</span>
    </a>
    <nav class="main-nav">
        <ul>
            <li><a href="#tours">Экскурсии</a></li>
            <li><a href="#about">О нас</a></li>
            <li><a href="#reviews">Отзывы</a></li>
            <li><a href="#booking">Забронировать</a></li>
            <li><a href="#contact">Контакты</a></li>
        </ul>
    </nav>
</header>

<main>
    <section class="hero">
        <h1>Экскурсии по Санкт-Петербургу</h1>
        <p>Питер… особый воздух, атмосфера и настроение. Это город, прячущий в закоулках двустворчатые окошечки, расположенные у самой земли, старинные обветшалые здания и ветхие особнячки. Здесь можно встретить «Булочные», от которых веет ароматом свежевыпеченного хлеба, и трактир с прекрасной русской кухней и музыкой. Прогулка по Питеру – все равно что прочтение дневника жизни.</p>
        <a href="#booking" class="cta-button">Выбрать экскурсию</a>
    </section>

    <section id="tours" class="section-block">
        <h2>Наши экскурсии</h2>
        <div class="tours-grid">
            <article class="tour-card">
                <img src="https://i.pinimg.com/originals/7e/0a/8a/7e0a8a5063e35c91a1bda92fea180807.jpg?nii=t" alt="Зимний дворец и Дворцовая площадь">
                <h3>Императорский Петербург</h3>
                <p>Эрмитаж, Зимний дворец, Петропавловская крепость. Роскошь и история.</p>
                <ul>
                    <li>4 часа</li>
                    <li>2500 ₽</li>
                </ul>
                <button class="btn-book" data-tour="imperial">Записаться</button>
            </article>
            <article class="tour-card">
                <img src="https://avatars.mds.yandex.net/i?id=463b83d44bc9058e556574953cc0b2c0_l-5146789-images-thumbs&n=13" alt="Вид с крыши на Исаакиевский собор">
                <h3>Петербург с высоты</h3>
                <p>Прогулка по крышам, Исаакиевский собор, лучшие панорамы города.</p>
                <ul>
                    <li>2.5 часа</li>
                    <li>1800 ₽</li>
                </ul>
                <button class="btn-book" data-tour="roofs">Записаться</button>
            </article>
            <article class="tour-card">
                <img src="https://halvamedia.sovcombank.ru/57622/shutterstock_1747647026-(1).jpg" alt="Разводной мост в белую ночь">
                <h3>Магия белых ночей</h3>
                <p>Ночная прогулка на катере под разводными мостами, романтика Невы.</p>
                <ul>
                    <li>2 часа</li>
                    <li>3200 ₽</li>
                </ul>
                <button class="btn-book" data-tour="white-nights">Записаться</button>
            </article>
            <article class="tour-card">
                <img src="https://pic.rutube.ru/video/09/d9/09d91f2bba0036ab79ec3bbcf46803bf.jpg" alt="Памятник Достоевскому в Петербурге">
                <h3>Петербург Достоевского</h3>
                <p>Пешеходный маршрут по местам «Преступления и наказания».</p>
                <ul>
                    <li>3 часа</li>
                    <li>1600 ₽</li>
                </ul>
                <button class="btn-book" data-tour="dostoevsky">Записаться</button>
            </article>
        </div>
    </section>

    <section id="about" class="section-block">
        <h2>О бюро «Мосты»</h2>
        <div class="about-container">
            <div class="about-text">
                <p>Привет! Мы - команда гидов, влюблённых в Санкт-Петербург. Работаем с 2020 года и за это время успели показать город сотням гостей - и каждый раз открываем что-то новое вместе с вами! У нас нет скучных лекций: только живые истории, любопытные факты и необычные ракурсы привычных мест. Мы знаем, где найти самый красивый вид на Неву, какие дворы хранят старинные секреты и какие улицы помнят шаги великих поэтов. Что мы предлагаем: душевные пешеходные прогулки по центру, тематические экскурсии — от дворцов до городских легенд, маршруты для взрослых и детей, гибкие программы: можем адаптировать тур под ваши интересы. Приходите — и Петербург станет для вас ближе и понятнее!</p>
            </div>
            <aside class="advantages-sidebar">
                <h3>Почему мы</h3>
                <ul>
                    <li>Лицензия Минкультуры</li>
                    <li>Группы до 15 человек</li>
                    <li>Авторские маршруты</li>
                    <li>Подход к каждому гостю</li>
                </ul>
            </aside>
        </div>
        <div class="inspire-block">
            <p id="inspirePhrase">Нажмите кнопку — получите вдохновение для прогулки </p>
            <button class="random-gen-btn" id="randomInspireBtn">Магия Петербурга ✨</button>
        </div>
    </section>

    <section id="reviews" class="section-block">
        <h2>Отзывы</h2>
        <div class="reviews-container" id="reviewsList"></div>
        <button id="addRandomReviewBtn" style="margin-top: 26px; background:#2c3e50; color:#fef7e7; padding: 8px 22px; border:none; border-radius: 40px; font-family:'Inter',sans-serif; font-weight:500; cursor:pointer;">Читать далее..</button>
    </section>

    <section id="booking" class="section-block">
        <h2>Забронировать экскурсию</h2>
        <form class="booking-form" id="bookingForm">
            <div class="form-group">
                <label>Имя *</label>
                <input type="text" id="name" placeholder="Анна Иванова" required>
            </div>
            <div class="form-group">
                <label>Email *</label>
                <input type="email" id="email" placeholder="anna@example.com" required>
            </div>
            <div class="form-group">
                <label>Телефон *</label>
                <input type="tel" id="phone" placeholder="+7 999 123-45-67" required>
            </div>
            <div class="form-group">
                <label>Экскурсия *</label>
                <select id="tourSelect" required>
                    <option value="">-- Выберите --</option>
                    <option value="imperial">Императорский Петербург</option>
                    <option value="roofs">Петербург с высоты</option>
                    <option value="white-nights">Магия белых ночей</option>
                    <option value="dostoevsky">Петербург Достоевского</option>
                </select>
            </div>
            <div class="form-group">
                <label>Количество гостей (1-15)</label>
                <input type="number" id="guests" min="1" max="15" value="2">
            </div>
            <div class="consent-group">
                <input type="checkbox" id="consent" required>
                <label>Согласен на обработку данных *</label>
            </div>
            <button type="submit" class="btn-submit">Отправить заявку</button>
        </form>
    </section>

    <section id="contact" class="section-block">
        <h2>Контакты</h2>
        <address style="font-style: normal; font-family: 'Inter', sans-serif;">
            <p>📍 Невский пр., 32, офис 4, Санкт-Петербург</p>
            <p>📞 <a href="tel:+79109545300" style="color:#2c3e50;">+7 (812) 600-80-90</a></p>
            <p>✉️ <a href="mailto:info@spbvenice.ru" style="color:#2c3e50;">info@spbvenice.ru</a></p>
            <p>🕒 09:00 – 22:00 ежедневно</p>
        </address>
    </section>
</main>

<footer class="site-footer">
    <p>© 2026 Экскурсионное бюро «Мосты»</p>
</footer>
                                     
<script>
    (function() {
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    e.preventDefault();
                    target.scrollIntoView({ behavior: 'smooth', block: 'start' });
                }
            });
        });

        const tourSelect = document.getElementById('tourSelect');
        document.querySelectorAll('.btn-book').forEach(btn => {
            btn.addEventListener('click', function() {
                const tourValue = this.getAttribute('data-tour');
                if (tourSelect && tourValue) {
                    tourSelect.value = tourValue;
                    document.getElementById('booking').scrollIntoView({ behavior: 'smooth' });
                }
            });
        });

        const form = document.querySelector('#bookingForm');
        const msgDiv = document.createElement('div');
        msgDiv.className = 'form-message';
        form.parentNode.insertBefore(msgDiv, form);

        function showMessage(text, type) {
            msgDiv.textContent = text;
            msgDiv.className = `form-message ${type}`;
            setTimeout(() => {
                msgDiv.style.display = 'none';
                msgDiv.className = 'form-message';
            }, 4300);
        }

        function markError(id) {
            const field = document.getElementById(id);
            if (field) field.classList.add('error-field');
        }
        function clearErrors() {
            document.querySelectorAll('.error-field').forEach(f => f.classList.remove('error-field'));
        }

        form.addEventListener('submit', function(e) {
            e.preventDefault();
            clearErrors();

            const name = document.getElementById('name');
            const email = document.getElementById('email');
            const phone = document.getElementById('phone');
            const tour = document.getElementById('tourSelect');
            const guests = document.getElementById('guests');
            const consent = document.getElementById('consent');

            let errors = [];

            if (!name.value.trim()) { errors.push('Введите имя.'); markError('name'); }
            if (!email.value.trim() || !/^\S+@\S+\.\S+$/.test(email.value)) { errors.push('Укажите корректный email.'); markError('email'); }
            if (!phone.value.trim() || phone.value.replace(/\D/g,'').length < 10) { errors.push('Введите телефон.'); markError('phone'); }
            if (!tour.value) { errors.push('Выберите экскурсию.'); markError('tourSelect'); }
            const g = parseInt(guests.value);
            if (isNaN(g) || g < 1 || g > 15) { errors.push('Гостей от 1 до 15.'); markError('guests'); }
            if (!consent.checked) { errors.push('Необходимо согласие на обработку данных.'); }

            if (errors.length) {
                showMessage(errors.join(' '), 'error');
                return;
            }

            const btn = form.querySelector('.btn-submit');
            const original = btn.textContent;
            btn.textContent = 'Отправка...';
            btn.disabled = true;
            setTimeout(() => {
                showMessage('Заявка отправлена! Мы свяжемся с вами в ближайшее время.', 'success');
                btn.textContent = original;
                btn.disabled = false;
            }, 800);
        });

        const petersburgPhrases = [
            "Петербург — город белых ночей и разводных мостов, где время течет иначе.",
            "Дворцовый мост разводится под музыку — зрелище, которое нельзя пропустить.",
            "Невский проспект хранит легенды веков, за каждым фасадом — своя история.",
            "Лучший вид на Исаакий — с высоты колоннады или с воды.",
            "Петербург Достоевского: мрачные дворы-колодцы и философия на каждом шагу.",
            "Атмосфера города: гранит, вода, свет и невероятная архитектура."
        ];
        function pickRandomWord(wordsArray) {
            return wordsArray[Math.floor(Math.random() * wordsArray.length)];
        }

        const inspireBtn = document.getElementById('randomInspireBtn');
        const inspireParagraph = document.getElementById('inspirePhrase');
        if (inspireBtn) {
            inspireBtn.addEventListener('click', () => {
                inspireParagraph.innerHTML = `✨ ${pickRandomWord(petersburgPhrases)} ✨`;
            });
        }

        let reviewsData = [
            { name: "Екатерина", city: "Москва", text: "Потрясающие ракурсы Исаакиевского собора! С каждой точки он выглядит по-новому — то монументально и строго, то удивительно изящно. Отдельное спасибо за отличную организацию экскурсии: всё чётко, вовремя, без суеты.", date: "1.5.2026", img: "https://i.pinimg.com/736x/3c/92/a6/3c92a6b6b197e6d58f68d0c7579a0cc7.jpg" },
            { name: "Дмитрий", city: "Кострома", text: "Особенно впечатлил «Достоевский дом» — там такая атмосфера, что мурашки по коже... Чувствуется, как вера и творчество были неразделимы для Фёдора Михайловича. Спасибо за глубокие рассказы!", date: "28.4.2026", img: "https://shakhty-media.ru/wp-content/uploads/2022/06/Dmitrij-Antonev.jpg" }
        ];

        function renderReviews() {
            const container = document.getElementById('reviewsList');
            if (!container) return;
            container.innerHTML = '';
            reviewsData.forEach(review => {
                const reviewDiv = document.createElement('div');
                reviewDiv.className = 'review-card';
                reviewDiv.innerHTML = `
                    <img src="${review.img}" alt="${review.name}" width="60" height="60" style="border-radius:50%; object-fit:cover;">
                    <div>
                        <h3>${review.name}, ${review.city}</h3>
                        <p>«${review.text}»</p>
                        <time>${review.date}</time>
                    </div>
                `;
                container.appendChild(reviewDiv);
            });
        }

        const randomNames = ["Алексей", "Марина", "Олег", "Елена", "Сергей", "Татьяна", "Игорь", "Полина"];
        const randomCities = ["Москва", "Екатеринбург", "Казань", "Нижний Новгород", "Сочи", "Шарья", "Ростов-на-Дону"];
        const reviewTexts = [
            "Невероятная экскурсия! Гид влюблён в своё дело. Узнали столько тайн, что не найти в путеводителях.",
            "Очень понравилась прогулка по крышам — Петербург открылся с новой стороны. Обязательно вернёмся!",
            "Магия белых ночей — это было волшебно! Катера под мостами, атмосфера… Спасибо команде Мосты.",
            "Петербург Достоевского произвёл сильное впечатление. Рекомендую всем, кто любит литературу и историю.",
            "Императорский Петербург: шикарный маршрут, много историй о царской семье. Организация на высоте."
        ];

        function generateRandomReview() {
            return {
                name: pickRandomWord(randomNames),
                city: pickRandomWord(randomCities),
                text: pickRandomWord(reviewTexts),
                date: `${Math.floor(Math.random() * 28) + 1}.${Math.floor(Math.random() * 6) + 1}.2025`,
                img: `https://i.pravatar.cc/100?img=${Math.floor(Math.random() * 70) + 1}`
            };
        }

        const addReviewBtn = document.getElementById('addRandomReviewBtn');
        if (addReviewBtn) {
            addReviewBtn.addEventListener('click', () => {
                reviewsData.unshift(generateRandomReview());
                renderReviews();
                showMessage("Свежий отзыв добавлен! Благодарим за эмоции", "success");
                setTimeout(() => {
                    if (msgDiv.style.display !== 'none') msgDiv.style.display = 'none';
                }, 2000);
            });
        }

        renderReviews();
    })();
</script>
</body>
</html>
