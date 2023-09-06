<template>
    <div id="nav">
        <router-link id="logo-url" to="/">
            <img id="logo" src="../assets/logo.webp" :alt="ImagemSE2050">
        </router-link>
        <form action="" class="searchbar">
            <input type="text" placeholder="Pesquisar" name="q">
            <button id="sbtn" type="submit"><img src="../assets/searchicon.webp" alt="SearchIcon"></button>
            <button id="mbtn" type="submit"><img src="../assets/microicon.webp" alt="MicroIcon"></button>
        </form>
    </div>
</template>

<script setup>

</script>

<style scoped>

    #nav {
        background-color: var(--bgrey);
        border-bottom: 4px solid var(--color3);
        padding: 15px 50px;
        display: flex;
        justify-content: flex-end;
        align-items: center;
        width: 100%;
        min-height: 2rem;
    }

    #nav #logo-url {
        margin: auto;
        margin-left: 0;
        border-radius: 50%; /* Efeito Redondo no Logo */

    }

    #logo {
        width: 100px;
        height: 100px;
        will-change: filter;
        transition: filter 300ms;
    }

    #logo:hover {
        filter: drop-shadow(0 0 0.5em var(--white));
        background-color: transparent;
        opacity: 0.9;
    }

    #nav a:hover {
        color: #ffffff;
    }

    .searchbar{
        width: 100%;
        height: 40px;
        margin-right: auto; /* Centraliza Search Bar */
        max-width: 700px;
        background: var(--white);
        display: flex;
        align-items: center;
        border-radius: 60px;
        padding: 10px 20px;
        backdrop-filter: blur(4px) saturate(180%); /* Efeito Atrás do Search Bar */
    }

    .searchbar input{
        background: transparent;
        border: 0;
        outline: none;
        font-size: 20px;
        color: var(--black);
        resize: none;
        flex: 1; /* Ocupa o espaço restante */
        order: 2; /* Ordem 2 (vem depois dos botões) */
        text-align: center;
        -webkit-appearance: none; /* Para navegadores WebKit como Chrome e Safari */
        appearance: none; /* Para navegadores que suportam a propriedade appearance */
    }


    /* Evita o background do Autofill do Navegador */
    .searchbar input:-webkit-autofill,
    .searchbar input:-webkit-autofill:hover,
    .searchbar input:-webkit-autofill:focus,
    .searchbar input:-webkit-autofill:active{
        -webkit-box-shadow: 0 0 0 30px var(--white) inset !important;
    }

    ::placeholder{
        color: var(--black);
        text-align: center;
    }

    .searchbar button img{
        width: 25px;
    }

    .searchbar button{
        border: 0;
        border-radius: 50%;
        width: 40px;
        height: 40px;
        background: transparent;
        cursor: pointer;
        order: 1; /* Ordem 2 ( Orderna os elementos do searchbar ) */
    }

    .searchbar #sbtn{
        order: 3; /* Ordem 3 */
    }

    .searchbar #mbtn{
        order: 1; /* Ordem 1 */
    }

    .searchbar button:hover{
        filter: drop-shadow(0 0 0.5em var(--white));
        background-color: transparent;
        opacity: 0.8;
    }

</style>