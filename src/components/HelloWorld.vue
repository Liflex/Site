<template>
<div id="main">
  <div class="stars">
    <div class="twinkling">
      <div class="clouds">
        <div class="space">
          <div class="row swim">
            <div class="block1">

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
      msg: 'Welcome to Your Vue.js App'
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
  .block1 {
    width: 300px;
    height: 300px;
    margin: 20px;
    background: white;
    position: absolute;
    top: 350px;
  }
.block2 {
    width: 300px;
    height: 300px;
    margin: 20px;
    background: white;
  }
.block3 {
    width: 300px;
    height: 300px;
    margin: 20px;
    background: white;
  }
</style>
