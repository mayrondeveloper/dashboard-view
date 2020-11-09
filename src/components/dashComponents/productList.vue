<template>
  <div class="col">
    <top-search-products />
    <search-input />
    <product title="Apple Watch Series 4 GPS" brand="Apple" description="Lorem Ipsum is simply dummy text of the
    printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
    when an unknown printer took a galley of type and scrambled it to make
a type specimen book." price="$399" rank />
    <product title="JBL Speaker" brand="JBL" description="Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make
a type specimen book." price="$199" />
    <product title="Apple iPhone X 128GB" brand="Apple" description="Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make
a type specimen book." price="$899" />
    <product title="Beats Headphones" brand="Beats" description="Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make
a type specimen book." price="$459" />
    <product title="Apple Watch Series 4 GPS" brand="Apple" description="Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make
a type specimen book." price="$2499" />
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
