<template>

  <section class="home">
    <Banner />
    <div class="container">
      <h1 class="burger-title">Monte seu hamburguer</h1>
      <BurgerForm />
    </div>
  </section>

</template>

<script>

  import Banner from '../components/Banner.vue';
  import BurgerForm from '@/components/BurgerForm.vue';

  export default {
    name: 'Home',
    components: {
      Banner,
      BurgerForm
    }
  }

</script>

<style scoped>

.burger-title {
  padding: 1rem 0;
  text-align: center;
  font-size: 1.2rem;
  color: #003F83;
  font-weight: 700;
  margin-block-end: 3rem;
}

</style>
