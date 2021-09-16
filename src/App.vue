<template>
  <div id="app">
    <lingallery :addons="{ enableLargeView: true }" :iid.sync="currentId" :width="width" :height="height" :items="[
    {id:'someid1', src: 'https://picsum.photos/600/400/?image=0', thumbnail: 'https://picsum.photos/64/64/?image=0', alt: 'Some alt text'},
    {id:'someid2', src: 'https://picsum.photos/600/400/?image=10', thumbnail: 'https://picsum.photos/64/64/?image=10', alt: 'Another alt text'},
    {id:'someid3', src: 'https://picsum.photos/400/600/?image=20', thumbnail: 'https://picsum.photos/64/64/?image=20'},
]"/>
        </div>

</template>

<script>
import Lingallery from './components/Lingallery.vue'

export default {
  name: 'App',
  components: {
    Lingallery
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
