<template>
  <div class="filters col-sm-12 col-md-3">
    <div class="">
      <div class="top-title text-left">Filters</div>
      <div class="card-ma text-left card-filter">
        <div class="title mb-2">Multi Range</div>
        <div class="elements">
          <b-form-group label="">
            <b-form-radio v-model="selectedRadio" name="some-radios" value="1">$10</b-form-radio>
            <b-form-radio v-model="selectedRadio" name="some-radios" value="2">$10-$100</b-form-radio>
            <b-form-radio v-model="selectedRadio" name="some-radios" value="3">$100 - $500</b-form-radio>
            <b-form-radio v-model="selectedRadio" name="some-radios" value="4">$500</b-form-radio>
            <b-form-radio v-model="selectedRadio" name="some-radios" value="5">All</b-form-radio>
          </b-form-group>
        </div>
        <div class="separator"></div>
        <div class="d-flex flex-row justify-content-between">
          <div class="title mb-2">Slider</div>
          <div class="title mb-2">1.99 - 4098</div>
        </div>
        <div class="slidecontainer pb-2 elements">
          <input type="range" min="1" max="100" value="50" class="slider" id="myRange">
        </div>
        <div class="separator"></div>
        <div class="title">Category</div>
        <b-form-group class="elements mt-2" label="">
          <b-form-checkbox-group v-model="selected" plain stacked>
            <b-form-checkbox value="orange">Cell Phones<span>1920</span></b-form-checkbox>
            <b-form-checkbox value="apple">Computers & Tablet<span>1820</span></b-form-checkbox>
            <b-form-checkbox value="pineapple">Cell Phone Accessories<span>462</span></b-form-checkbox>
            <b-form-checkbox value="Appliances">Appliances<span>6556</span></b-form-checkbox>
            <b-form-checkbox value="Audio">Audio<span>120</span></b-form-checkbox>
            <b-form-checkbox value="iPhone Accessories">iPhone Accessories<span>353</span></b-form-checkbox>
            <b-form-checkbox value="Cameras & Camcorders">Cameras & Camcorders<span>45</span></b-form-checkbox>
            <b-form-checkbox value="iPhone Cases & Clips">iPhone Cases & Clips<span>456</span></b-form-checkbox>
            <b-form-checkbox value="TV & Home Theater">TV & Home Theater<span>55</span></b-form-checkbox>
            <b-form-checkbox value="Small Kitchen Appliances">Small Kitchen Appliances<span>10</span></b-form-checkbox>
          </b-form-checkbox-group>
        </b-form-group>
        <div class="separator"></div>
        <div class="title">Brand</div>
        <b-form-group class="mt-2 elements" label="">
          <b-form-checkbox-group v-model="selected" plain stacked>
            <b-form-checkbox value="orange">Insigni<span>220</span></b-form-checkbox>
            <b-form-checkbox value="apple">Samsung<span>120</span></b-form-checkbox>
            <b-form-checkbox value="pineapple">Apple<span>320</span></b-form-checkbox>
            <b-form-checkbox value="Appliances">HP<span>32</span></b-form-checkbox>
            <b-form-checkbox value="Audio">Sony<span>520</span></b-form-checkbox>
            <b-form-checkbox value="iPhone Accessories">Metra<span>55</span></b-form-checkbox>
            <b-form-checkbox value="Cameras & Camcorders">Dyne<span>120</span></b-form-checkbox>
            <b-form-checkbox value="iPhone Cases & Clips">LG<span>98</span></b-form-checkbox>
            <b-form-checkbox value="TV & Home Theater">Canon<span>99</span></b-form-checkbox>
            <b-form-checkbox value="Small Kitchen Appliances">Speck<span>575</span></b-form-checkbox>
          </b-form-checkbox-group>
        </b-form-group>
        <div class="separator"></div>
        <div class="title mb-4">Rating</div>
        <div class="elements">
          <div class="rating mt-2">
            <div class="stars d-flex justify-content-between">
              <div class="d-flex">
                <span class="checked-star"></span>
                <span class="checked-star"></span>
                <span class="checked-star"></span>
                <span class="checked-star"></span>
                <span class="checked-star"></span>
                <div class="up">& UP</div>
              </div>
              <div class="reference-number">525</div>
            </div>
          </div>
          <div class="rating mt-2">
            <div class="stars d-flex justify-content-between">
              <div class="d-flex">
                <span class="star checked-star"></span>
                <span class="star checked-star"></span>
                <span class="star checked-star"></span>
                <span class="checked-star"></span>
                <span class="star"></span>
                <div class="up">& UP</div>
              </div>
              <div class="reference-number">525</div>
            </div>
          </div>
          <div class="rating mt-2">
            <div class="stars d-flex justify-content-between">
              <div class="d-flex">
                <span class="checked-star"></span>
                <span class="checked-star"></span>
                <span class="checked-star"></span>
                <span class="star"></span>
                <span class="star"></span>
                <div class="up">& UP</div>
              </div>
              <div class="reference-number">525</div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <b-modal id="modal-1" title="Filters">
      <div class="">
        <div class="card-ma text-left card-filter">
          <div class="title mb-2">Multi Range</div>
          <div class="elements">
            <b-form-group label="">
              <b-form-radio v-model="selectedRadio" name="some-radios" value="1">$10</b-form-radio>
              <b-form-radio v-model="selectedRadio" name="some-radios" value="2">$10-$100</b-form-radio>
              <b-form-radio v-model="selectedRadio" name="some-radios" value="3">$100 - $500</b-form-radio>
              <b-form-radio v-model="selectedRadio" name="some-radios" value="4">$500</b-form-radio>
              <b-form-radio v-model="selectedRadio" name="some-radios" value="5">All</b-form-radio>
            </b-form-group>
          </div>
          <div class="separator"></div>
          <div class="d-flex flex-row justify-content-between">
            <div class="title mb-2">Slider</div>
            <div class="title mb-2">1.99 - 4098</div>
          </div>
          <div class="slidecontainer pb-2 elements">
            <input type="range" min="1" max="100" value="50" class="slider" id="myRange">
          </div>
          <div class="separator"></div>
          <div class="title">Category</div>
          <b-form-group class="elements mt-2" label="">
            <b-form-checkbox-group v-model="selected" plain stacked>
              <b-form-checkbox value="orange">Cell Phones<span>1920</span></b-form-checkbox>
              <b-form-checkbox value="apple">Computers & Tablet<span>1820</span></b-form-checkbox>
              <b-form-checkbox value="pineapple">Cell Phone Accessories<span>462</span></b-form-checkbox>
              <b-form-checkbox value="Appliances">Appliances<span>6556</span></b-form-checkbox>
              <b-form-checkbox value="Audio">Audio<span>120</span></b-form-checkbox>
              <b-form-checkbox value="iPhone Accessories">iPhone Accessories<span>353</span></b-form-checkbox>
              <b-form-checkbox value="Cameras & Camcorders">Cameras & Camcorders<span>45</span></b-form-checkbox>
              <b-form-checkbox value="iPhone Cases & Clips">iPhone Cases & Clips<span>456</span></b-form-checkbox>
              <b-form-checkbox value="TV & Home Theater">TV & Home Theater<span>55</span></b-form-checkbox>
              <b-form-checkbox value="Small Kitchen Appliances">Small Kitchen Appliances<span>10</span></b-form-checkbox>
            </b-form-checkbox-group>
          </b-form-group>
          <div class="separator"></div>
          <div class="title">Brand</div>
          <b-form-group class="mt-2 elements" label="">
            <b-form-checkbox-group v-model="selected" plain stacked>
              <b-form-checkbox value="orange">Insigni<span>220</span></b-form-checkbox>
              <b-form-checkbox value="apple">Samsung<span>120</span></b-form-checkbox>
              <b-form-checkbox value="pineapple">Apple<span>320</span></b-form-checkbox>
              <b-form-checkbox value="Appliances">HP<span>32</span></b-form-checkbox>
              <b-form-checkbox value="Audio">Sony<span>520</span></b-form-checkbox>
              <b-form-checkbox value="iPhone Accessories">Metra<span>55</span></b-form-checkbox>
              <b-form-checkbox value="Cameras & Camcorders">Dyne<span>120</span></b-form-checkbox>
              <b-form-checkbox value="iPhone Cases & Clips">LG<span>98</span></b-form-checkbox>
              <b-form-checkbox value="TV & Home Theater">Canon<span>99</span></b-form-checkbox>
              <b-form-checkbox value="Small Kitchen Appliances">Speck<span>575</span></b-form-checkbox>
            </b-form-checkbox-group>
          </b-form-group>
          <div class="separator"></div>
          <div class="title mb-4">Rating</div>
          <div class="elements">
            <div class="rating mt-2">
              <div class="stars d-flex justify-content-between">
                <div class="d-flex">
                  <span class="checked-star"></span>
                  <span class="checked-star"></span>
                  <span class="checked-star"></span>
                  <span class="checked-star"></span>
                  <span class="checked-star"></span>
                  <div class="up">& UP</div>
                </div>
                <div class="reference-number">525</div>
              </div>
            </div>
            <div class="rating mt-2">
              <div class="stars d-flex justify-content-between">
                <div class="d-flex">
                  <span class="star checked-star"></span>
                  <span class="star checked-star"></span>
                  <span class="star checked-star"></span>
                  <span class="checked-star"></span>
                  <span class="star"></span>
                  <div class="up">& UP</div>
                </div>
                <div class="reference-number">525</div>
              </div>
            </div>
            <div class="rating mt-2">
              <div class="stars d-flex justify-content-between">
                <div class="d-flex">
                  <span class="checked-star"></span>
                  <span class="checked-star"></span>
                  <span class="checked-star"></span>
                  <span class="star"></span>
                  <span class="star"></span>
                  <div class="up">& UP</div>
                </div>
                <div class="reference-number">525</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </b-modal>
  </div>
</template>

<script>
export default {
  name: "filters",
  data() {
    return {
      value: 5,
      selected: [],
      selectedRadio: 5
    }
  }
}
</script>

<style scoped lang="scss">
.card-filter {
  min-width: 292px;
}

.slidecontainer {
  width: 100%;
}

.reference-number {
  position: relative;
  top: -2px
}

.slider {
  -webkit-appearance: none;
  width: 100%;
  height: 6px;
  background: #d3d3d3;
  outline: none;
  opacity: 0.7;
  -webkit-transition: .2s;
  transition: opacity .2s;
}

.slider:hover {
  opacity: 1;
}

.slider::-webkit-slider-thumb {
  -webkit-appearance: none;
  appearance: none;
  width: 20px;
  height: 20px;
  background: #606060;
  cursor: pointer;
  border-radius: 30px;
}

.slider::-moz-range-thumb {
  border-radius: 30px;
  width: 20px;
  height: 20px;
  background: #606060;
  cursor: pointer;
}

.top-title.text-left {
  margin-bottom: 22px;
}
</style>
