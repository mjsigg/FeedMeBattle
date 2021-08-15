<template>
    <div class="container">
        <Nav />
        <productpage />
    </div>

</template>

<script>
import Productpage from '../components/productpage.vue'
import producerapplication from './producerapplication.vue'
export default {
  components: { producerapplication, Productpage },
    
}
</script>

<style>

.container {

}
</style>