<template>
  <div>
    <!--<input v-on:input="onInput" />-->
    <input @input="onInput" />
  </div>
</template>

<script>
export default {
  name: "SearchBar",
  methods: {
    onInput: function(event) {
      //给App.vue传数据
      this.$emit("termChange", event.target.value);
    }
  }
};
</script>

<style scoped>
input {
  width: 75%;
}
div {
  text-align: center;
  margin: 20px;
}
</style>
