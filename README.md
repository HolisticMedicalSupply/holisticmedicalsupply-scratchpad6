<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DME Product Portfolio</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Segoe UI', sans-serif; background: linear-gradient(135deg, #3498db, #2980b9); padding: 20px; }
        .container { max-width: 1600px; margin: 0 auto; background: white; border-radius: 20px; box-shadow: 0 20px 60px rgba(0,0,0,0.3); }
        .language-toggle { position: sticky; top: 0; z-index: 1000; background: rgba(255,255,255,0.98); padding: 15px 40px; display: flex; justify-content: center; gap: 15px; border-bottom: 3px solid #3498db; box-shadow: 0 3px 15px rgba(0,0,0,0.1); }
        .lang-btn { padding: 12px 30px; border: 2px solid #3498db; background: white; color: #3498db; border-radius: 8px; cursor: pointer; font-size: 1.1em; font-weight: bold; transition: all 0.3s ease; }
        .lang-btn:hover { background: #e8f4f8; transform: translateY(-2px); }
        .lang-btn.active { background: #3498db; color: white; }
        .lang-content { display: none; }
        .lang-content.active { display: block; }
        .header { background: linear-gradient(135deg, #3498db, #2980b9); color: white; padding: 60px 40px; text-align: center; }
        .header h1 { font-size: 4em; margin-bottom: 20px; }
        .section { padding: 50px 40px; }
        .section:nth-child(even) { background: #f8f9fa; }
        .product-category { background: #e8f4f8; padding: 25px; border-radius: 12px; margin: 20px 0; border-left: 5px solid #3498db; }
        .product-category h3 { color: #3498db; margin-bottom: 15px; font-size: 1.6em; }
        ul { line-height: 1.9; margin-left: 20px; }
        ul li { margin: 10px 0; }
        .back-link { display: inline-block; background: #27ae60; color: white; padding: 12px 30px; border-radius: 8px; text-decoration: none; margin: 20px 0; font-weight: bold; }
        .back-link:hover { background: #229954; }
        .stat-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin: 40px 0; }
        .stat-box { background: linear-gradient(135deg, #3498db, #2980b9); color: white; padding: 30px; border-radius: 15px; text-align: center; }
        .stat-number { font-size: 3em; font-weight: bold; display: block; margin-bottom: 10px; }
    </style>
</head>
<body>
    <div class="container">
        <div class="language-toggle">
            <button class="lang-btn active" onclick="switchLanguage('en')" data-lang="en">🇺🇸 English</button>
            <button class="lang-btn" onclick="switchLanguage('ru')" data-lang="ru">🇷🇺 Русский</button>
            <button class="lang-btn" onclick="switchLanguage('uz')" data-lang="uz">🇺🇿 O'zbek</button>
        </div>

        <!-- ENGLISH -->
        <div class="lang-content active" id="content-en">
            <div class="header">
                <h1>🏥 DME PRODUCT PORTFOLIO</h1>
                <p style="font-size: 1.8em;">Complete 36 BOC-Licensed Categories</p>
            </div>

            <div class="section">
                <a href="https://holisticmedicalsupply.github.io/holisticmedicalsupply-scratchpad4/" class="back-link">← Back to Portfolio</a>

                <div class="stat-grid">
                    <div class="stat-box"><span class="stat-number">36</span><span>BOC Categories</span></div>
                    <div class="stat-box"><span class="stat-number">500+</span><span>Product Types</span></div>
                    <div class="stat-box"><span class="stat-number">70-80%</span><span>Revenue from DME</span></div>
                </div>

                <h2 style="font-size: 2.5em; margin: 40px 0 30px 0; text-align: center; color: #2980b9;">BOC Product Categories</h2>

                <div class="product-category">
                    <h3>🦽 Mobility Equipment (M06, M06A, M07, M07A)</h3>
                    <ul>
                        <li><strong>Standard Wheelchairs:</strong> Manual, lightweight, transport chairs ($200-$800)</li>
                        <li><strong>Power Wheelchairs:</strong> Complex rehab, standard power mobility ($2,500-$20,000)</li>
                        <li><strong>Custom Wheelchairs:</strong> Pediatric, bariatric, sports chairs ($500-$8,000)</li>
                        <li><strong>Wheelchair Accessories:</strong> Cushions, backs, trays, positioning ($50-$500)</li>
                    </ul>
                </div>

                <div class="product-category">
                    <h3>🛏️ Hospital Beds & Surfaces (DM11, DM12)</h3>
                    <ul>
                        <li><strong>Semi-Electric Beds:</strong> Basic adjustability ($800-$1,500)</li>
                        <li><strong>Full-Electric Beds:</strong> Complete positioning control ($1,500-$3,500)</li>
                        <li><strong>Bariatric Beds:</strong> Heavy-duty up to 1000 lbs ($2,000-$5,000)</li>
                        <li><strong>Therapeutic Mattresses:</strong> Pressure relief, air mattresses ($300-$2,000)</li>
                    </ul>
                </div>

                <div class="product-category">
                    <h3>🚶 Walking Aids (M05)</h3>
                    <ul>
                        <li><strong>Walkers:</strong> Standard, rolling, knee walkers ($50-$400)</li>
                        <li><strong>Canes:</strong> Single point, quad canes, forearm crutches ($15-$150)</li>
                        <li><strong>Gait Trainers:</strong> Pediatric and adult models ($500-$3,000)</li>
                    </ul>
                </div>

                <div class="product-category">
                    <h3>🦿 Orthotic Devices (OR03, OR04, OR05, OR06, OR07, OR08)</h3>
                    <ul>
                        <li><strong>Lower Extremity:</strong> Knee braces, ankle-foot orthoses ($150-$3,500)</li>
                        <li><strong>Upper Extremity:</strong> Wrist, elbow, shoulder supports ($60-$800)</li>
                        <li><strong>Spinal Orthoses:</strong> Back braces, TLSO, cervical collars ($80-$2,500)</li>
                        <li><strong>Custom Orthotics:</strong> Specialized bracing and supports ($500-$5,000)</li>
                    </ul>
                </div>

                <div class="product-category">
                    <h3>🫁 Respiratory Equipment (DM28, DM29, DM30)</h3>
                    <ul>
                        <li><strong>Oxygen Concentrators:</strong> Stationary and portable units ($800-$3,500)</li>
                        <li><strong>CPAP/BiPAP:</strong> Sleep apnea treatment ($500-$2,500)</li>
                        <li><strong>Nebulizers:</strong> Medication delivery systems ($40-$300)</li>
                        <li><strong>Suction Machines:</strong> Airway clearance devices ($200-$1,000)</li>
                    </ul>
                </div>

                <div class="product-category">
                    <h3>🛁 Bathroom Safety (DM02, DM03, DM04)</h3>
                    <ul>
                        <li><strong>Commodes:</strong> Bedside, drop-arm, bariatric ($100-$800)</li>
                        <li><strong>Shower/Bath Equipment:</strong> Chairs, benches, transfer benches ($80-$500)</li>
                        <li><strong>Grab Bars & Rails:</strong> Safety installation hardware ($30-$200)</li>
                        <li><strong>Raised Toilet Seats:</strong> Height adjustment aids ($25-$150)</li>
                    </ul>
                </div>

                <div class="product-category">
                    <h3>🏋️ Patient Lifts & Transfer (DM21, DM22, DM23)</h3>
                    <ul>
                        <li><strong>Patient Lifts:</strong> Hoyer-style floor lifts ($800-$3,500)</li>
                        <li><strong>Sit-to-Stand Lifts:</strong> Mobility assistance ($1,200-$4,000)</li>
                        <li><strong>Transfer Boards:</strong> Manual transfer aids ($30-$200)</li>
                        <li><strong>Ceiling Lifts:</strong> Permanent installation systems ($3,000-$8,000)</li>
                    </ul>
                </div>

                <div class="product-category">
                    <h3>🩹 Wound Care & Compression (DM15, S01, PD08)</h3>
                    <ul>
                        <li><strong>Compression Pumps:</strong> Lymphedema management ($1,200-$3,500)</li>
                        <li><strong>Compression Garments:</strong> Stockings, sleeves, gloves ($40-$400)</li>
                        <li><strong>Wound VAC:</strong> Negative pressure therapy ($2,000-$5,000)</li>
                        <li><strong>Diabetic Supplies:</strong> Shoes, inserts, wound care ($50-$400)</li>
                    </ul>
                </div>

                <a href="https://holisticmedicalsupply.github.io/holisticmedicalsupply-scratchpad4/" class="back-link">← Back to Portfolio</a>
            </div>
        </div>

        <!-- RUSSIAN -->
        <div class="lang-content" id="content-ru">
            <div class="header">
                <h1>🏥 ПОРТФОЛИО DME ПРОДУКТОВ</h1>
                <p style="font-size: 1.8em;">Полные 36 Лицензированных Категорий BOC</p>
            </div>

            <div class="section">
                <a href="https://holisticmedicalsupply.github.io/holisticmedicalsupply-scratchpad4/" class="back-link">← Назад</a>

                <div class="stat-grid">
                    <div class="stat-box"><span class="stat-number">36</span><span>Категорий BOC</span></div>
                    <div class="stat-box"><span class="stat-number">500+</span><span>Типов Продуктов</span></div>
                    <div class="stat-box"><span class="stat-number">70-80%</span><span>Доход от DME</span></div>
                </div>

                <h2 style="font-size: 2.5em; margin: 40px 0 30px 0; text-align: center; color: #2980b9;">Категории Продуктов BOC</h2>

                <div class="product-category">
                    <h3>🦽 Оборудование для Мобильности</h3>
                    <ul>
                        <li><strong>Стандартные Коляски:</strong> Ручные, легкие, транспортные ($200-$800)</li>
                        <li><strong>Электрические Коляски:</strong> Сложная реабилитация ($2,500-$20,000)</li>
                        <li><strong>Индивидуальные Коляски:</strong> Педиатрические, бариатрические ($500-$8,000)</li>
                    </ul>
                </div>

                <div class="product-category">
                    <h3>🛏️ Больничные Кровати</h3>
                    <ul>
                        <li><strong>Полуэлектрические Кровати:</strong> Базовая регулировка ($800-$1,500)</li>
                        <li><strong>Полностью Электрические:</strong> Полный контроль ($1,500-$3,500)</li>
                        <li><strong>Бариатрические Кровати:</strong> До 1000 фунтов ($2,000-$5,000)</li>
                    </ul>
                </div>

                <a href="https://holisticmedicalsupply.github.io/holisticmedicalsupply-scratchpad4/" class="back-link">← Назад</a>
            </div>
        </div>

        <!-- UZBEK -->
        <div class="lang-content" id="content-uz">
            <div class="header">
                <h1>🏥 DME MAHSULOT PORTFELI</h1>
                <p style="font-size: 1.8em;">To'liq 36 BOC Litsenziyalangan Toifalar</p>
            </div>

            <div class="section">
                <a href="https://holisticmedicalsupply.github.io/holisticmedicalsupply-scratchpad4/" class="back-link">← Orqaga</a>

                <div class="stat-grid">
                    <div class="stat-box"><span class="stat-number">36</span><span>BOC Toifalari</span></div>
                    <div class="stat-box"><span class="stat-number">500+</span><span>Mahsulot Turlari</span></div>
                    <div class="stat-box"><span class="stat-number">70-80%</span><span>DME dan Daromad</span></div>
                </div>

                <h2 style="font-size: 2.5em; margin: 40px 0 30px 0; text-align: center; color: #2980b9;">BOC Mahsulot Toifalari</h2>

                <div class="product-category">
                    <h3>🦽 Harakatlanish Uskunalari</h3>
                    <ul>
                        <li><strong>Standart Aravachalar:</strong> Qo'lda, yengil, transport ($200-$800)</li>
                        <li><strong>Elektr Aravachalar:</strong> Murakkab reabilitatsiya ($2,500-$20,000)</li>
                        <li><strong>Maxsus Aravachalar:</strong> Pediatrik, bariatrik ($500-$8,000)</li>
                    </ul>
                </div>

                <div class="product-category">
                    <h3>🛏️ Kasalxona Karavotlari</h3>
                    <ul>
                        <li><strong>Yarim Elektr Karavotlar:</strong> Asosiy sozlash ($800-$1,500)</li>
                        <li><strong>To'liq Elektr:</strong> To'liq boshqaruv ($1,500-$3,500)</li>
                        <li><strong>Bariatrik Karavotlar:</strong> 1000 funtgacha ($2,000-$5,000)</li>
                    </ul>
                </div>

                <a href="https://holisticmedicalsupply.github.io/holisticmedicalsupply-scratchpad4/" class="back-link">← Orqaga</a>
            </div>
        </div>
    </div>

    <script>
        function switchLanguage(lang) {
            document.querySelectorAll('.lang-content').forEach(content => content.classList.remove('active'));
            document.querySelectorAll('.lang-btn').forEach(btn => btn.classList.remove('active'));
            document.getElementById('content-' + lang).classList.add('active');
            document.querySelector(`.lang-btn[data-lang="${lang}"]`).classList.add('active');
            localStorage.setItem('preferred-language', lang);
            window.scrollTo(0, 0);
        }
        window.addEventListener('DOMContentLoaded', function() {
            const savedLang = localStorage.getItem('preferred-language');
            if (savedLang && ['en', 'ru', 'uz'].includes(savedLang)) switchLanguage(savedLang);
        });
    </script>
</body>
</html>
