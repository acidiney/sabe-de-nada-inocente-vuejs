<template>
  <!-- div id="app">
    <img src="./assets/sabe.png" alt="monkey" width="400" />
    <app-screen />
  </div -->

  <div>
    <h2> Olá, <span>{{ greetings }} </span></h2>
    <p> <small>@GDGDevFest 2018</small></p>
  </div>
</template>

<script>
import AppScreen from "./components/AppScreen.vue";

export default {
  name: "app",
  components: {
    "app-screen": AppScreen
  },
  created: function() {
    document.title = "DevFest Example";
  },
  data: function() {
    return {
      greetings: "Acidiney Dias"
    };
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #363636 !important;
  padding: 5pc;
}

div {
  padding: 5pc;
  padding-top: 18%;
  text-align: center;
}
h2 {
  font-size: 48pt !important;
  font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS", sans-serif;
}

span {
  color: rgb(0, 128, 198);
}
</style>
