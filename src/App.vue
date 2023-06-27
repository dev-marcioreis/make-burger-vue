<template>

  <Navbar :logo="logo_src" :alt="app_name" />
  <router-view/>
  <Footer />

</template>

<script>

  import Footer from './components/Footer.vue';
  import Navbar from './components/Navbar.vue';

  export default {
    components: {
      Navbar,
      Footer
    },
    data() {
      return {
        logo_src: '/images/logo.png',
        app_name: 'Faça seu próprio hambúrguer'
      }
    }
  }

</script>


<style>

/*==========Reset==========*/
*, *::before, *::after {
  margin: 0;
  padding: 0;
  border: 0;
  box-sizing: border-box;
  outline: none;
  text-decoration: none;
  list-style: none;
  font-family: 'Poppins', sans-serif;
}

/*==========General Styles==========*/
body {
  background: #FFEFBA;  /* fallback for old browsers */
  background: -webkit-linear-gradient(to right, #FFFFFF, #FFEFBA);
  background: linear-gradient(to right, #FFFFFF, #FFEFBA);
  color: #000;
  height: 100vh;
}
::-webkit-scrollbar {
  width: .5rem;
}
::-webkit-scrollbar-track {
  background: #003F83;
}
::-webkit-scrollbar-thumb {
  background: #fff;
}
.container {
  width: 80%;
  max-width: 1920px;
  margin-inline: auto;
}
section {
  margin-block-start: 8rem;
  height: 100vh;
}
h1, h2, h3, h4, h5, h6 {
  line-height: 1.1;
}
h1 {
  font-size: 3rem;
}
h2 {
  font-size: 2rem;
}
h3 {
  font-size: 1.6rem;
}
h4 {
  font-size: 1.1rem;
}
h5 {
  font-size: .9rem;
}
h6 {
  font-size: .8rem;
}
a {
  color: #000;
}
img {
  width: 100%;
}

/*==========Media Query Tablet==========*/
@media (max-width: 992px) {
  body {
    font-size: 1rem;
  }
  .container {
    width: 90%;
  }
  h1 {
    font-size: 2rem;
  }

}

/*==========Media Query Mobile==========*/
@media (max-width: 768px) {
  h1 {
    font-size: 2.4rem;
  }
  h2 {
    font-size: 1.8rem;
  }
  h3 {
    font-size: 1.4rem;
  }
  h4 {
    font-size: 1rem;
  }

}

</style>
