<template>
    <header id="header" class="header">
        <h1>{{ title }}</h1>
        <h2>{{ subtitle }}</h2>
        <div class="round-divider"></div>
    </header>
</template>

<script>
    export default {
        name: 'Header',
        props: {
            title: String,
            subtitle: String
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

    .header {
        font-family: 'Anstery';
        height: 100%; /* Impossible de mettre une taille 100% pour recouvrir tout l'écran --'  */
        padding: 10% 0; /* Obligé de passer par un vieux padding de mort */
        background-image: url("../images/bg_1.jpg");
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        z-index: 1;
    }
    h1 {
        color:white;
        font-size: 150px;
        font-weight: 300;
        margin: inherit;
    }
    h2 {
        color:white;
        font-size: 90px;
        font-weight: 500;

    }
    /*.round-divider{
        background-image: url("../images/round-divider.png");
        z-index: 100;
        position: absolute;
        top: 10%;
        width: 100%;
        height: 1000px;
        background-repeat: no-repeat;
    }*/
</style>