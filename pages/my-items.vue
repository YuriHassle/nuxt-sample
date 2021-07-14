<template>
  <div class="container">
    <MyItem v-for="item in myItems" :key="item.id" :item="item" />
  </div>
</template>

<script>
export default {
  layout: "no-nav",
  data() {
    return {
      myItems: this.$store.state.myRentals
    };
  }
};
</script>

<style scoped></style>
