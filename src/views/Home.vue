<template>
  <play-list />
</template>

<script lang="ts">
  import Vue from 'vue'
  import PlayList from '../components/PlayList.vue'

  export default Vue.extend({
    name: 'Home',

    components: {
      PlayList,
    },
  })
</script>
