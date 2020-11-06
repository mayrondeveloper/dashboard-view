<template>
  <div class="col">
    <top-search-products />
    <search-input />
    <product />
    <product />
    <product />
    <product />
    <product />
  </div>
</template>

<script>
import TopSearchProducts from "@/components/dashComponents/productsComponents/topSearchProducts";
import SearchInput from "@/components/dashComponents/productsComponents/search";
import Product from "@/components/dashComponents/productsComponents/product";
export default {
name: "productList",
  components: { Product, SearchInput, TopSearchProducts }
}
</script>

<style scoped>

</style>
