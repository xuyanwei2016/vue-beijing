<!--<template>
      <div class="play">
        <swiper>
          <swiper-slide>
            <img src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1511951103438&di=5e6d4f20232c9d59e12c3ee6772befe2&imgtype=0&src=http%3A%2F%2Fimg.taopic.com%2Fuploads%2Fallimg%2F140105%2F240374-14010513095146.jpg" alt="">
          </swiper-slide>
          <swiper-slide>Slide 2</swiper-slide>
          <swiper-slide>Slide 3</swiper-slide>
          <swiper-slide>Slide 4</swiper-slide>
          <swiper-slide>Slide 5</swiper-slide>
          <swiper-slide>Slide 6</swiper-slide>
          <swiper-slide>Slide 7</swiper-slide>
          <swiper-slide>Slide 8</swiper-slide>
          <swiper-slide>Slide 9</swiper-slide>
          <swiper-slide>Slide 10</swiper-slide>
        </swiper>
      </div>
</template>-->
<template>

      <swiper :options="swiperOption">
        <swiper-slide v-for="slide in swiperSlides">
          <div class="playcom">
          <img src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1511951103438&di=5e6d4f20232c9d59e12c3ee6772befe2&imgtype=0&src=http%3A%2F%2Fimg.taopic.com%2Fuploads%2Fallimg%2F140105%2F240374-14010513095146.jpg" alt="">
          <div class="playcon">
            <h2>最美的菜林深处，神仙居住的地方</h2>
            <i>雁荡山景区</i>
          </div>
          </div>

        </swiper-slide>

        <div class="swiper-pagination" slot="pagination"></div>


      </swiper>

</template>

<script>

  export default {
    name: 'carrousel',
    data() {
      return {
        nowindex:0,
        swiperOption: {
          autoplay: 11113500,
          grabCursor: true,
          setWrapperSize: true,
          pagination : '.swiper-pagination',
          paginationClickable :true,
          mousewheelControl : true,
          observeParents:true,
          loop:true,

        },
        swiperSlides: [1, 2, 3, 4, 5]
      }
    },
    mounted() {
      setInterval(() => {
        console.log('simulate async data')
        let swiperSlides = this.swiperSlides;

        /*if (swiperSlides.length < 10) swiperSlides.push(swiperSlides.length + 1)*/
      }, 3000)


    },
    /*methods:{
      goto(index){
        let that = this;
        this.ifshow = false;
        setTimeout(function(){
          that.ifshow = true;
          that.nowindex = index;
        },100)

      }
    }*/
  }
</script>
<style scoped>
  .swiper-container{width:96%;box-sizing: border-box;padding-left:4%;}
  .swiper-slide{ float: left;padding:0 4px 0 4px;overflow: hidden;animation: myfirst1 0.6s forwards;-moz-animation:myfirst1 0.6s linear forwards;}
  .playcom{position:relative;width:100%;overflow: hidden;/*padding-left: 0.15rem;*/}
  .playcom img{width:100%;border-radius: 0.05rem;}
  .playcon{height:0.8rem; background-color:rgba(0,0,0,0.3);position: absolute;bottom:0;
    display:flex; justify-content: space-between;color:#f8f8f8;}
  .playcon h2{font-size: 0.3rem; margin: 0;padding:0 0 0 0.15rem; line-height: 0.8rem;width:4.7rem;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;}
  .playcon i{font-size: 0.24rem;font-style: normal; background-image: url("../../img/title.png"); background-position: -1.3rem -0.44rem; background-size:1.6rem 1.8rem;height:0.5rem;background-repeat: no-repeat;padding-left: 0.38rem;margin-top:0.11rem; padding-top: 0.13rem;padding-right: 0.1rem;width:1.8rem;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;}
  .swiper-container .swiper-slide-next,.swiper-slide-prev{animation: myfirst 0.6s forwards;-moz-animation:myfirst 0.6s linear forwards;}
  @keyframes myfirst
  {
    from {opacity: 1}
    to {opacity: 0.5}
  }
  @keyframes myfirst1
  {
    from {opacity: 0.5}
    to {opacity: 1}
  }
   /*swiper-container-horizontal*/
  /*.swiper-pagination!* swiper-pagination-clickable swiper-pagination-bullets*!{position: fixed;z-index: 10;width:100%; height:200px;opacity: 0.5; background-color: aqua; bottom:0; left:0;overflow: hidden}
  .swiper-pagination span{ width:10px  !important; height:20px !important; background-color: red;position: absolute; float: left; top:0; left:0}
  .swiper-pagination-bullet{height:20px; width:20px; background-color: #000;}*/
</style>
