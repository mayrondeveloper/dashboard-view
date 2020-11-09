<template>
  <div class="card-ma card-product my-4">
    <div class="row">
      <div class="py-4 pl-4 d-flex flex-row">
        <div class="image-product pl-1">
          <img src="@/assets/image/beats-headphones.png" alt="">
        </div>
      </div>
      <div class="col-sm-12 col-md mt-md-4">
        <div class="description d-flex flex-column text-left px-3">
          <div class="name-product">{{ title }}</div>
          <div class="by">By <span>{{ brand }}</span></div>
          <div class="text pb-4">{{
              description
            }}
          </div>
        </div>
      </div>
      <div class="info-products text-center justify-content-center">
        <div class="p-3 d-flex flex-column">
          <div class="d-flex flex-column align-self-center">
            <div class="rank" v-if="rank"><span>3.4</span><img src="@/assets/image/icon/star-w.svg" alt=""></div>
            <div class="price">{{ price }}</div>
            <div class="cart"><img src="@/assets/image/icon/shopping-cart.svg" alt="">Free Shipping</div>
            <div class="buttons">
              <div>
                <button class="wishilistButton">Whishlist</button>
              </div>
              <div>
                <button class="addButton">Add to cart</button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
export default {
  name: "product",
  data() {
    return {
      n: null,
    }
  },
  props: {
    title: String,
    brand: String,
    description: String,
    price: String,
    rank: Boolean
    // eslint-disable-next-line vue/no-dupe-keys
  }
}
</script>

<style scoped lang="scss">
.info-products {
  margin: 0 auto;
  width: 240px;
  border-left: 1px solid #EBECF0;
  @media (max-width: 575.98px) {
    border: none;
  }
  @media (max-width: 934px) {
    border: 1px solid white;
  }
}


.card-product {
  padding: 0;
}

.buttons {
  margin-top: 14px;

  button {
    width: 186px;
  }
}

.rank {
  background: #FFAB00;
  border-radius: 3px;
  color: white;
  width: 60px;
  font-size: 14px;
  padding: 3px;
  display: flex;
  justify-content: center;
  align-content: flex-end;
  position: relative;
  align-self: end;

  span {
    margin-right: 3px;
  }
}

.price {
  margin-top: 20px;
  font-size: 18px;
  color: #091e42;
}

.cart {
  font-size: 14px;
  color: #172b4d;

  img {
    position: relative;
    top: -3px;
    margin-right: 10px;
  }
}

.description {
  padding-top: 14px;

  .name-product {
    font-size: 16px;
    color: #091e42;
  }

  .by {
    font-size: 12px;
    font-weight: 300;
    color: #FF000A;
    margin-top: 4px;
    margin-bottom: 10px;

    span {
      font-weight: 500;
    }
  }
  .text {
    font-size: 14px;
    color: #172b4d;
    font-weight: 300;
  }
}

</style>
