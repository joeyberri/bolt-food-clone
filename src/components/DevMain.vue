<template>
  <main class="content-wrap">
    <header class="content-head">
      <h1 class="is-blue">Foods available</h1>

      <div class="action">
        <button>Save search</button>
      </div>
    </header>

    <div class="content">
      <section class="food-boxes">
        <FoodBox
          :dishes="dish"
          v-for="dish in dishes"
          :key="dish.id"
          class="food-box"
        />
      </section>
    </div>
  </main>
</template>

<script>
import FoodBox from "./FoodBox.vue";

export default {
  name: "DevMain",
  components: { FoodBox },

  props: ["dishes"],
};
</script>
