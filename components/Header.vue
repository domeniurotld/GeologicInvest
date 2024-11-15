<template>
    <header class="header">
      <div class="row desktop-only align-items-center">
        <div class="row" style="display: flex; justify-content: start; width: 30%;">
          <a href="" style="width: auto;">
              <button class="tab-button" style="display: inline-flex; align-items: center; padding-top: 0.4rem; padding-bottom: 0.4rem;"> 
                  <span style="font-weight: 900;">GEOLOGIC INVEST</span>
              </button>
          </a>
        </div>
        <!-- <div class="col-auto logo">
          <img src="/assets/images/logo.png" alt="Logo" @click="goToRoute('/')"/>
        </div> -->
        <nav class="nav nav-right">
          <button class="tab-button" @click="goToRoute('/')">Acasă</button>
          <button class="tab-button" @click="scrollToSection('aboutus')">Despre noi</button>
          <button class="tab-button" @click="scrollToSection('services')">Servicii</button>
          <button class="tab-button" @click="scrollToSection('contact')">Contact</button>
        </nav>
      </div>

      <div class="col mobile-only">
        <!-- <div class="logo" style="padding: 0;">
          <img src="/assets/images/logo.png" alt="Logo" @click="goToRoute('/')"/>
        </div> -->
        <div style="display: flex; justify-content: center; width: 100%; margin-top: 1rem;">
          <a href="" style="width: auto;">
              <button class="tab-button" style="display: inline-flex; align-items: center; padding-top: 0.4rem; padding-bottom: 0.4rem;"> 
                  <span style="font-size: 28px; font-weight: 900;">GEOLOGIC INVEST</span>
              </button>
          </a>
        </div>
        <nav class="nav nav-left" style="margin-top: 1rem; margin-bottom: 1rem;">
          <div style="display: flex; justify-content: center; width: 100%; gap: 1rem; padding: 0 1rem;">
            <button class="tab-button" style="width: 25%;" @click="goToRoute('/')">Acasă</button>
            <button class="tab-button" style="width: 25%;" @click="scrollToSection('aboutus')">Despre</button>
            <button class="tab-button" style="width: 25%;" @click="scrollToSection('services')">Servicii</button>
            <button class="tab-button" style="width: 25%;" @click="scrollToSection('contact')">Contact</button>
          </div>
        </nav>
        <!-- <div class="row" style="display: flex; justify-content: center; margin-bottom: 1rem;">
          <a href="tel:+40740128833" style="width: auto;">
              <button class="tab-button" style="display: inline-flex; align-items: center; border:2px solid black; padding-top: 0.4rem; padding-bottom: 0.4rem;"> 
                  <Icon name="material-symbols:call" size="1.7rem" style="margin-right: 0.7rem;" /> 
                  <span>Contactați-ne</span>
              </button>
          </a>
        </div> -->
      </div>
    </header>
  </template>
  
<script>
  export default {
    methods: {
    goToRoute(route) {
      this.$router.push(route).then(() => {
        this.scrollToTop();
      });
    },
    goToHomeSection(section) {
      this.$router.push("/").then(() => {
        this.scrollToSection(section);
      });
    },
    goToHomeSection(section) {
      this.$router.push("/").then(() => {
        this.scrollToSection(section);
      });
    },
      scrollToSection(sectionId) {
        const section = document.getElementById(sectionId);
        if (section) {
          section.scrollIntoView({ behavior: 'smooth' });
        }
      },
      scrollToTop() {
        window.scrollTo({ top: 0, behavior: 'smooth' });
      }
    }
  }
  </script>
  
  <style scoped>
  
  @media (min-width: 1550px) {
    .header {
      padding-left: 19rem !important;
      padding-right: 19rem !important;
    }

  }

    .desktop-only {
      width:100%; 
      flex-direction:row; 
      display: flex;
    }
  
    .mobile-only {
      display: none; 
    }
  
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: auto;
    background: grey;
    padding: 0.5rem 9rem;
  }
  
  .logo {
    display: flex;
    height: 100px;
    align-items: center;
    margin-left: 9rem;
    width: 17%;
  }

  .logo img {
    height: 80px;
    cursor: pointer;
  }
  
  .nav {
    display: flex;
    gap: 1rem;
  }
  
  .nav-left {
    flex: 1;
    padding: 0 1.2rem;
  }
  
  .nav-right {
    flex: 1;
    justify-content: end;
  }
  
  .tab-button {
    width: auto;
    font-size: 20px;
    padding: 2px 10px;
    font-weight: 500;
    border: none;
    outline: none;
    color: black;
    background: transparent;
    border-radius: 0;
    cursor: pointer;
    }

    .dropdown {
      position: relative;
      display: inline-block;
    }

    .dropdown-container {
      display: none;
      position: absolute;
      right: 0;
      background: transparent;
      z-index: 1;
    }
    .dropdown-content {
      background: linear-gradient(
        45deg,
        #e3dddd 5%,
        #fff 10%,
        #ccc 30%,
        #ddd 50%,
        #ccc 70%,
        #fff 80%,
        #bebebe 95%
      );
      min-width: 150px;
      box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
      border-radius: 5px;
      margin-top: 5px;
    }

    .dropdown-content a {
      color: black;
      padding: 5px 15px;
      text-decoration: none;
      display: block;
      font-weight: 600;
      border-radius: 5px;
      cursor: pointer;
      
    }

    .dropdown-content hr {
      margin: 0;
      height: 2px;
    }

    .dropdown-content a:hover {
      background-color: #000000;
      color: white;
      
    }

    .dropdown:hover .dropdown-container {
      display: block;
    }
  
  /* Responsive Design */
  @media (max-width: 768px) {
    .desktop-only {
      display: none;
    }
  
    .mobile-only {
      width: 100%; 
      display: flex; 
      flex-direction: column;
    }
  
    .header {
      flex-direction: column;
      align-items: center;
      padding: 0;
    }
  
    .nav {
      width: 100%;
    }
  
    .nav-left, .nav-right {
      align-items: center;
    }
  
    .tab-button {
      font-size: 1.1rem;
    }

    .logo {
      margin-left: 1rem;
      width: auto;
    }
  }
  </style>
  