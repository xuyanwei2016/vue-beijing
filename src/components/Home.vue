<template>
    <div>
      <div class="banner">
        <img src="../../img/banner.jpg" alt="">
      </div>
      <ul class="navbar">
        <li><router-link to="/"></router-link></li>
        <li><router-link to="/"></router-link></li>
        <li><router-link to="/"></router-link></li>
        <li><router-link to="/"></router-link></li>
        <li><router-link to="/"></router-link></li>
      </ul>
      <div class="content">
        <div class="eat">
          <div class="titlebar">
            <div></div>
            <i class="more"><router-link to="/eat"></router-link></i>
          </div>
          <Eat></Eat>
        </div>
        <div class="play">
          <div class="titlebar">
            <div></div>
            <i class="more"><router-link to="/eat"></router-link></i>
          </div>
          <Play></Play>
        </div>
        <div class="happly">
          <div class="titlebar">
            <div></div>
            <i class="more"><router-link to="/eat"></router-link></i>
          </div>
          <Happly></Happly>
        </div>
      </div>
    </div>
</template>

<script>
  import Eat from '../components/Eat.vue';
  import Play from '../components/Play.vue';
  import Happly from '../components/Happly.vue';
    export default {
        data() {
            return {}
        },
        components: {
          Eat,
          Play,
          Happly
        },
        methods: {}
    }
</script>

<style scoped>
  .banner{ width:7.5rem;}
  .banner img{width:100%;}
  .navbar{ padding:0;margin-bottom:0;display: flex; flex-direction: row; justify-content: space-between;margin-top: 0.2rem;border-bottom: .01rem #bababa solid; height:1.25rem;}
  .navbar li{ width: 1rem; height:1rem;}
  .navbar li:nth-child(1){background-image: url("../../img/title.png"); background-repeat: no-repeat; background-position:0 0; background-size:5.1rem 5.8rem;}
  .navbar li:nth-child(2){background-image: url("../../img/title.png"); background-repeat: no-repeat; background-position:-1rem 0; background-size:5.1rem 5.8rem;}
  .navbar li:nth-child(3){background-image: url("../../img/title.png"); background-repeat: no-repeat; background-position:-2.01rem 0; background-size:5.1rem 5.8rem;}
  .navbar li:nth-child(4){background-image: url("../../img/title.png"); background-repeat: no-repeat; background-position:-3.02rem 0; background-size:5.1rem 5.8rem;}
  .navbar li:nth-child(5){background-image: url("../../img/title.png"); background-repeat: no-repeat; background-position:-4.03rem 0; background-size:5.1rem 5.8rem;}

  .content{width:100%; height:100%;background-color: #f6f6f6;}
  .titlebar{height:1.15rem; padding-top:0.3rem; position: relative}
  .titlebar div{width:3rem;height: 0.7rem; margin: 0 auto;}
  .eat .titlebar div:nth-child(1){background-image: url("../../img/title.png");background-repeat: no-repeat; background-position:0 -1.15rem; background-size: 3.8rem 4rem;}
  .titlebar .more{width:0.9rem; height:0.4rem;position: absolute;right:0;top:0.38rem; background-image: url("../../img/title.png"); background-repeat: no-repeat; background-position:0 -1.2rem; background-size: 5.1rem 5.8rem;}
  .titlebar .more a{width:0.9rem; height:0.4rem; display: block}
  .play .titlebar div:nth-child(1){background-image: url("../../img/title.png");background-repeat: no-repeat; background-position:0 -1.79rem; background-size: 3.8rem 4rem;}
  .play{overflow: hidden;}
  .happly .titlebar div:nth-child(1){background-image: url("../../img/title.png");background-repeat: no-repeat; background-position:0 -1.79rem; background-size: 3.8rem 4rem;}


</style>
