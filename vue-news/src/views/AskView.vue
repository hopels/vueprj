<template>
  <div>
    <div v-for="item in this.$store.state.ask">{{ item.title }}</div>
  </div>
</template>

<script>
export default {
  created() {
    this.$store.dispatch("FETCH_ASK");
    // var vm = this;
    // fetchAskList()
    //   .then(function (response) {
    //     vm.ask = response.data;
    //   })
    //   .catch(function (error) {
    //     console.log(error);
    //   });
  },
};
</script>

<style></style>
