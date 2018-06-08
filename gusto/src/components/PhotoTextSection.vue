<!--
    Images à définir en dynamique dans les props et margin à enlever avant un nouveau component
    Ajouter les media pour le responsive ( < 800px )
-->

<template>
    <div class="main-container">
        <div class="photo-text-container" v-if="orientation === 'left'">
            <div class="photo"></div>
            <div class="text-container">
                <div class="title">{{ title }}</div>
                <div class="divider"></div>
                <div class="text">{{ text }}</div>
                <div class="button">{{ button }}</div>
            </div>
        </div>
        <div class="photo-text-container" v-else-if="orientation === 'right'" style="flex-direction: row-reverse">
            <div class="photo"></div>
            <div class="text-container">
                <div class="title">{{ title }}</div>
                <div class="divider"></div>
                <div class="text">{{ text }}</div>
                <div class="button">{{ button }}</div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "photo-text-section",
        props: {
            image: String,
            title: String,
            text: String,
            button: String,
            orientation: String,
        }
    }
</script>

<style scoped>

    .main-container {
        display: flex;
        justify-content: center;
    }

    div.photo-text-container {
        max-width: 1200px;
        width: 100%;
        display: flex;
        margin-top: 32px;
        flex-direction: row;
        flex-wrap: nowrap;
    }

    .text-container {
        display: flex;
        flex-direction: column;
        text-align: center;
        justify-content: center;
        width: 50%;
        padding: 0 16px;
    }

    .photo {
        background-image: url("../images/pic-6.jpg");
        width: 576px;
        height: 100%;
        min-height: 400px;
        background-size: cover;
    }
    .title {
        text-transform: uppercase;
        font-family: 'Anstery', Helvetica, Arial, sans-serif;
        font-weight: 700;
        font-size: 30px;
        margin-top: 32px;
    }
    .divider {
        width: 70%;
        height: 1px;
        background-color: #505050;
        margin-left: 15%;
        margin-top: 32px;
        margin-bottom: 16px;
    }
    .text {
        font-family: "Bariol";
        padding: 32px;
    }

    .button {
        text-transform: uppercase;
        font-family: "Bariol";
        font-weight: 300;
        font-size: 16px;
        border: 1px solid #505050;
        width: 410px;
        padding: 8px;
        margin-left: calc(50% - 215px);
    }
</style>