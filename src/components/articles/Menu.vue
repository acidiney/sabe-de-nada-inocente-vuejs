<template>
  <div class="column">
    <ul> 
      <li v-for="(item, index) in items"
        v-bind:key="index">
        <button class="button is-white is-fullwidth">
        {{ item.name }}
        </button>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  props: ["items"],
  name: "Menu"
};
</script>
<style scoped>
button {
  color: #363636 !important;
  margin-bottom: 10px;
}
</style>
