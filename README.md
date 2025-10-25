<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DME Product Portfolio | Holistic Medical Supply - 36 BOC Categories</title>
    <meta name="description" content="Complete catalog of 36 BOC-licensed DME categories with 4-tier pricing, Medicare reimbursement info, and revenue projections.">
    <style>
        :root {
            --primary-blue: #1e3c72;
            --secondary-blue: #2a5298;
            --accent-purple: #667eea;
            --accent-violet: #764ba2;
            --success-green: #27ae60;
            --warning-orange: #f39c12;
            --danger-red: #e74c3c;
            --light-bg: #f8f9fa;
            --white: #ffffff;
            --text-dark: #333333;
            --text-light: #666666;
            --gold: #f1c40f;
            --silver: #95a5a6;
            --bronze: #cd7f32;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--text-dark);
            background: linear-gradient(135deg, var(--accent-purple) 0%, var(--accent-violet) 100%);
            padding: 20px;
        }

        .container {
            max-width: 1600px;
            margin: 0 auto;
            background: var(--white);
            border-radius: 20px;
            box-shadow: 0 20px 80px rgba(0, 0, 0, 0.3);
            overflow: hidden;
        }

        /* Language Toggle */
        .language-toggle {
            position: sticky;
            top: 0;
            z-index: 1000;
            background: rgba(255, 255, 255, 0.98);
            backdrop-filter: blur(10px);
            padding: 20px 40px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 3px solid var(--accent-purple);
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
        }

        .nav-links {
            display: flex;
            gap: 15px;
            align-items: center;
        }

        .back-link {
            padding: 10px 25px;
            background: var(--light-bg);
            color: var(--primary-blue);
            text-decoration: none;
            border-radius: 8px;
            font-weight: 600;
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .back-link:hover {
            background: var(--accent-purple);
            color: var(--white);
            transform: translateX(-3px);
        }

        .lang-buttons {
            display: flex;
            gap: 10px;
        }

        .lang-btn {
            padding: 10px 25px;
            border: 2px solid var(--accent-purple);
            background: var(--white);
            color: var(--accent-purple);
            border-radius: 8px;
            cursor: pointer;
            font-size: 0.95em;
            font-weight: bold;
            transition: all 0.3s ease;
        }

        .lang-btn:hover {
            background: #f0f0ff;
            transform: translateY(-2px);
        }

        .lang-btn.active {
            background: linear-gradient(135deg, var(--accent-purple), var(--accent-violet));
            color: var(--white);
        }

        .lang-content {
            display: none;
        }

        .lang-content.active {
            display: block;
            animation: fadeIn 0.5s ease-in;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Header */
        .header {
            background: linear-gradient(135deg, var(--primary-blue) 0%, var(--secondary-blue) 100%);
            color: var(--white);
            padding: 60px 60px 40px;
            position: relative;
            overflow: hidden;
        }

        .doc-badge {
            display: inline-block;
            padding: 8px 20px;
            background: var(--success-green);
            color: var(--white);
            border-radius: 20px;
            font-size: 0.9em;
            font-weight: bold;
            margin-bottom: 15px;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .header h1 {
            font-size: 3.5em;
            margin-bottom: 15px;
            font-weight: 800;
            position: relative;
            z-index: 1;
        }

        .header .subtitle {
            font-size: 1.5em;
            opacity: 0.95;
            margin-bottom: 30px;
        }

        .header-stats {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 40px;
        }

        .header-stat {
            background: rgba(255, 255, 255, 0.15);
            backdrop-filter: blur(10px);
            padding: 20px;
            border-radius: 12px;
            text-align: center;
        }

        .header-stat .number {
            font-size: 2.5em;
            font-weight: bold;
            display: block;
            margin-bottom: 5px;
        }

        .header-stat .label {
            font-size: 1em;
            opacity: 0.9;
        }

        /* Section Styling */
        .section {
            padding: 60px;
        }

        .section:nth-child(even) {
            background: var(--light-bg);
        }

        .section-header {
            text-align: center;
            margin-bottom: 50px;
        }

        .section-title {
            font-size: 2.8em;
            color: var(--primary-blue);
            margin-bottom: 15px;
            font-weight: 800;
            position: relative;
            display: inline-block;
            padding-bottom: 15px;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 4px;
            background: linear-gradient(90deg, var(--accent-purple), var(--accent-violet));
            border-radius: 2px;
        }

        .section-subtitle {
            font-size: 1.2em;
            color: var(--text-light);
            max-width: 800px;
            margin: 15px auto 0;
        }

        /* Info Boxes */
        .info-box {
            background: var(--white);
            border-left: 5px solid var(--accent-purple);
            padding: 25px;
            border-radius: 10px;
            margin: 20px 0;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.08);
        }

        .info-box.success {
            border-left-color: var(--success-green);
            background: #f0fff4;
        }

        .info-box h4 {
            font-size: 1.3em;
            margin-bottom: 15px;
            color: var(--primary-blue);
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .info-box ul {
            margin-left: 20px;
            line-height: 1.8;
        }

        .info-box li {
            margin: 8px 0;
            color: var(--text-dark);
        }

        .info-box p {
            margin: 10px 0;
            line-height: 1.8;
        }

        /* Summary Tables */
        .summary-table {
            background: var(--white);
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.1);
            margin: 30px 0;
        }

        table {
            width: 100%;
            border-collapse: collapse;
        }

        thead {
            background: linear-gradient(135deg, var(--primary-blue) 0%, var(--secondary-blue) 100%);
            color: var(--white);
        }

        th {
            padding: 20px;
            text-align: left;
            font-weight: 700;
            font-size: 1.1em;
        }

        tbody tr {
            border-bottom: 1px solid var(--light-bg);
            transition: background 0.2s ease;
        }

        tbody tr:hover {
            background: var(--light-bg);
        }

        td {
            padding: 18px 20px;
            color: var(--text-dark);
        }

        .table-number {
            font-weight: 700;
            color: var(--success-green);
        }

        /* CTA Section */
        .cta-section {
            background: linear-gradient(135deg, var(--primary-blue) 0%, var(--secondary-blue) 100%);
            color: var(--white);
            padding: 60px;
            text-align: center;
        }

        .cta-section h2 {
            font-size: 2.5em;
            margin-bottom: 20px;
        }

        .cta-section p {
            font-size: 1.3em;
            margin-bottom: 30px;
            opacity: 0.95;
        }

        .cta-buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }

        .cta-btn {
            padding: 18px 40px;
            font-size: 1.1em;
            font-weight: bold;
            border-radius: 10px;
            text-decoration: none;
            transition: all 0.3s ease;
            display: inline-flex;
            align-items: center;
            gap: 10px;
        }

        .cta-btn.primary {
            background: var(--success-green);
            color: var(--white);
        }

        .cta-btn.primary:hover {
            background: #229954;
            transform: translateY(-3px);
            box-shadow: 0 10px 30px rgba(39, 174, 96, 0.4);
        }

        .cta-btn.secondary {
            background: var(--white);
            color: var(--primary-blue);
        }

        .cta-btn.secondary:hover {
            background: var(--light-bg);
            transform: translateY(-3px);
        }

        /* Footer */
        .footer {
            background: linear-gradient(135deg, var(--primary-blue) 0%, var(--secondary-blue) 100%);
            color: var(--white);
            padding: 40px 60px;
            text-align: center;
        }

        .footer p {
            opacity: 0.9;
            margin: 5px 0;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            body { padding: 10px; }
            .header, .section { padding: 30px 20px; }
            .header h1 { font-size: 2.2em; }
            .section-title { font-size: 1.8em; }
            .language-toggle {
                flex-direction: column;
                gap: 15px;
                padding: 15px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Language Toggle & Navigation -->
        <div class="language-toggle">
            <div class="nav-links">
                <a href="PRIMARY-LANDING-PAGE.html" class="back-link">
                    ← Back to Portfolio
                </a>
            </div>
            <div class="lang-buttons">
                <button class="lang-btn active" onclick="switchLanguage('en')" data-lang="en">🇺🇸 EN</button>
                <button class="lang-btn" onclick="switchLanguage('ru')" data-lang="ru">🇷🇺 RU</button>
                <button class="lang-btn" onclick="switchLanguage('uz')" data-lang="uz">🇺🇿 UZ</button>
            </div>
        </div>

        <!-- ENGLISH CONTENT -->
        <div class="lang-content active" id="content-en">
            <!-- Header -->
            <div class="header">
                <span class="doc-badge">Document 3 | Critical</span>
                <h1>🏥 Complete DME Product Portfolio</h1>
                <p class="subtitle">Comprehensive Catalog of 36 BOC-Licensed Medical Equipment Categories</p>
                
                <div class="header-stats">
                    <div class="header-stat">
                        <span class="number">36</span>
                        <span class="label">BOC-Licensed Categories</span>
                    </div>
                    <div class="header-stat">
                        <span class="number">200+</span>
                        <span class="label">Product SKUs</span>
                    </div>
                    <div class="header-stat">
                        <span class="number">4</span>
                        <span class="label">Pricing Tiers</span>
                    </div>
                    <div class="header-stat">
                        <span class="number">$3.2M-$7.1M</span>
                        <span class="label">Annual Revenue Potential</span>
                    </div>
                </div>
            </div>

            <!-- Portfolio Overview -->
            <div class="section">
                <div class="section-header">
                    <h2 class="section-title">Portfolio Overview</h2>
                    <p class="section-subtitle">
                        Complete coverage across 36 BOC-licensed categories serving all DME market segments
                    </p>
                </div>

                <div class="info-box success">
                    <h4>✅ Complete Product Portfolio - All 36 BOC Categories</h4>
                    <p><strong>This document provides a comprehensive overview of all 36 BOC-licensed product categories available through Holistic Medical Supply.</strong> Each category includes detailed product examples, 4-tier pricing structure, revenue projections, and strategic alignment with our 11 growth strategies.</p>
                    
                    <p style="margin-top: 20px;"><strong>Portfolio Highlights:</strong></p>
                    <ul>
                        <li><strong>36 BOC Categories:</strong> Complete licensing for all mobility, home DME, respiratory, orthotic, prosthetic, and medical supply categories</li>
                        <li><strong>200+ Product SKUs:</strong> Extensive product selection across economy, value, US-made, and luxury tiers</li>
                        <li><strong>4-Tier Pricing:</strong> Economy (25-35% margin), Value (35-45% margin), US-Made (40-50% margin), Luxury (45-55% margin)</li>
                        <li><strong>Medicare/Medicaid Eligible:</strong> 100% of products qualify for insurance reimbursement with proper documentation</li>
                        <li><strong>Multi-Strategy Integration:</strong> Products support all 11 growth strategies for diversified revenue</li>
                        <li><strong>Recurring Revenue Opportunities:</strong> CPAP supplies, diabetic testing, oxygen supplies, compression garments</li>
                    </ul>
                </div>

                <div class="summary-table">
                    <table>
                        <thead>
                            <tr>
                                <th>Category Group</th>
                                <th>BOC Codes</th>
                                <th>Product Count</th>
                                <th>Avg. Gross Margin</th>
                                <th>Annual Revenue Potential</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td><strong>Mobility Equipment</strong></td>
                                <td>M01-M09</td>
                                <td>45+ SKUs</td>
                                <td class="table-number">38-48%</td>
                                <td class="table-number">$800K-$1.8M</td>
                            </tr>
                            <tr>
                                <td><strong>Home DME</strong></td>
                                <td>DM01-DM29</td>
                                <td>80+ SKUs</td>
                                <td class="table-number">35-45%</td>
                                <td class="table-number">$1.2M-$2.5M</td>
                            </tr>
                            <tr>
                                <td><strong>Compression & Support</strong></td>
                                <td>S01-S04</td>
                                <td>30+ SKUs</td>
                                <td class="table-number">45-55%</td>
                                <td class="table-number">$400K-$900K</td>
                            </tr>
                            <tr>
                                <td><strong>Orthotics</strong></td>
                                <td>OR01-OR04</td>
                                <td>25+ SKUs</td>
                                <td class="table-number">42-52%</td>
                                <td class="table-number">$350K-$750K</td>
                            </tr>
                            <tr>
                                <td><strong>Prosthetics</strong></td>
                                <td>PR01-PR02</td>
                                <td>15+ SKUs</td>
                                <td class="table-number">40-50%</td>
                                <td class="table-number">$200K-$500K</td>
                            </tr>
                            <tr>
                                <td><strong>Medical Supplies</strong></td>
                                <td>SU01-SU03</td>
                                <td>35+ SKUs</td>
                                <td class="table-number">48-58%</td>
                                <td class="table-number">$450K-$1.0M</td>
                            </tr>
                            <tr style="background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%); font-weight: bold; font-size: 1.15em;">
                                <td colspan="4"><strong>TOTAL PORTFOLIO (All 36 Categories)</strong></td>
                                <td class="table-number" style="font-size: 1.3em;">$3.2M-$7.1M</td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>

            <!-- Detailed Category Breakdown -->
            <div class="section">
                <div class="section-header">
                    <h2 class="section-title">Complete 36-Category Breakdown</h2>
                    <p class="section-subtitle">
                        Detailed product examples, pricing tiers, and revenue projections for each BOC category
                    </p>
                </div>

                <div class="info-box">
                    <h4>📋 Category Organization</h4>
                    <p>Our 36 BOC-licensed categories are organized into six major product groups:</p>
                    <ul>
                        <li><strong>Group 1: Mobility Equipment (M01-M09)</strong> - Canes, crutches, walkers, wheelchairs, bath safety</li>
                        <li><strong>Group 2: Home DME (DM01-DM11)</strong> - Hospital beds, patient lifts, bathroom safety, monitoring equipment</li>
                        <li><strong>Group 3: Respiratory Equipment (DM06-DM07, DM28-DM29)</strong> - Nebulizers, CPAP/BiPAP, oxygen concentrators</li>
                        <li><strong>Group 4: Compression & Support (S01-S04)</strong> - Compression stockings, lymphedema pumps, diabetic shoes</li>
                        <li><strong>Group 5: Orthotics & Prosthetics (OR01-OR04, PR01-PR02)</strong> - Custom braces, orthotic devices, prosthetic limbs</li>
                        <li><strong>Group 6: Medical Supplies (SU01-SU03)</strong> - Wound care, ostomy supplies, urological products</li>
                    </ul>
                </div>

                <div class="summary-table">
                    <table>
                        <thead>
                            <tr>
                                <th style="width: 10%;">BOC Code</th>
                                <th style="width: 30%;">Category Name</th>
                                <th style="width: 35%;">Key Products & Pricing Range</th>
                                <th style="width: 15%;">Annual Revenue</th>
                                <th style="width: 10%;">Strategies</th>
                            </tr>
                        </thead>
                        <tbody>
                            <!-- MOBILITY EQUIPMENT (M01-M09) -->
                            <tr style="background: #e8f8f5;">
                                <td colspan="5"><strong>MOBILITY EQUIPMENT</strong></td>
                            </tr>
                            <tr>
                                <td><strong>M01</strong></td>
                                <td>Canes & Walking Sticks</td>
                                <td>Standard aluminum ($15-$150), Offset handle ($20-$180), Quad canes ($30-$220)</td>
                                <td class="table-number">$18K-$45K</td>
                                <td>2, 7, 11</td>
                            </tr>
                            <tr>
                                <td><strong>M02</strong></td>
                                <td>Crutches</td>
                                <td>Underarm crutches ($25-$200), Forearm crutches ($35-$250)</td>
                                <td class="table-number">$20K-$50K</td>
                                <td>1, 7, 8</td>
                            </tr>
                            <tr>
                                <td><strong>M03</strong></td>
                                <td>Bath Safety Equipment</td>
                                <td>Shower chairs ($40-$300), Transfer benches ($55-$380), Grab bars ($30-$250)</td>
                                <td class="table-number">$45K-$110K</td>
                                <td>5, 9, 11</td>
                            </tr>
                            <tr>
                                <td><strong>M04</strong></td>
                                <td>Bedside Commodes</td>
                                <td>Standard commodes ($45-$350), Bariatric drop-arm ($80-$520)</td>
                                <td class="table-number">$40K-$95K</td>
                                <td>1, 5, 8</td>
                            </tr>
                            <tr>
                                <td><strong>M05</strong></td>
                                <td>Walkers & Rollators</td>
                                <td>Folding walkers ($35-$280), 2-wheel ($50-$390), 4-wheel rollators ($80-$520)</td>
                                <td class="table-number">$90K-$220K</td>
                                <td>1, 2, 5, 6</td>
                            </tr>
                            <tr>
                                <td><strong>M06</strong></td>
                                <td>Manual Wheelchairs</td>
                                <td>Standard steel ($150-$1,500), Transport ($120-$1,200), Ultra-light ($450-$3,800)</td>
                                <td class="table-number">$200K-$500K</td>
                                <td>1, 5, 6, 8</td>
                            </tr>
                            <tr>
                                <td><strong>M06A</strong></td>
                                <td>Power Wheelchairs</td>
                                <td>Standard power ($2,000-$8,000), Mid-wheel drive ($3,500-$12,000), Standing ($8,000-$25,000)</td>
                                <td class="table-number">$300K-$750K</td>
                                <td>1, 4, 6, 8</td>
                            </tr>
                            <tr>
                                <td><strong>M07</strong></td>
                                <td>Pediatric Wheelchairs</td>
                                <td>Pediatric manual ($500-$2,500), Pediatric power ($3,000-$15,000)</td>
                                <td class="table-number">$60K-$180K</td>
                                <td>8 (Ped)</td>
                            </tr>
                            <tr>
                                <td><strong>M08</strong></td>
                                <td>Wheelchair Accessories</td>
                                <td>Cushions ($50-$400), Armrests ($30-$200), Wheels/tires ($40-$300)</td>
                                <td class="table-number">$35K-$90K</td>
                                <td>All</td>
                            </tr>
                            <tr>
                                <td><strong>M09</strong></td>
                                <td>Traction Equipment</td>
                                <td>Cervical traction ($100-$500), Lumbar traction devices ($150-$800)</td>
                                <td class="table-number">$15K-$40K</td>
                                <td>8, 11</td>
                            </tr>

                            <!-- HOME DME (DM01-DM11) -->
                            <tr style="background: #ebf5fb;">
                                <td colspan="5"><strong>HOME DME EQUIPMENT</strong></td>
                            </tr>
                            <tr>
                                <td><strong>DM01</strong></td>
                                <td>Hospital Beds</td>
                                <td>Semi-electric ($800-$2,800), Full-electric ($1,500-$5,000), Bariatric ($2,500-$8,000)</td>
                                <td class="table-number">$250K-$600K</td>
                                <td>1, 4, 9, 11</td>
                            </tr>
                            <tr>
                                <td><strong>DM02</strong></td>
                                <td>Bathroom Safety Products</td>
                                <td>Toilet safety frames ($35-$200), Raised toilet seats ($25-$150)</td>
                                <td class="table-number">$30K-$75K</td>
                                <td>5, 9, 11</td>
                            </tr>
                            <tr>
                                <td><strong>DM03</strong></td>
                                <td>Patient Lifts</td>
                                <td>Manual floor lifts ($600-$2,000), Electric lifts ($1,200-$4,500), Ceiling lifts ($3,000-$10,000)</td>
                                <td class="table-number">$150K-$400K</td>
                                <td>1, 4, 9, 11</td>
                            </tr>
                            <tr>
                                <td><strong>DM04</strong></td>
                                <td>Trapeze Equipment</td>
                                <td>Bed trapeze bars ($80-$300), Free-standing trapeze ($150-$600)</td>
                                <td class="table-number">$20K-$50K</td>
                                <td>9, 11</td>
                            </tr>
                            <tr>
                                <td><strong>DM05</strong></td>
                                <td>Blood Glucose Monitors</td>
                                <td>Basic meters ($25-$80), Advanced meters ($80-$200) + recurring test strips</td>
                                <td class="table-number">$60K-$180K</td>
                                <td>3, 6, 10, 11</td>
                            </tr>
                            <tr>
                                <td><strong>DM06</strong></td>
                                <td>Nebulizers</td>
                                <td>Compressor nebulizers ($50-$150), Portable mesh ($100-$300)</td>
                                <td class="table-number">$35K-$85K</td>
                                <td>3, 6, 10, 11</td>
                            </tr>
                            <tr>
                                <td><strong>DM07</strong></td>
                                <td>CPAP/BiPAP Equipment</td>
                                <td>CPAP auto-adjusting ($400-$3,000), BiPAP ($800-$5,500) + recurring supplies</td>
                                <td class="table-number">$350K-$850K</td>
                                <td>4, 6, 10, 11</td>
                            </tr>
                            <tr>
                                <td><strong>DM08</strong></td>
                                <td>Heat/Cold Therapy</td>
                                <td>Heating pads ($20-$100), Ice therapy systems ($150-$500)</td>
                                <td class="table-number">$25K-$65K</td>
                                <td>8, 11</td>
                            </tr>
                            <tr>
                                <td><strong>DM09</strong></td>
                                <td>Traction Equipment</td>
                                <td>Home traction devices ($150-$800)</td>
                                <td class="table-number">$15K-$40K</td>
                                <td>8, 11</td>
                            </tr>
                            <tr>
                                <td><strong>DM10</strong></td>
                                <td>Light Therapy</td>
                                <td>Phototherapy lamps ($100-$500)</td>
                                <td class="table-number">$12K-$35K</td>
                                <td>11</td>
                            </tr>
                            <tr>
                                <td><strong>DM11</strong></td>
                                <td>Hospital Beds (Full Featured)</td>
                                <td>Low hospital beds ($1,200-$4,000), Bariatric hospital beds ($2,500-$8,000)</td>
                                <td class="table-number">$100K-$280K</td>
                                <td>1, 4, 9, 11</td>
                            </tr>

                            <!-- RESPIRATORY EQUIPMENT -->
                            <tr style="background: #fef5e7;">
                                <td colspan="5"><strong>RESPIRATORY EQUIPMENT</strong></td>
                            </tr>
                            <tr>
                                <td><strong>DM28</strong></td>
                                <td>Oxygen Equipment (Stationary)</td>
                                <td>Stationary concentrators ($600-$2,500), High-flow systems ($1,200-$4,000)</td>
                                <td class="table-number">$200K-$500K</td>
                                <td>3, 4, 10, 11</td>
                            </tr>
                            <tr>
                                <td><strong>DM29</strong></td>
                                <td>Oxygen Equipment (Portable)</td>
                                <td>Portable concentrators ($1,500-$3,500), Portable oxygen systems ($800-$2,000)</td>
                                <td class="table-number">$180K-$450K</td>
                                <td>3, 4, 10, 11</td>
                            </tr>

                            <!-- COMPRESSION & SUPPORT -->
                            <tr style="background: #fadbd8;">
                                <td colspan="5"><strong>COMPRESSION & SUPPORT PRODUCTS</strong></td>
                            </tr>
                            <tr>
                                <td><strong>S01</strong></td>
                                <td>Compression Stockings</td>
                                <td>Knee-high 20-30mmHg ($25-$220), Thigh-high 30-40mmHg ($40-$330)</td>
                                <td class="table-number">$60K-$150K</td>
                                <td>2, 5, 7, 8</td>
                            </tr>
                            <tr>
                                <td><strong>S02</strong></td>
                                <td>Lymphedema Pumps</td>
                                <td>Sequential pumps ($1,200-$4,500), Advanced pneumatic ($2,500-$7,000)</td>
                                <td class="table-number">$80K-$220K</td>
                                <td>6, 10, 11</td>
                            </tr>
                            <tr>
                                <td><strong>S03</strong></td>
                                <td>Orthotic Braces</td>
                                <td>Knee braces ($60-$500), Ankle braces ($40-$300), Back supports ($50-$400)</td>
                                <td class="table-number">$180K-$430K</td>
                                <td>2, 7, 8, 11</td>
                            </tr>
                            <tr>
                                <td><strong>S04</strong></td>
                                <td>Diabetic/Therapeutic Shoes</td>
                                <td>Depth-style diabetic shoes ($80-$600), Custom molded ($200-$1,400)</td>
                                <td class="table-number">$80K-$200K</td>
                                <td>2, 7, 11</td>
                            </tr>

                            <!-- ORTHOTICS -->
                            <tr style="background: #e8daef;">
                                <td colspan="5"><strong>ORTHOTICS</strong></td>
                            </tr>
                            <tr>
                                <td><strong>OR01</strong></td>
                                <td>Custom Orthotics</td>
                                <td>Custom foot orthotics ($200-$800), Specialty orthotics ($300-$1,200)</td>
                                <td class="table-number">$120K-$300K</td>
                                <td>2, 7, 8, 11</td>
                            </tr>
                            <tr>
                                <td><strong>OR02</strong></td>
                                <td>Spinal Orthotics</td>
                                <td>TLSO braces ($800-$2,500), Cervical collars ($60-$400)</td>
                                <td class="table-number">$80K-$200K</td>
                                <td>8, 11</td>
                            </tr>
                            <tr>
                                <td><strong>OR03</strong></td>
                                <td>Lower Extremity Orthotics</td>
                                <td>AFO braces ($400-$1,500), KAFO braces ($800-$3,000)</td>
                                <td class="table-number">$90K-$180K</td>
                                <td>8, 11</td>
                            </tr>
                            <tr>
                                <td><strong>OR04</strong></td>
                                <td>Upper Extremity Orthotics</td>
                                <td>Wrist/hand orthoses ($80-$500), Shoulder stabilizers ($120-$700)</td>
                                <td class="table-number">$60K-$150K</td>
                                <td>8, 11</td>
                            </tr>

                            <!-- PROSTHETICS -->
                            <tr style="background: #f4ecf7;">
                                <td colspan="5"><strong>PROSTHETICS</strong></td>
                            </tr>
                            <tr>
                                <td><strong>PR01</strong></td>
                                <td>Prosthetic Limbs</td>
                                <td>Below-knee prosthetics ($5,000-$20,000), Above-knee ($10,000-$50,000)</td>
                                <td class="table-number">$150K-$400K</td>
                                <td>8 (Vet), 11</td>
                            </tr>
                            <tr>
                                <td><strong>PR02</strong></td>
                                <td>Prosthetic Components</td>
                                <td>Feet ($800-$5,000), Knees ($2,000-$15,000), Sockets ($1,000-$6,000)</td>
                                <td class="table-number">$50K-$150K</td>
                                <td>8 (Vet), 11</td>
                            </tr>

                            <!-- MEDICAL SUPPLIES -->
                            <tr style="background: #d5f4e6;">
                                <td colspan="5"><strong>MEDICAL SUPPLIES</strong></td>
                            </tr>
                            <tr>
                                <td><strong>SU01</strong></td>
                                <td>Wound Care Supplies</td>
                                <td>Dressings ($5-$80), Negative pressure wound therapy ($800-$3,000)</td>
                                <td class="table-number">$200K-$500K</td>
                                <td>3, 5, 11</td>
                            </tr>
                            <tr>
                                <td><strong>SU02</strong></td>
                                <td>Ostomy Supplies</td>
                                <td>Pouches ($10-$50), Barriers ($8-$40), Complete systems ($50-$200)</td>
                                <td class="table-number">$150K-$350K</td>
                                <td>5, 11</td>
                            </tr>
                            <tr>
                                <td><strong>SU03</strong></td>
                                <td>Urological Supplies</td>
                                <td>Catheters ($5-$30), Drainage bags ($10-$50), Incontinence products ($15-$80)</td>
                                <td class="table-number">$100K-$250K</td>
                                <td>5, 11</td>
                            </tr>

                            <!-- TOTAL ROW -->
                            <tr style="background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%); font-weight: bold; font-size: 1.2em;">
                                <td colspan="3"><strong>TOTAL: ALL 36 BOC CATEGORIES</strong></td>
                                <td class="table-number" style="font-size: 1.4em;">$3.2M-$7.1M</td>
                                <td><strong>All 11</strong></td>
                            </tr>
                        </tbody>
                    </table>
                </div>

                <div class="info-box success">
                    <h4>💡 Portfolio Strategy Notes</h4>
                    <ul>
                        <li><strong>Strategy Numbers Reference:</strong> 1=Hospital, 2=Golf, 3=Resilient, 4=Rental, 5=Facilities, 6=E-Commerce, 7=Pharmacy, 8=Specialty, 9=Home Mod, 10=Virtual Care, 11=General</li>
                        <li><strong>Highest Volume Categories:</strong> M05 (Walkers), M06 (Wheelchairs), S01 (Compression), DM07 (CPAP)</li>
                        <li><strong>Highest Margin Categories:</strong> S01-S04 (Compression/Support), SU01-SU03 (Medical Supplies)</li>
                        <li><strong>Recurring Revenue Stars:</strong> DM05 (Diabetic supplies), DM07 (CPAP supplies), DM28/29 (Oxygen)</li>
                        <li><strong>Premium Categories:</strong> M06A (Power wheelchairs), PR01-PR02 (Prosthetics), DM01/DM11 (Hospital beds)</li>
                    </ul>
                </div>
            </div>

            <!-- CTA Section -->
            <div class="cta-section">
                <h2>📊 Ready to Implement These Products?</h2>
                <p>
                    Explore our detailed strategy documents to see how these 36 product categories integrate 
                    into each growth strategy with specific revenue projections and implementation plans.
                </p>
                <div class="cta-buttons">
                    <a href="PRIMARY-LANDING-PAGE.html#all-strategies" class="cta-btn primary">
                        View All 11 Strategies →
                    </a>
                    <a href="complete-revenue-summary.html" class="cta-btn secondary">
                        See Revenue Projections →
                    </a>
                </div>
            </div>

            <!-- Footer -->
            <div class="footer">
                <p><strong>Holistic Medical Supply</strong> | Complete DME Product Portfolio</p>
                <p>Document 3 of 34 | Last Updated: October 25, 2025 | Version 1.0</p>
                <p>Nassau County, New York | 36 BOC-Licensed Categories | $3.2M-$7.1M Annual Revenue Potential</p>
            </div>
        </div>

        <!-- RUSSIAN & UZBEK CONTENT (Abbreviated versions) -->
        <div class="lang-content" id="content-ru">
            <div class="header">
                <span class="doc-badge">Документ 3 | Критический</span>
                <h1>🏥 Полный портфель продуктов DME</h1>
                <p class="subtitle">Комплексный каталог 36 лицензированных категорий BOC</p>
                
                <div class="header-stats">
                    <div class="header-stat">
                        <span class="number">36</span>
                        <span class="label">Категорий BOC</span>
                    </div>
                    <div class="header-stat">
                        <span class="number">200+</span>
                        <span class="label">SKU продуктов</span>
                    </div>
                    <div class="header-stat">
                        <span class="number">4</span>
                        <span class="label">Ценовых уровня</span>
                    </div>
                    <div class="header-stat">
                        <span class="number">$3.2M-$7.1M</span>
                        <span class="label">Годовой потенциал</span>
                    </div>
                </div>
            </div>

            <div class="section">
                <div class="info-box success">
                    <h4>📊 Обзор портфеля - Все 36 категорий BOC</h4>
                    <p>Полная информация о всех 36 лицензированных категориях доступна в английской версии документа.</p>
                    <p><strong>Основные группы продуктов:</strong></p>
                    <ul>
                        <li><strong>Оборудование для мобильности (M01-M09):</strong> $800K-$1.8M годовой доход</li>
                        <li><strong>Домашнее DME (DM01-DM29):</strong> $1.2M-$2.5M годовой доход</li>
                        <li><strong>Компрессия и поддержка (S01-S04):</strong> $400K-$900K годовой доход</li>
                        <li><strong>Ортопедия (OR01-OR04):</strong> $350K-$750K годовой доход</li>
                        <li><strong>Протезирование (PR01-PR02):</strong> $200K-$500K годовой доход</li>
                        <li><strong>Медицинские принадлежности (SU01-SU03):</strong> $450K-$1.0M годовой доход</li>
                    </ul>
                    <p><strong>Общий потенциал:</strong> $3.2M-$7.1M годовой доход по всем 36 категориям</p>
                </div>
            </div>

            <div class="cta-section">
                <h2>📊 Готовы внедрить эти продукты?</h2>
                <div class="cta-buttons">
                    <a href="PRIMARY-LANDING-PAGE.html#all-strategies" class="cta-btn primary">
                        Все 11 стратегий →
                    </a>
                    <a href="complete-revenue-summary.html" class="cta-btn secondary">
                        Прогнозы доходов →
                    </a>
                </div>
            </div>

            <div class="footer">
                <p><strong>Holistic Medical Supply</strong> | Полный портфель продуктов DME</p>
                <p>Документ 3 из 34 | 25 октября 2025 | Версия 1.0</p>
            </div>
        </div>

        <div class="lang-content" id="content-uz">
            <div class="header">
                <span class="doc-badge">Hujjat 3 | Muhim</span>
                <h1>🏥 To'liq DME mahsulot portfeli</h1>
                <p class="subtitle">36 BOC litsenziyalangan toifalarning kompleks katalogi</p>
                
                <div class="header-stats">
                    <div class="header-stat">
                        <span class="number">36</span>
                        <span class="label">BOC toifalar</span>
                    </div>
                    <div class="header-stat">
                        <span class="number">200+</span>
                        <span class="label">Mahsulot SKU</span>
                    </div>
                    <div class="header-stat">
                        <span class="number">4</span>
                        <span class="label">Narx darajalari</span>
                    </div>
                    <div class="header-stat">
                        <span class="number">$3.2M-$7.1M</span>
                        <span class="label">Yillik potentsial</span>
                    </div>
                </div>
            </div>

            <div class="section">
                <div class="info-box success">
                    <h4>📊 Portfel sharhi - Barcha 36 BOC toifalar</h4>
                    <p>Barcha 36 litsenziyalangan toifalar haqida to'liq ma'lumot hujjatning ingliz tilidagi versiyasida mavjud.</p>
                    <p><strong>Asosiy mahsulot guruhlari:</strong></p>
                    <ul>
                        <li><strong>Harakatchanlik uskunalari (M01-M09):</strong> $800K-$1.8M yillik daromad</li>
                        <li><strong>Uy DME (DM01-DM29):</strong> $1.2M-$2.5M yillik daromad</li>
                        <li><strong>Kompressiya va qo'llab-quvvatlash (S01-S04):</strong> $400K-$900K yillik daromad</li>
                        <li><strong>Ortopediya (OR01-OR04):</strong> $350K-$750K yillik daromad</li>
                        <li><strong>Protezlash (PR01-PR02):</strong> $200K-$500K yillik daromad</li>
                        <li><strong>Tibbiy buyumlar (SU01-SU03):</strong> $450K-$1.0M yillik daromad</li>
                    </ul>
                    <p><strong>Umumiy potentsial:</strong> $3.2M-$7.1M barcha 36 toifa bo'yicha yillik daromad</p>
                </div>
            </div>

            <div class="cta-section">
                <h2>📊 Ushbu mahsulotlarni joriy qilishga tayyormisiz?</h2>
                <div class="cta-buttons">
                    <a href="PRIMARY-LANDING-PAGE.html#all-strategies" class="cta-btn primary">
                        Barcha 11 strategiya →
                    </a>
                    <a href="complete-revenue-summary.html" class="cta-btn secondary">
                        Daromad prognozlari →
                    </a>
                </div>
            </div>

            <div class="footer">
                <p><strong>Holistic Medical Supply</strong> | To'liq DME mahsulot portfeli</p>
                <p>34 dan 3-hujjat | 25-oktabr 2025 | Versiya 1.0</p>
            </div>
        </div>
    </div>

    <script>
        function switchLanguage(lang) {
            document.querySelectorAll('.lang-content').forEach(content => {
                content.classList.remove('active');
            });
            document.querySelectorAll('.lang-btn').forEach(btn => {
                btn.classList.remove('active');
            });
            document.getElementById('content-' + lang).classList.add('active');
            document.querySelector('.lang-btn[data-lang="' + lang + '"]').classList.add('active');
            localStorage.setItem('preferredLanguage', lang);
        }

        window.addEventListener('DOMContentLoaded', function() {
            const savedLang = localStorage.getItem('preferredLanguage');
            if (savedLang && ['en', 'ru', 'uz'].includes(savedLang)) {
                switchLanguage(savedLang);
            }
        });
    </script>
</body>
</html>
