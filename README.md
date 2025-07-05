<!DOCTYPE html>
<html lang="he" dir="rtl">
<head>
    <meta charset="UTF-8">
    <title>הפורטפוליו של ארטם</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <style>
        body {
            font-family: "Arial", sans-serif;
            margin: 0;
            background: #f4f4f4;
            direction: rtl;
        }
        header {
            background: #2b3a55;
            color: #fff;
            padding: 32px 0 16px 0;
            text-align: center;
        }
        nav {
            margin: 0 0 24px 0;
        }
        nav a {
            color: #fff;
            text-decoration: none;
            margin: 0 12px;
            font-size: 1.1em;
            transition: border-bottom 0.2s;
            border-bottom: 2px solid transparent;
            padding-bottom: 2px;
        }
        nav a:hover {
            border-bottom: 2px solid #eee;
        }
        section {
            max-width: 800px;
            margin: 32px auto;
            background: #fff;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.08);
            padding: 32px 24px;
        }
        h2 {
            color: #38598b;
            margin-top: 0;
        }
        .projects {
            display: flex;
            flex-wrap: wrap;
            gap: 24px;
        }
        .project-card {
            background: #e8eaf6;
            border-radius: 8px;
            flex: 1 1 240px;
            min-width: 220px;
            box-shadow: 0 1px 4px rgba(56,89,139,0.07);
            padding: 16px;
        }
        .project-card h3 {
            margin-top: 0;
            font-size: 1.2em;
        }
        .skills {
            margin-top: 24px;
        }
        .skill {
            margin-bottom: 18px;
        }
        .skill-title {
            display: flex;
            justify-content: space-between;
            font-size: 1.05em;
            margin-bottom: 2px;
        }
        .progress-bar-bg {
            background: #e0e0e0;
            border-radius: 12px;
            height: 22px;
            width: 100%;
            overflow: hidden;
        }
        .progress-bar {
            height: 100%;
            border-radius: 12px 0 0 12px;
            background: linear-gradient(90deg, #38598b 60%, #73a5c6 100%);
            text-align: left;
            color: #fff;
            font-weight: bold;
            line-height: 22px;
            padding-right: 10px;
            transition: width 1s;
        }
        /* Simple Pie Chart */
        .charts {
            display: flex;
            gap: 38px;
            margin-top: 32px;
            flex-wrap: wrap;
            justify-content: center;
        }
        .pie-chart {
            width: 110px;
            height: 110px;
            border-radius: 50%;
            background: conic-gradient(
                #38598b 0 70%, /* 70% - JS */
                #e0e0e0 0 100%
            );
            position: relative;
            margin: 0 auto 8px auto;
        }
        .pie-label {
            position: absolute;
            width: 100%;
            top: 42%;
            text-align: center;
            font-weight: bold;
            color: #38598b;
            font-size: 1.1em;
        }
        .pie-chart.react {
            background: conic-gradient(
                #3898b4 0 60%, /* 60% - React */
                #e0e0e0 0 100%
            );
        }
        .pie-chart.css {
            background: conic-gradient(
                #73a5c6 0 85%, /* 85% - CSS */
                #e0e0e0 0 100%
            );
        }
        .pie-chart.html {
            background: conic-gradient(
                #f4b400 0 95%, /* 95% - HTML */
                #e0e0e0 0 100%
            );
        }
        .charts-title {
            text-align: center;
            color: #38598b;
            font-size: 1.1em;
            margin-bottom: 10px;
        }
        .contact-form label {
            display: block;
            margin: 12px 0 4px;
        }
        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 8px;
            margin-bottom: 16px;
            border-radius: 4px;
            border: 1px solid #bbb;
            font-size: 1em;
        }
        .contact-form button {
            background: #38598b;
            color: #fff;
            border: none;
            padding: 10px 22px;
            border-radius: 4px;
            font-size: 1em;
            cursor: pointer;
        }
        .contact-form button:hover {
            background: #2b3a55;
        }
        @media (max-width: 600px) {
            section {
                padding: 16px 6px;
            }
            .projects {
                flex-direction: column;
            }
            .charts {
                flex-direction: column;
                gap: 16px;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>הפורטפוליו של ארטם</h1>
        <nav>
            <a href="#welcome">ברוך הבא</a>
            <a href="#about">קצת עליי</a>
            <a href="#skills">מיומנויות</a>
            <a href="#projects">פרויקטים</a>
            <a href="#contact">צור קשר</a>
        </nav>
    </header>
    <section id="welcome">
        <h2>ברוך הבא!</h2>
        <p>ברוכים הבאים לפורטפוליו שלי. כאן תמצאו מידע עליי, עבודות שביצעתי ודרכי יצירת קשר.</p>
    </section>
    <section id="about">
        <h2>קצת עליי</h2>
        <p>שמי ארטם, מפתח ווב בעל ניסיון בתכנות, עיצוב אתרים ויצירת פתרונות יצירתיים. אני אוהב ללמוד טכנולוגיות חדשות ולשלב עיצוב מודרני עם קוד איכותי.</p>
    </section>
    <!-- New Skills Section with Visualizations -->
    <section id="skills">
        <h2>מיומנויות</h2>
        <div class="skills">
            <div class="skill">
                <div class="skill-title">
                    <span>JavaScript</span>
                    <span>70%</span>
                </div>
                <div class="progress-bar-bg">
                    <div class="progress-bar" style="width: 70%;">&nbsp;</div>
                </div>
            </div>
            <div class="skill">
                <div class="skill-title">
                    <span>React</span>
                    <span>60%</span>
                </div>
                <div class="progress-bar-bg">
                    <div class="progress-bar" style="width: 60%;background:linear-gradient(90deg,#3898b4 60%,#b4e1fa 100%);">&nbsp;</div>
                </div>
            </div>
            <div class="skill">
                <div class="skill-title">
                    <span>CSS</span>
                    <span>85%</span>
                </div>
                <div class="progress-bar-bg">
                    <div class="progress-bar" style="width: 85%;background:linear-gradient(90deg,#73a5c6 60%,#e7f3fa 100%);">&nbsp;</div>
                </div>
            </div>
            <div class="skill">
                <div class="skill-title">
                    <span>HTML</span>
                    <span>95%</span>
                </div>
                <div class="progress-bar-bg">
                    <div class="progress-bar" style="width: 95%;background:linear-gradient(90deg,#f4b400 60%,#fffbe7 100%);">&nbsp;</div>
                </div>
            </div>
        </div>
        <div class="charts-title">התפלגות מיומנויות (דיאגרמות עוגה)</div>
        <div class="charts">
            <div style="position:relative;">
                <div class="pie-chart">
                    <span class="pie-label">JS<br>70%</span>
                </div>
                <div style="text-align:center;">JavaScript</div>
            </div>
            <div style="position:relative;">
                <div class="pie-chart react">
                    <span class="pie-label">React<br>60%</span>
                </div>
                <div style="text-align:center;">React</div>
            </div>
            <div style="position:relative;">
                <div class="pie-chart css">
                    <span class="pie-label">CSS<br>85%</span>
                </div>
                <div style="text-align:center;">CSS</div>
            </div>
            <div style="position:relative;">
                <div class="pie-chart html">
                    <span class="pie-label">HTML<br>95%</span>
                </div>
                <div style="text-align:center;">HTML</div>
            </div>
        </div>
    </section>
    <section id="projects">
        <h2>פרויקטים</h2>
        <div class="projects">
            <div class="project-card">
                <h3>אתר תדמית לעסק</h3>
                <p>בניית אתר תדמית מודרני לעסקים, כולל עיצוב רספונסיבי ומערכת ניהול.</p>
            </div>
            <div class="project-card">
                <h3>מערכת ניהול לקוחות</h3>
                <p>פיתוח מערכת CRM לניהול לקוחות, מעקב אחרי פניות ודוחות מתקדמים.</p>
            </div>
            <div class="project-card">
                <h3>אפליקציית משימות</h3>
                <p>אפליקציה לניהול משימות יומיומיות עם ממשק ידידותי למשתמש.</p>
            </div>
        </div>
    </section>
    <section id="contact">
        <h2>צור קשר</h2>
        <form class="contact-form">
            <label for="name">שם:</label>
            <input type="text" id="name" name="name" required>
            <label for="email">אימייל:</label>
            <input type="email" id="email" name="email" required>
            <label for="message">הודעה:</label>
            <textarea id="message" name="message" rows="4" required></textarea>
            <button type="submit">שלח</button>
        </form>
    </section>
</body>
</html>
