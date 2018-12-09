<template>
  <div class="container">
    <h3 class="is-size-4"> Bem vindo ao Jogo,</h3>
    <small> Começa a jogar agora</small>
    <div class="panel">
      <div class="panel-heading">
        Escolha o menu 😀
      </div>
      <div class="panel-block">
        <div class="container columns">
          <app-menu v-bind:items="menuItems['first']" />
          <app-menu v-bind:items="menuItems['second']"/>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
.panel {
  width: 450px;
  margin: 0 auto;
}
</style>
<script>
import Menu from "./articles/Menu.vue";
export default {
  name: "AppScreen",
  components: {
    "app-menu": Menu
  },
  data: function() {
    return {
      menuItems: {
        first: [
          {
            name: "Jogar",
            action: "play"
          },
          {
            name: "Pontuações",
            action: "ranking"
          }
        ],
        second: [
          {
            name: "Sugerir algo",
            action: "suggestion"
          },
          {
            name: "Compartilhar",
            action: "share"
          }
        ]
      }
    };
  }
};
</script>
