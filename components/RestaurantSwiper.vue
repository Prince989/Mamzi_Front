<template>
  <div>
    <div class="swiper-container swiper2" dir="rtl">
      <!-- Additional required wrapper -->
      <div class="swiper-wrapper">
        <!--        <div class="row m-0 d-flex justify-content-center flex-lg-nowrap Restaurant-Card-Container">-->
        <div class="swiper-slide row m-0 d-flex justify-content-center flex-nowrap Restaurant-Card-Container"
             v-for="n in x">
          <RestaurantCard class="col-lg-3 col-md-4 col-sm-5 col-12 m-1" v-for="r in indexer(n)" :key="r.name" dir="ltr">

          </RestaurantCard>
        </div>
        <!--        </div>-->
      </div>
      <div class="swiper-pagination pagination2"></div>
    </div>
    <div class="d-flex justify-content-center" dir="rtl">
<!--      <div class="swiper-pagination pagination2"></div>-->
    </div>
  </div>
</template>

<script>
  import Swiper, {Navigation, Pagination} from 'swiper'
  import 'swiper/swiper-bundle.css'

  Swiper.use([Navigation, Pagination]);
  export default {
    name: "RestaurantSwiper",
    data() {
      return {
        restaurants: [{'name': 'جوجه طلایی'}, {'name': 'کباب طلایی'}, {'name': 'برگر طلایی'}, {'name': 'پیتزا طلایی'},
          {'name': 'فست فود طلایی'}, {'name': 'جوجه رنگی'}, {'name': 'کباب رنگی'}, {'name': 'برگر رنگی'}, {'name': 'پیتزا رنگی'}, {'name': 'جوجه نگین'},
          {'name': 'کباب نگین'}],
        windowWidth: 0,
        x: [],
        y: [],
        swip: []
      }
    },
    methods: {
      arrange() {
        let w = this.windowWidth;
        if (w >= 992) {
          this.arrangeSlides(4);
          console.log("lg" + 4)
        } else if (w < 992 && w >= 768) {
          this.arrangeSlides(3);
          console.log("md" + 3)
        } else if (w < 768 && w >= 576) {
          this.arrangeSlides(2);
        } else if (w < 576) {
          this.arrangeSlides(1);
        }
      },
      arrangeSlides(x) {
        this.x = [];
        this.y = [];
        let r = this.restaurants.length % x;
        let t = Math.floor(this.restaurants.length / x);
        if (r > 0) {
          t++;
        }
        for (let i = 0; i < t; i++) {
          this.x.push(i);
        }
        console.log("t :" + t);
        for (let i = 0; i < t; i++) {
          console.log(i);
          this.y[i] = new Array();
          for (let j = 0; j < x; j++) {
            if (this.restaurants[(i * x) + j] !== undefined) {
              this.y[i].push(this.restaurants[(i * x) + j]);
            }
          }
        }
        console.log(this.y);
        this.readySwiper();
      },
      readySwiper() {
        this.swip = new Swiper('.swiper2', {
          loop: false,
          observer: true,
          observeParents: true,
          pagination: {
            el: '.pagination2',
          },
          /*,
          navigation: {
            nextEl: '.swiper-button-next',
            prevEl: '.swiper-button-prev',
          },
          scrollbar: {
            el: '.swiper-scrollbar',
          },*/
        });
        console.log("SwiperReady");
        this.swip.update();
        setTimeout(()=>{
          let v = document.getElementsByClassName('swiper-pagination-bullet');
          v.forEach(function (x) {
            x.classList.add('spp');
            console.log("vvv");
          });
          this.swip.update();
        },5000);

      }
      ,
      indexer(t) {
        return this.y[t];
      },
    },
    mounted() {
      if (process.browser) {
        this.windowWidth = window.innerWidth;
        this.arrange();
      }
      // this.hasClass();
/*      for(let x in v){
        x.classList[0].add('spp');
      }*/
    },
    created() {
      if (process.browser) {
        console.log(window.innerWidth, window.innerHeight);
        window.onresize = () => {
          this.windowWidth = window.innerWidth;
          console.log(this.windowWidth);
          this.arrange();
        }
      }
    },
  }
</script>

<style scoped>
  .Restaurant-Card-Container {
    padding: 30px 70px 70px 70px;
  }

  .swiper-pagination-bullet {
    margin: 3px
  }

  .spp {
    margin: 15px !important;
  }

  .swiper-pagination * {
    margin: 3px
  }
  .pagination2{

  }
</style>
