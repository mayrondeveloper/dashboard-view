<template>
  <div>
    <nav aria-label="Page navigation example">
      <ul class="pagination justify-content-center">
        <li class="page-item">
          <a class="page-link previous-control" href="#" tabindex="-1"></a>
        </li>
        <li class="page-item custom-page-item first-page-link"><a class="page-link" href="#">1</a></li>
        <li class="page-item custom-page-item"><a class="page-link" href="#">2</a></li>
        <li class="page-item custom-page-item"><a class="page-link" href="#">3</a></li>
        <li class="page-item custom-page-item"><a class="page-link" href="#">4</a></li>
        <li class="page-item custom-page-item"><a class="page-link" href="#">5</a></li>
        <li class="page-item custom-page-item active"><a class="page-link" href="#">6</a></li>
        <li class="page-item custom-page-item d-none d-md-block"><a class="page-link" href="#">7</a></li>
        <li class="page-item custom-page-item d-none d-md-block"><a class="page-link" href="#">8</a></li>
        <li class="page-item custom-page-item d-none d-md-block"><a class="page-link" href="#">9</a></li>
        <li class="page-item custom-page-item d-none d-md-block last-page-link"><a class="page-link" href="#">10</a></li>
        <li class="page-item">
          <a class="page-link next-control" href="#"></a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: "pagination"
}
</script>

<style scoped lang="scss">



</style>
