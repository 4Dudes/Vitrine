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
    }

    h3 {
        margin: 40px 0 0;
    }
    ul {
        list-style-type: none;
        padding: 0;
    }
    li {
        display: inline-block;
        margin: 0 10px;
    }
    a {
        color: #42b983;
    }


    @font-face {
        font-family: "Anstery";
        src: url('/src/font/AnsteryScript.otf');
    }

</style>