<template>
  <div>
    <div v-for="user in this.$store.state.news">{{ user.title }}</div>
  </div>
</template>

<script>
export default {
  created() {
    this.$store.dispatch("FETCH_NEWS");

    // fetchNewsList()
    //   .then((response) => {
    //     console.log("호출 후 : ", this);
    //     this.users = response.data;
    //   })
    //   .catch(function (error) {
    //     console.log(error);
    //   });
  },
};
</script>

<style></style>
