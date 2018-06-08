<template>
  <div id="app">
    <Header title="Gusto !" subtitle="Italiano Ristorante" />
    <PhotoTextSection
            image="../images/pic-6.jpg"
            title="Nos produits favoris !"
            text="Ils sont bons, ils sont frais, un peu comme la mère de Bastien mais en moins mouillés ! Le plat-signature du Boccaccio, servi directement depuis le poêlon. La revisite gastronomique de ce plat populaire espagnol explose dans l’assiette : couleurs, odeurs, saveurs… Tous les sens sont sublimés par des matériaux nobles. Le riz brille, les légumes éclatent et que dire des invités de la mer ? Gambas, calamars, moules, palourdes, poulpes… C’est tout l’océan qui s’invite !"
            button="Il en reste ? Fais ton ricains et demande un takeway !"
            orientation="left"
    />
    <PhotoTextSection
            image="../images/pic-4.jpg"
            title="Nos produits favoris !"
            text="Ils sont bons, ils sont frais, un peu comme la mère de Bastien mais en moins mouillés ! Le plat-signature du Boccaccio, servi directement depuis le poêlon. La revisite gastronomique de ce plat populaire espagnol explose dans l’assiette : couleurs, odeurs, saveurs… Tous les sens sont sublimés par des matériaux nobles. Le riz brille, les légumes éclatent et que dire des invités de la mer ? Gambas, calamars, moules, palourdes, poulpes… C’est tout l’océan qui s’invite !"
            button="Il en reste ? Fais ton ricains et demande un takeway !"
            orientation="right"
    />
    <PhotoTextSection
            image="../images/pic-6.jpg"
            title="Nos produits favoris !"
            text="Ils sont bons, ils sont frais, un peu comme la mère de Bastien mais en moins mouillés ! Le plat-signature du Boccaccio, servi directement depuis le poêlon. La revisite gastronomique de ce plat populaire espagnol explose dans l’assiette : couleurs, odeurs, saveurs… Tous les sens sont sublimés par des matériaux nobles. Le riz brille, les légumes éclatent et que dire des invités de la mer ? Gambas, calamars, moules, palourdes, poulpes… C’est tout l’océan qui s’invite !"
            button="Il en reste ? Fais ton ricains et demande un takeway !"
            orientation="left"
    />
  </div>
</template>

<script>
    import HelloWorld from './components/HelloWorld.vue'
    import Header from './components/Header.vue'
    import PhotoTextSection from './components/PhotoTextSection.vue'

    export default {
        name: 'app',
        components: {
            Header,
            HelloWorld,
            PhotoTextSection
        }
    }
</script>

<style>
  #app {
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }

  body, html{
    margin: inherit;
    height: 100%;
  }

  @font-face {
    font-family: "Anstery";
    src: url('./font/AnsteryScript.otf');
  }

  @font-face {
    font-family: "MyriadPro";
    src: url('./font/MyriadPro-Regular.otf');
  }

  @font-face {
    font-family: "Bosk";
    src: url("./font/Bosk.otf");
  }

  @font-face {
    font-family: "Bariol";
    src: url("./font/Bariol_Regular.otf");
  }

</style>
