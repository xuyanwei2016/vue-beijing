<template>
    <div class="eat">
      <ul>
        <li>
          <div class="imgtop">
            <img src="../../img/chi.jpg" alt="">
            <h2>特别推荐</h2>
          </div>
          <div class="conbtn">
            <h3>北京烤鸭</h3>
            <i>人均：50元</i>
          </div>
          <p>烤鸭已成为北京饮食的象征。据说基辛格每次到北京是必吃烤鸭的。</p>
        </li>
        <li>
          <div class="imgtop">
            <img src="../../img/chi.jpg" alt="">
            <h2>特别推荐</h2>
          </div>
          <div class="conbtn">
            <h3>北京烤鸭</h3>
            <i>人均：50元</i>
          </div>
          <p>烤鸭已成为北京饮食的象征。据说基辛格每次到北京是必吃烤鸭的。</p>
        </li>
        <li>
          <div class="imgtop">
            <img src="../../img/chi.jpg" alt="">
            <h2>特别推荐</h2>
          </div>
          <div class="conbtn">
            <h3>北京烤鸭</h3>
            <i>人均：50元</i>
          </div>
          <p>烤鸭已成为北京饮食的象征。据说基辛格每次到北京是必吃烤鸭的。</p>
        </li>
        <li>
          <div class="imgtop">
            <img src="../../img/chi.jpg" alt="">
            <h2>特别推荐</h2>
          </div>
          <div class="conbtn">
            <h3>北京烤鸭</h3>
            <i>人均：50元</i>
          </div>
          <p>烤鸭已成为北京饮食的象征。据说基辛格每次到北京是必吃烤鸭的。</p>
        </li>
      </ul>
    </div>
</template>

<script>
    export default {
        data() {
            return {}
        },
        components: {},
        methods: {}
    }
</script>

<style scoped>
  .eat{padding: 0 .15rem 0 0.15rem;}
  .eat ul{ display: flex;justify-content: space-between; flex-wrap: wrap;}
  .eat ul li{ width:3.4rem; padding-bottom: 0.1rem;}
  .eat ul li .imgtop{position: relative;}
  .eat ul li img{width:3.4rem; height:2rem;}
  .eat ul li h2{position: absolute;top:0.1rem;left:0.1rem;width:1.3rem;height:0.5rem; background-color:rgba(0,0,0,0.5); font-size: 0.24rem;color:#fff; margin: 0;padding:0; font-weight:100; border-radius:0.3rem 0 0.3rem 0.3rem; line-height: 0.5rem; text-align: center;}
  .eat ul li .conbtn{ display: flex; justify-content: space-between; height:0.5rem; line-height: 0.5rem;}
  .eat ul li .conbtn h3{margin: 0;padding: 0; font-size: 0.32rem;line-height:0.5rem;font-weight:600}
  .eat ul li .conbtn i{ font-size: 0.26rem; font-style: normal; color:#af0000;}
  .eat ul li p{line-height: 0.34rem;font-size: 0.22rem;}

</style>
