/* ==============================
   PERSONAL PORTFOLIO - STYLE
   ============================== */

/* Basic reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    line-height: 1.6;
    color: #172033;
    background: #ffffff;
}

/* Navigation */
header {
    position: sticky;
    top: 0;
    z-index: 1000;
    background: rgba(255, 255, 255, 0.96);
    border-bottom: 1px solid #e7eaf0;
}

.navbar {
    max-width: 1100px;
    margin: auto;
    padding: 18px 24px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.logo {
    font-size: 24px;
    font-weight: 800;
    letter-spacing: -1px;
}

.logo span {
    color: #5b4bdb;
}

.nav-links {
    display: flex;
    list-style: none;
    gap: 24px;
}

.nav-links a {
    color: #172033;
    text-decoration: none;
    font-size: 14px;
    font-weight: 600;
}

.nav-links a:hover {
    color: #5b4bdb;
}

/* Hero */
.hero {
    max-width: 1100px;
    min-height: 680px;
    margin: auto;
    padding: 90px 24px;
    display: grid;
    grid-template-columns: 1.4fr 0.8fr;
    align-items: center;
    gap: 60px;
}

.hello,
.section-label {
    color: #5b4bdb;
    font-size: 13px;
    font-weight: 800;
    letter-spacing: 2px;
}

.hero h1 {
    margin-top: 8px;
    font-size: clamp(52px, 8vw, 86px);
    line-height: 1;
    letter-spacing: -4px;
}

.hero h2 {
    margin-top: 18px;
    font-size: clamp(22px, 3vw, 32px);
    color: #424b60;
}

.intro {
    max-width: 650px;
    margin-top: 20px;
    color: #667085;
    font-size: 17px;
}

.hero-buttons {
    margin-top: 32px;
    display: flex;
    gap: 14px;
    flex-wrap: wrap;
}

.btn {
    display: inline-block;
    padding: 13px 22px;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 700;
    transition: 0.2s;
}

.btn:hover {
    transform: translateY(-2px);
}

.primary {
    color: white;
    background: #5b4bdb;
}

.secondary {
    color: #5b4bdb;
    border: 1px solid #5b4bdb;
}

.hero-card {
    padding: 45px 30px;
    text-align: center;
    border-radius: 24px;
    background: #f1f0ff;
    border: 1px solid #dedbff;
}

.profile-circle {
    width: 150px;
    height: 150px;
    margin: 0 auto 24px;
    display: grid;
    place-items: center;
    border-radius: 50%;
    color: white;
    background: #5b4bdb;
    font-size: 70px;
    font-weight: 800;
}

.hero-card h3 {
    font-size: 22px;
}

.hero-card p {
    color: #667085;
    margin-top: 5px;
}

/* Sections */
.section {
    max-width: 1100px;
    margin: auto;
    padding: 90px 24px;
}

.section h2 {
    margin-top: 6px;
    margin-bottom: 35px;
    font-size: 40px;
    letter-spacing: -1px;
}

.alt-section {
    max-width: none;
    padding-left: max(24px, calc((100% - 1100px) / 2));
    padding-right: max(24px, calc((100% - 1100px) / 2));
    background: #f7f7fb;
}

.about-content {
    display: grid;
    grid-template-columns: 1.4fr 1fr;
    gap: 50px;
}

.about-content p {
    margin-bottom: 18px;
    color: #596275;
    font-size: 16px;
}

.info-box {
    padding: 25px;
    border-left: 4px solid #5b4bdb;
    background: #f7f7fb;
}

.info-box p {
    margin-bottom: 10px;
}

/* Skills */
.cards {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 18px;
}

.card {
    padding: 28px;
    background: white;
    border: 1px solid #e5e7eb;
    border-radius: 14px;
}

.card:hover,
.project-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 12px 30px rgba(20, 25, 40, 0.08);
}

.card,
.project-card {
    transition: 0.2s;
}

.icon {
    width: 50px;
    height: 50px;
    margin-bottom: 18px;
    display: grid;
    place-items: center;
    border-radius: 12px;
    color: #5b4bdb;
    background: #f1f0ff;
    font-weight: 800;
}

.card h3 {
    margin-bottom: 8px;
}

.card p {
    color: #667085;
    font-size: 14px;
}

/* Projects */
.project-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
}

.project-card {
    padding: 30px;
    border: 1px solid #e5e7eb;
    border-radius: 16px;
}

.project-number {
    color: #5b4bdb;
    font-weight: 800;
}

.project-card h3 {
    margin: 12px 0;
}

.project-card p {
    color: #667085;
    font-size: 15px;
    margin-bottom: 20px;
}

.tag {
    display: inline-block;
    padding: 5px 10px;
    border-radius: 20px;
    color: #5b4bdb;
    background: #f1f0ff;
    font-size: 12px;
    font-weight: 700;
}

/* Education */
.timeline {
    border-left: 2px solid #d9d7f5;
    padding-left: 30px;
}

.timeline-item {
    position: relative;
    max-width: 700px;
}

.dot {
    position: absolute;
    left: -39px;
    top: 4px;
    width: 16px;
    height: 16px;
    border-radius: 50%;
    background: #5b4bdb;
}

.date {
    color: #5b4bdb;
    font-size: 12px;
    font-weight: 800;
    letter-spacing: 1px;
}

.timeline-item h3 {
    margin: 8px 0;
    font-size: 23px;
}

.timeline-item p {
    color: #667085;
    margin-bottom: 6px;
}

/* Contact */
.contact-section {
    text-align: center;
}

.contact-section > p:not(.section-label) {
    max-width: 600px;
    margin: 0 auto 25px;
    color: #667085;
}

.contact-links {
    display: flex;
    justify-content: center;
    gap: 14px;
    flex-wrap: wrap;
}

.contact-links a {
    padding: 11px 20px;
    color: #5b4bdb;
    text-decoration: none;
    border: 1px solid #5b4bdb;
    border-radius: 8px;
    font-weight: 700;
}

.contact-links a:hover {
    color: white;
    background: #5b4bdb;
}

/* Footer */
footer {
    padding: 30px 24px;
    text-align: center;
    color: #7b8496;
    background: #172033;
    font-size: 13px;
}

footer p + p {
    margin-top: 5px;
}

/* Mobile responsive design */
@media (max-width: 800px) {
    .nav-links {
        display: none;
    }

    .hero {
        grid-template-columns: 1fr;
        padding-top: 60px;
    }

    .hero-card {
        max-width: 420px;
        width: 100%;
        margin: auto;
    }

    .about-content,
    .project-grid {
        grid-template-columns: 1fr;
    }

    .cards {
        grid-template-columns: repeat(2, 1fr);
    }

    .section h2 {
        font-size: 32px;
    }
}

@media (max-width: 480px) {
    .hero h1 {
        font-size: 55px;
    }

    .cards {
        grid-template-columns: 1fr;
    }

    .section {
        padding-top: 65px;
        padding-bottom: 65px;
    }
}
