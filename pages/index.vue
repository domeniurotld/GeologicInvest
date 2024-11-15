<template>
    <div>
        <div class="section-content" style="padding-top: 2.5rem;">
            <div class="text-content">
                <h1 class="page-title">Bun venit la Geologic Invest!</h1>
                <p class="simple-text">
                    Geologic Invest, înființată în 2018, este lider în oferirea de servicii geotehnice și geologice. Cu o echipă de experți dedicați și echipamente de ultimă generație, ne asigurăm că proiectele dumneavoastră beneficiază de suportul tehnic necesar pentru succes. Fie că aveți nevoie de documentații geotehnice, verificări AF, foraje sau determinări de laborator, suntem aici pentru a vă oferi soluțiile de care aveți nevoie.
                </p>
                <div class="contact-button">
                    <a href="tel:+40744837601">
                        <button class="top-section-button"> 
                            <Icon name="material-symbols:call" size="1.7rem" style="margin-right: 0.7rem;" /> 
                            <span>Contactați-ne</span>
                        </button>
                    </a>
                </div>
            </div>
            <div class="image-container" style="display:flex; justify-content: right;">
                <img src="/assets/images/first-image.jpg" alt="Worker">
            </div>
        </div>
        <hr>
        <div id="aboutus" class="section-content">
            <div class="image-container">
                <img src="/assets/images/second-image.jpg" alt="Worker">
            </div>
            <div class="text-content">
                <h1 class="page-title">Despre noi</h1>
                <p class="simple-text">
                    Geologic Invest a fost fondată în 2018 cu misiunea de a furniza servicii geotehnice și geologice de înaltă calitate. De atunci, ne-am dedicat să oferim clienților noștri soluții precise și eficiente pentru toate tipurile de sol, de la soluri necoezive și coezive până la roci. Echipa noastră este formată din profesioniști cu experiență vastă în domeniu, care se angajează să răspundă celor mai exigente cerințe tehnice și să livreze rezultate excepționale.
                </p>
            </div>
        </div>
        <hr>
        <div id="services" class="section-content">
            <div class="text-content">
                <h1 class="page-title">Servicii</h1>
                <p class="simple-text">
                    <b>1. Documentații geotehnice:</b>
                </p>
                <p class="simple-text" style="margin-left: 1rem;">
                    • Elaborăm documentații geotehnice complete și detaliate, esențiale pentru succesul proiectelor de construcție și infrastructură.
                </p>
                <p class="simple-text">
                    <b>2. Verificări AF:</b>
                </p>
                <p class="simple-text" style="margin-left: 1rem;">
                    • Oferim servicii de verificare a adecvării fundațiilor (AF), asigurând stabilitatea și siguranța construcțiilor dumneavoastră.
                </p>
                <p class="simple-text">
                    <b>3. Execuția de foraje geologice și geotehnice:</b>
                </p>
                <p class="simple-text" style="margin-left: 1rem;">
                    • Realizăm foraje în toate tipurile de sol, de la soluri necoezive și coezive până la roci, folosind echipamente moderne pentru a obține date precise și fiabile.
                </p>
                <p class="simple-text">
                    <b>4. Determinări de laborator:</b>
                </p>
                <p class="simple-text" style="margin-left: 1rem;">
                    • Efectuăm determinări de laborator pentru a evalua caracteristicile fizice și mecanice ale solurilor și rocilor, oferind informații esențiale pentru proiectarea fundațiilor și structurilor.
                </p>
            </div>
        </div>
        <hr>
        <div id="contact" class="section-content">
            <div class="text-content">
                <h1 class="page-title">Contact</h1>
                <p class="simple-text">
                    Ne-ar plăcea să discutăm despre cum vă putem ajuta în proiectele dumneavoastră. Pentru orice întrebări sau pentru a solicita un serviciu, ne puteți contacta folosind informațiile de mai jos.
                </p>
                <p class="simple-text" style="margin-left: 1rem;">
                    • Adresă: <b>[]</b>
                    <br>• Telefon: <a class="simple-text" href="tel:+40744837601" style="text-decoration: none;"><b>+40 744 837 601</b></a>
                    <br>• Email: <b>[]</b>
                </p>
                <p class="simple-text">
                    Suntem nerăbdători să auzim de la dumneavoastră!
                </p>
            </div>
            <div class="image-container" style="display:flex; justify-content: right;">
                <img src="/assets/images/third-image.jpg" alt="Worker">
            </div>
        </div>
    </div>
</template>

<style scoped>
@media (min-width: 1550px) {
    .section-content {
        padding: 2rem 20rem !important;
    }

    hr {
        margin: 1rem 20rem !important;
    }

}
    .mobile-only {
        display: none;
    }
    .main-section-img {
        height: 600px; 
        object-fit: cover;
    }
    .second-section-img {
        height: 600px; 
        object-fit: cover;
    }
    .dark-overlay {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%; /* Full width to cover the image */
        height: 100%;
        background: linear-gradient(to right, rgb(0 0 0 / 75%), rgb(0 0 0 / 75%));
        pointer-events: none; /* Prevents interaction with the overlay */
    }
    .main-moto {
        font-size: 3rem;
        font-weight: 700;
        text-transform: uppercase;
        color: #ffc107;
    }
    .moto-description {
        font-size: 1.7rem;
    }
    .top-section-button {
        font-size: 1.3rem;
        color: black;
        background: transparent;
        border: 2px solid black;
        border-radius: 8px;
        padding: 0.4rem 1.2rem;
        margin-right: 1rem;
        display: inline-flex;
        align-items: center;
    }
    .card-button-size {
        width: 100%; 
        display: flex; 
        justify-content: center;
    }
    .card-button {
        font-size: 1.5rem;
        color: black;
        background: transparent;
        border-width: 2px;
        border-color: black;
        border-radius: 10px;
        padding: 0.4rem 1.2rem;
        margin-right: 1rem;
    }
    .card-button:hover {
        color: white;
        background: black;
    }
    .card-img-text {
        padding: 3rem 5rem;
        display: flex;
        align-items: center;
    }
    .main-section {
        padding: 1rem 5rem;
    }
    .main-section-title {
        width: 100%;
        font-size: 2rem;
        font-weight: 700;
        margin-bottom: 0.5rem;
    }

    .simple-text {
        font-size: 1.2rem;
        color: rgb(54, 54, 54);
        margin-top: 0;
    }

    .small-description {
        font-size: 1.4rem;
    }

    .page-title {
        margin-bottom: 1.2rem;
    }

    .image-container {
        flex: 1;
        max-width: 500px;
        height: auto;
        overflow: hidden;
        border-radius: 5px;
    }

    .image-container img {
        max-height: 400px;
    }

    .section-content {
        display: flex;
        flex-wrap: wrap;
        gap: 2rem;
        align-items: center;
        padding: 2rem 10rem;
    }

    .text-content {
        flex: 1;
    }
    
    .feature-card {
        width: 30%;
        border-width: 3px;
        border-radius: 15px;
        border-color: #656262;
        padding: 2rem;
    }

    .contact-button {
        width: 100%; 
        margin-top: 2rem;
    }

    .moto-container {
        display: flex; 
        width: 100%;
    }

    .moto-card {
        width: 50%;
    }

    .second-moto-container {
        display: flex; 
        width: 100%;
        justify-content: center;
    }

    .second-moto-card {
        width: 70%;
    }

    .second-moto-card .main-moto {
        color: white;
    }
    .moto-title-size {
        width: 100%; 
        margin-top: 1rem;
    }

    .moto-description-size {
        width: 100%; 
        margin-top: 1rem;
    }

    .second-moto .moto-title-size {
        width: 80%; 
        margin-top: 1rem;
    }

    .second-moto .moto-description-size {
        width: 80%; 
        margin-top: 1rem;
    }

    hr {
        margin: 1rem 10rem;
        border-top: 2px solid black;
    }

    @media (max-width: 768px) {
    .page-title {
        margin-bottom: 1rem;
    }
    .section-content {
      padding: 1rem 2rem;
      flex-direction: column;
        gap: 1rem;
    }
    .image-container {
      max-width: 100%;
      max-height: 300px;
    }
    .image-container img {
        width: 100%;
    }
    .second-img-section {
        max-height: 700px !important;
        height: 700px;
    }
    .second-img-section .moto-title-size{
        width: 100%;
    }
    .second-img-section .moto-description-size{
        width: 100%;
    }
    .second-img-section img{
        max-height: 700px !important;
    }
    .simple-text {
      font-size: 1rem;
    }
    .moto-container {
        flex-direction: column;
        gap: 1rem;
        text-align: center;
    }
    .moto-card {
        width: 100%;
    }
    .moto-title-size {
        width: 100%;
    }
    .main-moto {
        font-size: 2rem;
    }
    .moto-description-size {
        width: 100%;
    }
    .moto-description, .small-description {
        font-size: 1rem;
    }

    .main-section-img {
        height: 350px;
    }
    .second-section-img {
        height: 800px; 
    }
    .feature-card {
        width: 100%;
        padding: 1rem;
    }
    .card-button {
        font-size: 1.2rem;
    }
    .top-section-button {
        font-size: 1.2rem;
        margin-right: 0;
    }
    .contact-button {
        margin-top: 1rem;
        justify-content: center;
        display: flex;
    }
    .main-section {
        padding: 1rem 1rem !important;
    }
    .card-img-text {
        padding: 1rem 1rem !important;
    }
    hr {
      margin: 0 2rem;
    }
}
</style>