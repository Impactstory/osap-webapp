<template>
  <div class="page home">
    <div class="content">
      <h2>
          Welcome to the Open Science Assessment Project page for
      the National Institutes of Mental Health
      </h2>
      <div class="more">
        <div class="buttons">
          <md-button class="md-raised md-button md-primary" to="investigators">
            View investigators
          </md-button>

          <md-button class="md-raised md-button" to="faq">
            View FAQ
          </md-button>
        </div>

        <p>
          This project is a collaboration between the nonprofit <a href="https://impactstory.org">Impactstory</a> and the <a
                href="https://www.nimh.nih.gov/index.shtml">National Institutes of Mental Health,</a> part of the <a
                href="https://www.nimh.nih.gov/index.shtml">US National Institutes of Health.</a>
        </p>
        <p>
          Our goal is to create a system that will help decision-makers track, and ultimately reward, all kinds of <a
                href="https://en.wikipedia.org/wiki/Open_science">open science</a> practices from faculty at any institution. For now, we're in the trial stage, and limited to use with NIMH intramural researchers. For now we track just three practices: open sharing of papers (open access), data, and code. Please interpret results with caution since we're still in the trial stage.
        </p>
      </div>
    </div>



  </div>
</template>

<script>
    import axios from 'axios'

    export default {
        name: 'Home',
        data: () => ({
        }),
        components: {
            axios
        },
        metaInfo: {
            title: 'Home'
        },
        computed: {

        },
        methods: {
        },
        mounted() {
        }
    }
</script>


<style scoped lang="scss">

  .page.home {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vm;
    .content {
      max-width: 600px;
      .buttons {
        margin-bottom: 30px;
      }
      p {
        font-size: 18px;
      }
    }

  }




</style>
