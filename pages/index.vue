<template>
  <div class="container">
    <div class="header">
      <buyingListHeader />
    </div>
    <div class="contents">
      <contents />
    </div>
    <div class="footer">
      <buyingListFooter />
    </div>
  </div>
</template>

<script>
import buyingListHeader from "~/components/header.vue";
import contents from "~/components/contents.vue";
import buyingListFooter from "~/components/footer.vue";

export default {
  components: {
    buyingListHeader,
    contents,
    buyingListFooter
  }
};
</script>

<style scoped>
.header {
  width: 100%;
  display: flex;
  position: fixed;
  justify-content: center;
  background-color: #404040c9;
}
.contents {
  padding: 40px 0 100px;
}
.footer {
  width: 100%;
  position: fixed;
  top: calc(100vh - 60px); /*calc(100vh - フッターの高さpx)*/
  z-index: 10;
}
</style>
