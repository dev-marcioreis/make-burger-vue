<template>

    <div class="burger-container">
        <p>Componente de mensagem</p>
        <div>
            <form class="burger-form">
                <div class="input-container">
                    <label for="name">Nome do cliente:</label>
                    <input type="text" id="name" name="name" v-model="name" placeholder="Digite seu nome">
                </div>
                <div class="input-container">
                    <label for="bread">Escolha seu pão:</label>
                    <select name="bread" id="bread" v-model="bread">
                        <option value="">Selecione uma opções...</option>
                        <option value="integral">Pão integral</option>
                    </select>
                </div>
                <div class="input-container">
                    <label for="meat">Escolha sua carne:</label>
                    <select name="meat" id="meat" v-model="meat">
                        <option value="">Selecione uma opções...</option>
                        <option value="titty">Maminha</option>
                    </select>
                </div>
                <div class="input-container optional-container">
                    <label for="optional" class="optional-title">Escolha os opcionais:</label>
                    <div class="checkbox-container">
                        <input type="checkbox" name="optional" value="salami" v-model="optional">
                        <span>Salame</span>
                    </div>
                    <div class="checkbox-container">
                        <input type="checkbox" name="optional" value="salami" v-model="optional">
                        <span>Salame</span>
                    </div>
                    <div class="checkbox-container">
                        <input type="checkbox" name="optional" value="salami" v-model="optional">
                        <span>Salame</span>
                    </div>
                </div>
                <div class="input-container">
                    <input type="submit" value="Meu Burger" class="submit-btn">
                </div>
            </form>
        </div>
    </div>

</template>

<script>

    export default {
        name: 'BurgerForm'
    }

</script>

<style scope>

    .burger-container {
        margin-block-start: 5rem;
    }
    .burger-form {
        max-width: 400px;
        margin: 0 auto;
    }
    .input-container {
        display: flex;
        flex-direction: column;
        margin-block-end: 1.2rem;
    }
    label {
        color: #003F83;
        font-weight: 700;
        margin-block-end: .5rem;
        padding: .4rem .8rem;
        border-left: 4px solid #F39735;
    }
    input, select {
        width: 300px;
        padding: .4rem .8rem;
    }
    .optional-container {
        flex-direction: row;
        flex-wrap: wrap;
    }
    .optional-title {
        width: 100%;
    }
    .checkbox-container {
        display: flex;
        align-items: center;
        width: 50%;
        margin-block-end: 1rem;
    }
    .checkbox-container span, .checkbox-container input {
        width: auto;
    }
    .checkbox-container span {
        margin-left: .2rem;
        font-weight: 700;
    }
    .submit-btn {
        background: #003F83;
        color: #F39735;
        font-weight: 700;
        font-size: 1rem;
        text-transform: uppercase;
        padding: .7rem;
        box-shadow: -20px 15px 5px hsla(0, 0%, 0%, 0.11);
        margin: 0 auto;
        cursor: pointer;
        transition: all 400ms ease-in-out;
    }
    .submit-btn:hover {
        box-shadow: none;
        background: #F39735;
        color: #fff;
    }

</style>