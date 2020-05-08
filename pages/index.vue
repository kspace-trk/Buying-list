<template>
  <div class="container">
    <buyingListHeader />
    <contents />
  </div>
</template>

<script>
import buyingListHeader from "~/components/header.vue";
import contents from "~/components/contents.vue";

export default {
  components: {
    buyingListHeader,
    contents
  }
};
</script>

<style>
</style>
