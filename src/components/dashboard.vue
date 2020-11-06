<template>
  <div class="container-fluid">
    <topbar />
    <breadcrumb />
    <div class="row products">
      <filters />
      <product-list />
    </div>
  </div>
</template>

<script>
import Topbar from "@/components/dashComponents/topbar";
import Breadcrumb from "@/components/dashComponents/breadcrumb";
import Filters from "@/components/dashComponents/filters";
import ProductList from "@/components/dashComponents/productList";

export default {
  name: "Dashboard",
  components: { ProductList, Filters, Breadcrumb, Topbar }
}
</script>
<style lang="scss">
.dropdown-filter {
  opacity: 0;
}
@media (max-width: 1500px) {
  .products {
    flex-direction: column;
  }
  .filters {
    display: none;
  }
  .dropdown-filter {
    opacity: 1;
  }
}
</style>
