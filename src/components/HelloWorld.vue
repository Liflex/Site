<template>
  <div id="main">
    <div class="stars">
      <div class="twinkling">
        <div class="clouds">
          <div class="space">
            <div class="row swim">
              <div class="block-start">
                <transition name="fade">
                  <div v-if="start">
                    <h2 class="form-heading" style="color:rgb(0,76,255)">
                      <span class="fas fa-user-astronaut" style="color:rgb(113,18,255)"></span>
                      Do it</h2>
                    <button @click="start = !start">Priv</button>
                  </div>
                </transition>
              </div>
              <div class="block2">

              </div>
              <div class="block3">

              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// import common from 'src/css/common'
// import movestar from 'src/css/movestar'
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      start: true
    }
  }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="css">
  @import '../css/movestar.css';

  #main {

  }

  #main .row {
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
  }

  .block-start {
    width: 300px;
    height: 300px;
    margin: 20px;
    position: absolute;
    top: 350px;
  }
  .fade-leave-active {
    transition: all 1s cubic-bezier(1.0, 0.5, 0.8, 1.0);
  }
  .fade-leave-to
    /* .slide-fade-leave-active до версии 2.1.8 */ {
    transform: translateY(-200px);
    opacity: 0;
  }

  .block2 {
    width: 300px;
    height: 300px;
    margin: 20px;
    /*background: white;*/
  }

  .block3 {
    width: 300px;
    height: 300px;
    margin: 20px;
    /*background: white;*/
  }
</style>
