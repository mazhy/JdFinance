<template lang="html">
    <div>
      <Header></Header>
      <Hslider></Hslider>
      <Novice/>
      <Borrow/>
      <Monerty/>
      <Product/>
      <Life/>
      <Footer/>
      <Navbar/>
    </div>
</template>

<script>
import Header from '../public/header.vue'
import Hslider from './hslider.vue'
import Novice from './novice.vue'
import Borrow from './borrow.vue'
import Monerty from './monery.vue'
import Product from './product.vue'
import Life from './life.vue'
import Footer from '../public/footer.vue'
import Navbar from '../public/navbar.vue'
export default {
  components: {
    Header,
    Footer,
    Hslider,
    Novice,
    Borrow,
    Monerty,
    Product,
    Life,
    Navbar
  }
}
</script>
