<template>
  <article>
    <Slider :items="items" :cname="$style.slider"></Slider>
    <section :class="$style.list">
      <div :class="$style.item" v-for="item of enters" :key="item.img">
        <router-link :to="item.href">
          <img :src="item.img" :alt="item.title">
          <h4>{{item.title}}</h4>
        </router-link>
      </div>
    </section>
  </article>
</template>

<script>
import Slider from '../code/slider'
export default {
  data () {
    return {
      items: [
        {
          href:'home',
          src:'//img12.360buyimg.com/jrpmobile/jfs/t26368/348/1679436268/40503/35c319f0/5be8d994N1d428930.jpg?width=750&height=320'
        },
        {
          href:'home',
          src:'//img12.360buyimg.com/jrpmobile/jfs/t1/3690/33/14781/79350/5bdc1b03Ef9df3b40/05b336f969569a01.jpg?width=750&height=320'
        },{
          href:'home',
          src:'//img12.360buyimg.com/jrpmobile/jfs/t1/4093/34/15874/82184/5be0120fE739c627f/fcd0a90a6863602f.jpg?width=750&height=320'
        }
      ],
      enters: [{
        href:'home',
        img:'//img12.360buyimg.com/jrpmobile/jfs/t3991/64/2521945388/12110/93c0139/58d1e462Ncf294123.png?width=132&height=132',
        title:'优惠券'
      },{
        href:'home',
        img:'//img12.360buyimg.com/jrpmobile/jfs/t5590/252/875247023/17343/946aa72c/59224650N0f7ffc92.png?width=132&height=132',
        title:'领福利'
      },{
        href:'home',
        img:'//img12.360buyimg.com/jrpmobile/jfs/t4393/329/2180608902/13217/c88c0cec/58ec9dcdN1534e2d7.png?width=132&height=132',
        title:'领钢镚'
      },{
        href:'home',
        img:'//img12.360buyimg.com/jrpmobile/jfs/t5488/298/1036263348/12073/b4f4de97/590ac8e8Ne9def22e.png?width=135&height=135',
        title:'白条提额'
      },{
        href:'home',
        img:'//img12.360buyimg.com/jrpmobile/jfs/t1/520/34/950/3686/5b9239e3Eaaf5465c/8d8c35badacfc114.png?width=90&height=90',
        title:'工资理财'
      }]
    };
  },

  components: {
    Slider
  }
}

</script>
<style lang='scss' module>
  @import '../../css/element.scss';
  .slider{
    margin-top: 120px;
    img{
      width: 100%
    }
  }
  .list{
    @include list(row);
    background: #fff;
    padding-top: 40px;
    padding-bottom: 20px;
    justify-content: space-around;
    a {
      text-decoration: none;
      color: #333;
    }
    .item{
      text-align: center;
      img{
        display: inline-block;
        width: 90px;
        height: 90px;
      }
      h4{
        margin-top: 12px;
        font-size: 26px;
      }
    }
  }
</style>