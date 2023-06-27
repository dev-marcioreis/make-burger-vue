<template>

    <nav class="navbar">
        <div class="container">
            <div class="navbar-container">
                <router-link to="/" class="logo-url">
                    <img :src="logo" :alt="alt" class="logo">
                    <span>bur<small>ger</small></span>
                </router-link>
                <div class="navbar-links">
                    <router-link to="/">
                        início
                    </router-link>
                    <router-link to="/pedidos">
                        pedidos
                    </router-link>
                </div>
            </div>
        </div>
    </nav>

</template>

<script>

    export default {
        name: 'Navbar',
        props: ['logo', 'alt']
    }

</script>

<style scoped>

    .navbar {
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        background: #003F83;
        height: 3.5rem;
        box-shadow: 0px 3px 6px #00000066;
    }
    .navbar-container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 3.5rem;
    }
    .logo-url {
        display: flex;
        align-items: center;
        gap: .5rem;
    }
    .logo {
        width: 2.4rem;
        transition: all 400ms ease-in-out;
        animation: 3s scale linear infinite;
    }

    @keyframes scale {
        0% {
            transform: scale(1);
        }
        50% {
            transform: scale(1.3);
        }
        100% {
            transform: scale(1);
        }
    }
    .logo-url span {
        text-transform: uppercase;
        font-size: 1rem;
        font-weight: 900;
        color: #F39735;
        text-shadow: 0px 3px 6px #00000066;
        font-style: italic;
    }
    .logo-url span small {
        font-size: 1rem;
        color: #fff;
    }
    .navbar-links {
        display: flex;
        align-items: center;
        gap: 2rem;
    }
    .navbar-links a {
        color: #fff;
        text-transform: capitalize;
        font-weight: 700;
        letter-spacing: 2px;
        text-shadow: 0px 3px 6px #00000066;
        transition: all 400ms ease-in-out;
    }
    .navbar-links a:hover {
        color: #F39735;
    }

</style>
