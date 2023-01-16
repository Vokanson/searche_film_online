<template>
  <div class="v-list">
  <p>List</p>
    <filmCart/>
  </div>

</template>

<script>
import filmCart from './filmCart.vue'
export default {
  name: "v-list",
  components: {
    filmCart
  },

  props:{},
  data() {
    return{}

  }


}
</script>

<style lang="scss">
.v-list {
  &list {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
  }
}
</style>