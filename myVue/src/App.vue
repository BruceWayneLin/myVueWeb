<template>
  <div id="app">
   <div class="container">
      <div class="row">
       <div id="content" class="col-lg-12 text-center" v-on:click="toSlideDiv">
       </div>
      </div>
   </div>
    <hello>
    </hello>  
  </div>
</template>

<script>
import hello from './components/hello'
import 'jquery/dist/jquery.js'
import $ from 'jquery'
import 'bootstrap/dist/css/bootstrap.css'

export default {
  name: 'app',
  mounted () {
    $('#content').append('<h1>hello</h1>')
  },
  methods: {
    toSlideDiv: function () {
      $('#content').addClass('animated bounceIn')
    }
  },
  components: {
    hello
  }
}
</script>

<style>

</style>
