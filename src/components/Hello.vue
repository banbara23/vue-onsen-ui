<template>
  <v-ons-page>
    <v-ons-toolbar>
      <div class="center"> Title </div>
    </v-ons-toolbar>
    <p style="text-align: center">
      <v-ons-button @click="notification">Click</v-ons-button>
    </p>
  </v-ons-page>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  methods: {
    notification: function (event) {
      console.log('Hello World!')
      // $notification.alert('Hello World!') // '$notification' is not defined
      alert('Hello World!')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
