<template>
  <div id="app">
    <div id="nav" >
        <HeaderView class="mb-3"></HeaderView>
    </div>
    <router-view/>
  </div>
</template>

<script lang="ts">
import HeaderView from './components/HeaderView.vue'

export default {
  components: {
    HeaderView,
  }
}
</script>
