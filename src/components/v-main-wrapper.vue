<template>
  <div class="v-main-wrapper">
    <h1>{{title}}</h1>
    <vList/>
    <v-favourites/>

  </div>
</template>

<script>
import vList from './v-list.vue'
import vFavourites from './v-favourites.vue'
export default {
  name: "v-main-wrapper",
  components: {
    vList,
    vFavourites,
  },
  props: {},
  data() {
    return {
      title: 'Поиск фильма по названию'
    }
  }

}
</script>

<style>
.v-main-wrapper {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  max-width: 900px;
  margin: 0 auto;
}
</style>