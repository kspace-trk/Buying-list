<template>
  <div class="container">
    <div class="header">
      <buyingListHeader />
    </div>
    <div class="contents">
    <contents />
    </div>
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

<style scoped>
.header {
  width: 100%;
  display: flex;
  position: fixed;
}
.contents {
  padding-top: 50px;
}
</style>
