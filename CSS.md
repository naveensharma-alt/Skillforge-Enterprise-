*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}


html{
    scroll-behavior:smooth;
}


body{

    font-family:'Inter',sans-serif;
    color:#172033;
    background:#ffffff;
    line-height:1.6;

}


.container{

    width:90%;
    max-width:1200px;
    margin:auto;

}


/* =====================
NAVBAR
===================== */


.navbar{

    position:sticky;
    top:0;
    z-index:1000;
    background:white;
    box-shadow:0 5px 20px rgba(0,0,0,0.06);

}


.nav-container{

    display:flex;
    align-items:center;
    justify-content:space-between;
    height:80px;

}


.logo{

    font-size:28px;
    font-weight:800;
    color:#101828;

}


.logo span{

    color:#2563eb;

}


nav{

    display:flex;
    gap:35px;

}


nav a{

    text-decoration:none;
    color:#475467;
    font-weight:500;
    transition:.3s;

}


nav a:hover{

    color:#2563eb;

}


.menu{

    display:none;

}



/* =====================
BUTTONS
===================== */


.btn{

    padding:14px 28px;
    border-radius:10px;
    border:none;
    cursor:pointer;
    font-size:15px;
    font-weight:600;
    transition:.3s;

}


.primary{

    background:#2563eb;
    color:white;

}


.primary:hover{

    background:#1d4ed8;
    transform:translateY(-2px);

}


.outline{

    background:white;
    color:#2563eb;
    border:2px solid #2563eb;

}


.outline:hover{

    background:#eff6ff;

}



/* =====================
HERO
===================== */


.hero{

    padding:100px 0;
    background:
    linear-gradient(135deg,#eff6ff,#ffffff);

}



.hero-grid{

    display:grid;
    grid-template-columns:1fr 1fr;
    align-items:center;
    gap:60px;

}



.hero-content h1{

    font-size:55px;
    line-height:1.15;
    font-weight:800;
    margin-bottom:25px;

}



.hero-content p{

    font-size:18px;
    color:#667085;
    max-width:550px;
    margin-bottom:35px;

}



.hero-buttons{

    display:flex;
    gap:20px;

}





/* HERO CARD */


.hero-card{

    position:relative;

}



.main-dashboard{

    background:white;
    padding:40px;
    border-radius:25px;
    box-shadow:
    0 20px 50px rgba(0,0,0,.12);

}



.main-dashboard h3{

    margin-top:25px;
    font-size:22px;

}



.main-dashboard p{

    color:#667085;

}




.chart{

    height:180px;
    display:flex;
    align-items:flex-end;
    gap:15px;

}



.chart div{

    width:40px;
    background:#2563eb;
    border-radius:8px;

}


.chart div:nth-child(1){

    height:50%;

}


.chart div:nth-child(2){

    height:80%;

}


.chart div:nth-child(3){

    height:60%;

}


.chart div:nth-child(4){

    height:95%;

}




.floating-card{

    position:absolute;
    top:-25px;
    right:-20px;

    background:white;
    padding:20px;
    border-radius:15px;

    box-shadow:0 10px 30px rgba(0,0,0,.1);

}



.floating-card i{

    color:#2563eb;

}


.floating-card h3{

    font-size:25px;

}






/* =====================
TRUST SECTION
===================== */


.trusted{

    padding:50px 0;
    text-align:center;

}



.trusted h3{

    color:#667085;
    margin-bottom:35px;

}



.company-list{

    display:flex;
    justify-content:space-around;
    flex-wrap:wrap;
    gap:25px;

}



.company-list div{

    font-size:22px;
    font-weight:700;
    color:#344054;

}





/* =====================
STATS
===================== */


.stats{

    background:#2563eb;
    padding:70px 0;
    color:white;

}



.stats-grid{

    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:30px;

}



.stat-box{

    text-align:center;

}



.stat-box h2{

    font-size:45px;

}



.stat-box p{

    opacity:.9;

}






/* =====================
SECTION TITLES
===================== */


.section-title{

    text-align:center;
    margin-bottom:50px;

}



.section-title h2{

    font-size:38px;
    margin-bottom:10px;

}



.section-title p{

    color:#667085;

}






/* =====================
SOLUTIONS
===================== */


.solutions{

    padding:100px 0;

}



.cards{

    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:25px;

}



.card{

    padding:35px;
    border-radius:20px;
    background:white;

    box-shadow:
    0 10px 30px rgba(0,0,0,.08);

    transition:.3s;

}



.card:hover{

    transform:translateY(-10px);

}



.card i{

    color:#2563eb;
    width:40px;

}



.card h3{

    margin:20px 0 10px;

}



.card p{

    color:#667085;

}




/* =====================
PROGRAMS
===================== */


.programs{

    background:#f8fafc;
    padding:100px 0;

}



.program-grid{

    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:30px;

}



.program{

    background:white;
    padding:35px;
    border-radius:20px;

}



.program h3{

    margin-bottom:15px;

}



.program p{

    color:#667085;
    margin-bottom:20px;

}



.program a{

    color:#2563eb;
    text-decoration:none;
    font-weight:600;

}

/* =====================
ABOUT SECTION
===================== */


.about{

    padding:100px 0;

}



.about-grid{

    display:grid;
    grid-template-columns:1fr 1fr;
    gap:60px;
    align-items:center;

}



.about h2{

    font-size:40px;
    margin-bottom:20px;

}



.about p{

    color:#667085;
    margin-bottom:25px;

}



.about ul{

    list-style:none;

}



.about li{

    margin:15px 0;
    font-size:17px;
    color:#344054;

}




.about-box{

    background:
    linear-gradient(135deg,#2563eb,#1e40af);

    color:white;

    padding:50px;

    border-radius:25px;

    text-align:center;

}



.about-box h3{

    font-size:28px;
    margin-bottom:30px;

}



.progress{

    height:18px;
    background:rgba(255,255,255,.3);
    border-radius:20px;
    overflow:hidden;
    margin-bottom:20px;

}



.progress span{

    display:block;
    width:85%;
    height:100%;
    background:white;
    border-radius:20px;

}

.main-dashboard img,
.about-image img,
.office img{

    width:100%;
    height:auto;
    border-radius:20px;
    object-fit:cover;

}






/* =====================
TESTIMONIALS
===================== */


.testimonial{

    padding:100px 0;
    background:#f8fafc;
    text-align:center;

}



.testimonial h2{

    font-size:38px;
    margin-bottom:40px;

}



.testimonial-box{

    max-width:700px;
    margin:auto;

    background:white;

    padding:50px;

    border-radius:20px;

    box-shadow:
    0 15px 40px rgba(0,0,0,.08);

}



.testimonial-box p{

    font-size:22px;
    font-style:italic;
    color:#344054;
    margin-bottom:25px;

}



.testimonial-box h4{

    color:#2563eb;

}






/* =====================
FAQ
===================== */


.faq{

    padding:100px 0;

}



.faq h2{

    text-align:center;
    font-size:38px;
    margin-bottom:50px;

}



.faq-item{

    max-width:800px;
    margin:20px auto;

    border:1px solid #e4e7ec;

    border-radius:12px;

    overflow:hidden;

}



.faq-item button{

    width:100%;

    padding:20px;

    background:white;

    border:none;

    display:flex;

    justify-content:space-between;

    cursor:pointer;

    font-size:17px;

    font-weight:600;

}



.faq-item p{

    padding:0 20px 20px;

    color:#667085;

    display:none;

}



.faq-item.active p{

    display:block;

}






/* =====================
CONTACT
===================== */


.contact{

    padding:100px 0;

    background:
    linear-gradient(135deg,#eff6ff,#ffffff);

}



.contact-box{

    max-width:800px;

    text-align:center;

}



.contact-box h2{

    font-size:40px;

    margin-bottom:15px;

}



.contact-box p{

    color:#667085;

    margin-bottom:35px;

}



form{

    display:grid;
    gap:18px;

}



input,
textarea{

    width:100%;

    padding:16px;

    border:1px solid #d0d5dd;

    border-radius:10px;

    font-size:15px;

    font-family:inherit;

}



textarea{

    min-height:120px;

    resize:none;

}





form button{

    justify-self:center;

}







/* =====================
FOOTER
===================== */


footer{

    background:#101828;

    color:white;

    padding:70px 0;

}



.footer-grid{

    display:grid;

    grid-template-columns:2fr 1fr 1fr;

    gap:40px;

}



footer h2{

    font-size:30px;

    margin-bottom:15px;

}



footer h4{

    margin-bottom:20px;

}



footer p{

    color:#98a2b3;

}



footer a{

    display:block;

    color:#d0d5dd;

    text-decoration:none;

    margin-bottom:12px;

}



footer a:hover{

    color:white;

}








/* =====================
SCROLL ANIMATION
===================== */


.card,
.program,
.stat-box,
.about-box,
.testimonial-box{

    animation:fadeUp .8s ease;

}



@keyframes fadeUp{

    from{

        opacity:0;

        transform:translateY(30px);

    }


    to{

        opacity:1;

        transform:translateY(0);

    }

}






/* =====================
TABLET RESPONSIVE
===================== */


@media(max-width:1000px){


.hero-grid,
.about-grid{

    grid-template-columns:1fr;

}



.hero-content h1{

    font-size:42px;

}



.cards{

    grid-template-columns:repeat(2,1fr);

}



.program-grid{

    grid-template-columns:1fr;

}



.stats-grid{

    grid-template-columns:repeat(2,1fr);

}



.footer-grid{

    grid-template-columns:1fr;

}



.hero-card{

    margin-top:40px;

}


}







/* =====================
MOBILE RESPONSIVE
===================== */


@media(max-width:700px){


.nav-container{

    height:70px;

}



nav{

    display:none;

}



.menu{

    display:block;

}



.navbar .btn{

    display:none;

}



.hero{

    padding:70px 0;

}



.hero-content h1{

    font-size:34px;

}



.hero-buttons{

    flex-direction:column;

}



.floating-card{

    display:none;

}



.cards{

    grid-template-columns:1fr;

}



.stats-grid{

    grid-template-columns:1fr;

}



.section-title h2,
.about h2,
.contact-box h2,
.faq h2{

    font-size:30px;

}



.company-list{

    flex-direction:column;

}



.main-dashboard{

    padding:25px;

}



}
