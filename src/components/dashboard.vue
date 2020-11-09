<template>
  <div class="container-fluid pr-3 pr-sm-4">
    <topbar />
    <breadcrumb />
    <div class="row products">
      <filters />
      <product-list />
    </div>
    <pagination />
  </div>
</template>

<script>
import Topbar from "@/components/dashComponents/topbar";
import Breadcrumb from "@/components/dashComponents/breadcrumb";
import Filters from "@/components/dashComponents/filters";
import ProductList from "@/components/dashComponents/productList";
import Pagination from "@/components/dashComponents/common/pagination";

export default {
  name: "Dashboard",
  components: { Pagination, ProductList, Filters, Breadcrumb, Topbar }
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
