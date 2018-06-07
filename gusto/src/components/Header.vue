<template>
    <header id="header">
        <h1>{{ title }}</h1>
        <h2>{{ subtitle}}</h2>
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

    #header{
        font-family: 'Anstery', Helvetica, Arial, sans-serif;
        font-weight: normal;
        font-style: normal;

    }

    @font-face {
        font-family: "Anstery";
        src: url('../font/AnsteryScript.otf');
    }

</style>