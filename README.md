<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Upadhyay Harvester | Agricultural Services</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family:Arial, Helvetica, sans-serif;
    line-height:1.6;
    color:#17221a;
    background:#f5f8f3;
}

/* NAVBAR */
header{
    position:sticky;
    top:0;
    z-index:1000;
    background:#123d20;
    color:white;
    box-shadow:0 3px 15px rgba(0,0,0,.18);
}

.navbar{
    max-width:1200px;
    margin:auto;
    padding:14px 20px;
    display:flex;
    align-items:center;
    justify-content:space-between;
}

.logo{
    font-size:22px;
    font-weight:800;
}

.logo span{
    color:#9ee36d;
}

nav a{
    color:white;
    text-decoration:none;
    margin-left:22px;
    font-weight:600;
}

nav a:hover{
    color:#9ee36d;
}

.menu{
    display:none;
    font-size:27px;
    cursor:pointer;
}

/* HERO */
.hero{
    min-height:78vh;
    display:flex;
    align-items:center;

    background:
    linear-gradient(
        rgba(0,30,10,.58),
        rgba(0,30,10,.62)
    ),
    url("images/harvester-day.jpg") center/cover;
}

.hero-content{
    max-width:1200px;
    width:100%;
    margin:auto;
    padding:70px 20px;
    color:white;
}

.hero h1{
    font-size:clamp(40px,7vw,72px);
    line-height:1.05;
    margin-bottom:18px;
}

.hero h1 span{
    color:#a7ef70;
}

.hero p{
    max-width:680px;
    font-size:20px;
    margin-bottom:28px;
}

.btn{
    display:inline-block;
    padding:13px 22px;
    border-radius:8px;
    text-decoration:none;
    font-weight:700;
    margin-right:10px;
    background:#9ee36d;
    color:#123d20;
}

.btn.dark{
    background:white;
    color:#123d20;
}

.btn:hover{
    transform:translateY(-2px);
}

/* COMMON SECTION */
section{
    padding:75px 20px;
}

.container{
    max-width:1200px;
    margin:auto;
}

.section-title{
    text-align:center;
    margin-bottom:42px;
}

.section-title h2{
    font-size:38px;
    color:#174d27;
}

.section-title p{
    color:#617066;
}

/* SERVICES */
.cards{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:22px;
}

.card{
    background:white;
    padding:28px;
    border-radius:15px;
    box-shadow:0 8px 25px rgba(0,0,0,.08);
    border:1px solid #e3ebe1;
}

.icon{
    font-size:40px;
    margin-bottom:12px;
}

.card h3{
    color:#174d27;
    margin-bottom:10px;
}

.card p{
    color:#59665c;
}

/* MACHINES */
.machines-section{
    background:#eef4eb;
}

.machine-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:24px;
}

.machine{
    background:white;
    border-radius:16px;
    overflow:hidden;
    box-shadow:0 8px 25px rgba(0,0,0,.1);
}

.machine img{
    width:100%;
    height:240px;
    object-fit:cover;
    display:block;
}

.machine-content{
    padding:20px;
}

.machine-content h3{
    color:#174d27;
    margin-bottom:8px;
}

/* AGRI WORK */
.work{
    background:#123d20;
    color:white;
}

.work .section-title h2{
    color:white;
}

.work-grid{
    display:grid;
    grid-template-columns:repeat(2,1fr);
    gap:20px;
}

.work-item{
    padding:24px;
    border:1px solid rgba(255,255,255,.15);
    background:rgba(255,255,255,.06);
    border-radius:14px;
}

.work-item h3{
    color:#a7ef70;
    margin-bottom:8px;
}

/* ABOUT */
.about-box{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:35px;
    align-items:center;
}

.about-box img{
    width:100%;
    height:390px;
    object-fit:cover;
    border-radius:18px;
    box-shadow:0 10px 30px rgba(0,0,0,.12);
}

.about-text h2{
    font-size:38px;
    color:#174d27;
    margin-bottom:15px;
}

.about-text p{
    margin-bottom:15px;
    color:#536056;
}

/* CONTACT */
.contact{
    background:#edf5e9;
}

.contact-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:28px;
}

.contact-box{
    background:white;
    padding:30px;
    border-radius:16px;
    box-shadow:0 8px 25px rgba(0,0,0,.07);
}

.contact-box h3{
    color:#174d27;
    margin-bottom:10px;
}

.contact-box a{
    color:#174d27;
    font-weight:800;
    text-decoration:none;
}

.contact-box p{
    margin:8px 0;
    color:#59665c;
}

/* FORM */
form{
    display:grid;
    gap:13px;
}

input,
textarea{
    width:100%;
    padding:13px;
    border:1px solid #ccd8ca;
    border-radius:8px;
    font:inherit;
}

textarea{
    min-height:120px;
    resize:vertical;
}

button{
    border:0;
    padding:14px;
    border-radius:8px;
    background:#174d27;
    color:white;
    font-weight:800;
    cursor:pointer;
    font-size:16px;
}

button:hover{
    background:#0e3319;
}

/* FOOTER */
footer{
    background:#0c2814;
    color:white;
    text-align:center;
    padding:25px 15px;
}

footer strong{
    color:#a7ef70;
}

/* MOBILE */
@media(max-width:800px){

    nav{
        display:none;
        position:absolute;
        top:61px;
        left:0;
        right:0;
        background:#123d20;
        padding:15px 20px;
    }

    nav.show{
        display:block;
    }

    nav a{
        display:block;
        margin:13px 0;
    }

    .menu{
        display:block;
    }

    .cards,
    .machine-grid,
    .work-grid,
    .about-box,
    .contact-grid{
        grid-template-columns:1fr;
    }

    .hero{
        min-height:70vh;
    }

    .hero p{
        font-size:17px;
    }

    section{
        padding:55px 16px;
    }
}
</style>
</head>

<body>

<!-- NAVBAR -->
<header>

<div class="navbar">

    <div class="logo">
        Upadhyay <span>Harvester</span>
    </div>

    <div class="menu" onclick="toggleMenu()">
        ☰
    </div>

    <nav id="nav">

        <a href="#home">Home</a>

        <a href="#services">Services</a>

        <a href="#machines">Machines</a>

        <a href="#work">Agri Work</a>

        <a href="#about">About</a>

        <a href="#contact">Contact</a>

    </nav>

</div>

</header>


<!-- HERO -->
<section class="hero" id="home">

<div class="hero-content">

    <h1>
        Modern Machines.<br>
        <span>Better Farming.</span>
    </h1>

    <p>
        Harvester aur agricultural machinery ke through
        farming work ke liye reliable service.
        Khet ka kaam, harvesting aur anya agricultural work
        ke liye humse contact karein.
    </p>

    <a class="btn" href="tel:+919580669349">
        📞 Kaam Ke Liye Contact Kare
    </a>

    <a class="btn dark" href="#machines">
        🚜 Machines Dekhein
    </a>

</div>

</section>


<!-- SERVICES -->
<section id="services">

<div class="container">

<div class="section-title">

    <h2>Hamari Services</h2>

    <p>
        Agricultural work ke liye machine aur field services.
    </p>

</div>


<div class="cards">

<div class="card">

    <div class="icon">🚜</div>

    <h3>Harvester Service</h3>

    <p>
        Harvesting aur crop-related machine work ke liye
        harvester service available.
        Kaam ke liye advance mein contact karein.
    </p>

</div>


<div class="card">

    <div class="icon">🌾</div>

    <h3>Agri Field Work</h3>

    <p>
        Kheti se jude field work aur machine-based
        agricultural kaam ke liye sampark karein.
    </p>

</div>


<div class="card">

    <div class="icon">🔧</div>

    <h3>Machinery Support</h3>

    <p>
        Agricultural machinery ke kaam aur basic support
        ke liye Upadhyay Harvester se contact karein.
    </p>

</div>

</div>

</div>

</section>


<!-- MACHINES -->
<section class="machines-section" id="machines">

<div class="container">

<div class="section-title">

    <h2>Hamari Machines</h2>

    <p>
        Agricultural machinery aur equipment.
    </p>

</div>


<div class="machine-grid">


<div class="machine">

    <img
        src="images/harvester-day.jpg"
        alt="Agricultural Harvester"
    >

    <div class="machine-content">

        <h3>Harvester Machine</h3>

        <p>
            Harvesting aur crop work ke liye
            agricultural harvester.
        </p>

    </div>

</div>


<div class="machine">

    <img
        src="images/harvester-night.jpg"
        alt="Agricultural Machinery"
    >

    <div class="machine-content">

        <h3>Field Machinery</h3>

        <p>
            Field work aur agricultural operations
            ke liye machinery.
        </p>

    </div>

</div>


<div class="machine">

    <img
        src="images/agri-machinery.jpg"
        alt="Agricultural Equipment"
    >

    <div class="machine-content">

        <h3>Agricultural Equipment</h3>

        <p>
            Anya farming aur agriculture-related
            machine work ke liye.
        </p>

    </div>

</div>


</div>

</div>

</section>


<!-- AGRICULTURAL WORK -->
<section class="work" id="work">

<div class="container">

<div class="section-title">

    <h2>Kaam Ke Liye Contact Karein</h2>

    <p>
        Apne agricultural work ke baare mein humein batayein.
    </p>

</div>


<div class="work-grid">


<div class="work-item">

    <h3>🌾 Harvesting Work</h3>

    <p>
        Fasal ki harvesting aur machine-based
        agricultural work ke liye contact karein.
    </p>

</div>


<div class="work-item">

    <h3>🚜 Harvester Booking</h3>

    <p>
        Harvester ya agricultural machine ki
        requirement ho to pehle contact karein.
    </p>

</div>


<div class="work-item">

    <h3>🌱 Other Agri Work</h3>

    <p>
        Koi anya agricultural machine work ho
        to apni requirement share karein.
    </p>

</div>


<div class="work-item">

    <h3>📍 Work Enquiry</h3>

    <p>
        Kaam ki location aur requirement batakar
        service ke baare mein enquiry karein.
    </p>

</div>


</div>


<div style="text-align:center;margin-top:35px">

    <a class="btn" href="tel:+919580669349">
        📞 9580669349 — Contact Now
    </a>

</div>

</div>

</section>


<!-- ABOUT -->
<section id="about">

<div class="container about-box">

    <img
        src="images/harvester-day.jpg"
        alt="Upadhyay Harvester Agricultural Work"
    >


    <div class="about-text">

        <h2>
            About Upadhyay Harvester
        </h2>

        <p>
            Upadhyay Harvester agricultural machinery
            aur farming work se related services ke liye
            banaya gaya hai.
        </p>

        <p>
            Hamara focus simple hai —
            agricultural work ke liye machine services
            ko customers tak easily pahunchana.
        </p>

        <p>
            Harvesting, harvester booking aur
            anya agricultural work ke liye
            humse contact karein.
        </p>

        <p>
            <strong>
                Made by Hemant Upadhyay
            </strong>
        </p>

    </div>

</div>

</section>


<!-- CONTACT -->
<section class="contact" id="contact">

<div class="container">

<div class="section-title">

    <h2>Contact & Enquiry</h2>

    <p>
        Kaam karwane ke liye call ya WhatsApp karein.
    </p>

</div>


<div class="contact-grid">


<!-- DIRECT CONTACT -->
<div class="contact-box">

    <h3>📞 Direct Contact</h3>

    <p>
        Harvester, agricultural work ya
        anya agri work ke liye:
    </p>

    <p>
        <a href="tel:+919580669349">
            9580669349
        </a>
    </p>

    <br>

    <a
        class="btn"
        href="https://wa.me/919580669349?text=Namaste%2C%20mujhe%20agricultural%20work%20ke%20liye%20jankari%20chahiye."
        target="_blank"
    >
        WhatsApp Kare
    </a>

</div>


<!-- ENQUIRY FORM -->
<div class="contact-box">

    <h3>📝 Work Enquiry</h3>

    <form id="enquiryForm">

        <input
            id="name"
            type="text"
            placeholder="Aapka naam"
            required
        >

        <input
            id="location"
            type="text"
            placeholder="Work location"
            required
        >

        <textarea
            id="message"
            placeholder="Kaunsa agricultural work karwana hai?"
            required
        ></textarea>

        <button type="submit">
            WhatsApp Par Enquiry Bhejein
        </button>

    </form>

</div>


</div>

</div>

</section>


<!-- FOOTER -->
<footer>

    <p>
        <strong>
            Upadhyay Harvester
        </strong>
    </p>

    <p>
        Agricultural Machinery & Farming Work Services
    </p>

    <p>
        Made by Hemant Upadhyay |
        Contact: 9580669349
    </p>

</footer>


<!-- JAVASCRIPT -->
<script>

function toggleMenu(){

    document
        .getElementById("nav")
        .classList
        .toggle("show");

}


document
    .querySelectorAll("#nav a")
    .forEach(function(link){

        link.addEventListener("click", function(){

            document
                .getElementById("nav")
                .classList
                .remove("show");

        });

    });


document
    .getElementById("enquiryForm")
    .addEventListener("submit", function(e){

        e.preventDefault();

        const name =
            document.getElementById("name").value;

        const location =
            document.getElementById("location").value;

        const message =
            document.getElementById("message").value;


        const text =
            "Namaste, Upadhyay Harvester.%0A%0A" +

            "Name: " +
            encodeURIComponent(name) +
            "%0A" +

            "Work Location: " +
            encodeURIComponent(location) +
            "%0A" +

            "Agricultural Work: " +
            encodeURIComponent(message);


        window.open(
            "https://wa.me/919580669349?text=" +
            text,
            "_blank"
        );

    });

</script>

</body>
</html>
