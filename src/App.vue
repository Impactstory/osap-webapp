<template>
  <div id="app" class="container">
    <main-header/>
    <div class="container-wrapper md-layout-row">
      <router-view/>
    </div>
    <main-footer />

  </div>






</template>

<script>
    import MainHeader from './components/MainHeader'
    import MainFooter from './components/MainFooter'

    export default {
        name: 'App',
        components: {
            MainHeader,
            MainFooter
        },
        metaInfo: {
            // if no subcomponents specify a metaInfo.title, this title will be used
            title: 'Open Science dashboard',
            // all titles will be injected into this template
            titleTemplate: '%s | Open Science dashboard',
            link: [
                { rel: 'favicon', href: 'favicon.png' }
            ]
        }
    }
</script>

<style lang="scss">

  @import url("https://use.fontawesome.com/releases/v5.0.10/css/all.css");

  $screen-xsmall: 600px;
  $screen-small: 960px;

  body {
    background: #fff;
    code {
      padding: 2px 5px;
      border: 1px solid #ddd;
      border-radius: 3px;
      font-size: 90%;
    }
    h1 {
      margin-top: 50px;
    }
    h2 {
      margin-top: 50px;
    }
  }
  div.page {
    font-size: 18px;
    line-height: 1.5;
    max-width: 800px;
    margin: 50px auto;
    padding: 0 10px 100px;
    min-height: 80vh;
  }


  .vue-typer {
    .custom.char {
      /*color: #fff;*/
    }
  }

</style>
