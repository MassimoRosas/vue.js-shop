<template>
  <ShopProductsList :products="products" class="p-3"></ShopProductsList>
</template>

<script>
import ShopProductsList from './ShopProductsList';
import { eventBus } from '../../../../main';

export default {
  components: {
    ShopProductsList,
  },
  data() {
    return {
      products: []
    }
  },
  created() {
    this.products = eventBus.products;
    eventBus.$on('update:products', (products) => {
      this.products = products;
    })
  }
}
</script>

<style>

</style>
