<template>

    <div class="banner-container">
        <div class="container">
            <h1>Faça seu próprio hambúrguer</h1>
        </div>
    </div>

</template>

<script>

    export default {
        name: 'Banner'
    }

</script>

<style scoped>

    .banner-container {
        background-image: url('../../public/images/banner.png');
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        height: 400px;
        display: flex;
        align-items: center;
        filter: contrast(1.5);
    }
    .banner-container h1 {
        font-family: 'Cedarville Cursive', cursive;
        background: #003f83ec;
        border-radius: .5rem;
        text-align: center;
        padding: 1rem 0;
        font-size: 4rem;
        color: #F39735;
        box-shadow: 0px 3px 6px #00000066;
        text-shadow: 0px 3px 6px #00000066;
    }

    @media (max-width: 768px) {
        .banner-container h1 {
            font-size: 3rem;
        }
    }

</style>