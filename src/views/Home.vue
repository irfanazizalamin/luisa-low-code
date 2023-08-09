<template>
  <div class="home">
    <Luisa :design="design" v-model="viewModel" :config="config" />
  </div>
</template>
<style lang="scss"></style>

<script>
import Vue from "vue";
import Luisa from 'luisa-vue'
Vue.use(Luisa);

import '@mdi/font/css/materialdesignicons.css'

// import app from './app.json'

export default {
  name: 'Home',
  data: function () {
    return {
      design: {
        figmaFile: "fMHTms1d2sWFy72lL5Gw1T",
        figmaAccessKey: "figd_tlYXNXnLFJ7ylOG7Idrwtcn6x9ZCEDv5p-lxI3qZ"

  },
  viewModel: {
    name: '',
    result: ''
  },
  config: {
  }
}
  },
components: {
},
methods: {
  sayHello() {
    this.viewModel.result = "Hello " + this.viewModel.name
  }
}
}
</script>
