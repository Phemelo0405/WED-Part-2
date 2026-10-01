/* =========================
   GENERAL STYLING
========================= */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    background-color: #fff8f5;
    color: #333;
}

/* =========================
   HEADER
========================= */

header {
    background-color: #8b4a5a;
    color: white;
    padding: 20px;
    text-align: center;
    position: sticky;
    top: 0;
    z-index: 1000;
}

header h1 {
    margin-bottom: 15px;
    font-size: 32px;
}

/* =========================
   NAVIGATION
========================= */

nav ul {
    list-style: none;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 10px;
}

nav ul li {
    display: inline-block;
}

nav ul li a {
    color: white;
    text-decoration: none;
    padding: 10px 15px;
    display: block;
    border-radius: 5px;
}

nav ul li a:hover {
    background-color: #663442;
}

/* =========================
   GENERAL SECTIONS
========================= */

section {
    padding: 70px 8%;
    text-align: center;
}

section h2 {
    font-size: 32px;
    color: #8b4a5a;
    margin-bottom: 20px;
}

section p {
    max-width: 800px;
    margin: 10px auto;
}

/* =========================
   HOME
========================= */

#home {
    min-height: 500px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    background-image: linear-gradient(
        rgba(0, 0, 0, 0.45),
        rgba(0, 0, 0, 0.45)
    ),
    url("../IMAGES/pexels-brent-keane-181485-1702373.jpg");

    background-size: cover;
    background-position: center;
    background-attachment: fixed;

    color: white;
}

#home h1 {
    font-size: 45px;
    margin-bottom: 20px;
}

#home p {
    font-size: 18px;
    margin-bottom: 25px;
}

#home a {
    background-color: #8b4a5a;
    color: white;
    text-decoration: none;
    padding: 12px 25px;
    border-radius: 5px;
    font-weight: bold;
}

#home a:hover {
    background-color: #663442;
}

/* =========================
   ABOUT
========================= */

#about {
    color: white;

    background-image: linear-gradient(
        rgba(0, 0, 0, 0.55),
        rgba(0, 0, 0, 0.55)
    ),
    url("../IMAGES/OIP (5).webp");

    background-size: cover;
    background-position: center;
    background-attachment: fixed;
}

#about h2 {
    color: white;
}

/* =========================
   CAKES
========================= */

#cakes {
    background-color: #fff8f5;
}

#cakes article {
    display: inline-block;
    vertical-align: top;
    width: 30%;
    min-width: 250px;
    margin: 15px;
    padding: 20px;

    background-color: white;
    border-radius: 10px;

    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);

    transition: transform 0.3s ease;
}

#cakes article:hover {
    transform: translateY(-8px);
}

#cakes article img {
    width: 100%;
    height: 220px;
    object-fit: cover;
    border-radius: 8px;
}

#cakes article h3 {
    color: #8b4a5a;
    margin: 15px 0 10px;
}

#cakes article strong {
    color: #8b4a5a;
    font-size: 18px;
}

/* =========================
   SPECIAL OFFERS
========================= */

#offers {
    color: white;

    background-image: linear-gradient(
        rgba(0, 0, 0, 0.55),
        rgba(0, 0, 0, 0.55)
    ),
    url("../IMAGES/OIP (3).webp");

    background-size: cover;
    background-position: center;
    background-attachment: fixed;
}

#offers h2 {
    color: white;
}

.offers-container {
    display: flex;
    justify-content: center;
    gap: 25px;
    flex-wrap: wrap;
    margin-top: 30px;
}

.offer-card {
    background-color: white;
    color: #333;
    width: 300px;
    padding: 30px 20px;
    border-radius: 10px;

    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
}

.offer-icon {
    font-size: 45px;
    margin-bottom: 15px;
}

.offer-card h3 {
    color: #8b4a5a;
    margin-bottom: 15px;
}

.offer-price {
    color: #8b4a5a;
    font-size: 20px;
    font-weight: bold;
}

/* =========================
   ORDER FORM
========================= */

#order {
    background-color: #f8e8eb;
}

form {
    max-width: 600px;
    margin: 30px auto;
    padding: 30px;

    background-color: white;
    border-radius: 10px;

    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);

    text-align: left;
}

form label {
    font-weight: bold;
    color: #8b4a5a;
}

form input,
form select,
form textarea {
    width: 100%;
    padding: 12px;
    margin-top: 8px;

    border: 1px solid #ccc;
    border-radius: 5px;

    font-family: Arial, sans-serif;
    font-size: 15px;
}

form textarea {
    height: 120px;
    resize: vertical;
}

form button {
    width: 100%;
    padding: 13px;

    background-color: #8b4a5a;
    color: white;

    border: none;
    border-radius: 5px;

    font-size: 16px;
    font-weight: bold;
    cursor: pointer;
}

form button:hover {
    background-color: #663442;
}

/* =========================
   CONTACT
========================= */

#contact {
    background-color: #fff8f5;
}

#contact h3 {
    color: #8b4a5a;
    margin-top: 25px;
}

/* =========================
   FOOTER
========================= */

footer {
    background-color: #8b4a5a;
    color: white;
    text-align: center;
    padding: 25px;
}

footer p {
    margin: 5px;
}

/* =========================
   MOBILE RESPONSIVENESS
========================= */

@media (max-width: 768px) {

    header h1 {
        font-size: 26px;
    }

    nav ul {
        flex-direction: column;
        align-items: center;
    }

    #home h1 {
        font-size: 32px;
    }

    section {
        padding: 50px 5%;
    }

    #cakes article {
        width: 90%;
        margin: 15px auto;
    }

    .offer-card {
        width: 90%;
    }

    form {
        width: 95%;
    }
}
