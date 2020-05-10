<template>
  <div class="container">
    <div class="header">
      <buyingListHeader />
    </div>
    <div class="descript">
      <buyingListDescript />
    </div>
    <div class="footer">
      <buyingListBackFooter />
    </div>
  </div>
</template>
<script>
import buyingListHeader from "~/components/header.vue";
import buyingListBackFooter from "~/components/back.vue";
import buyingListDescript from "~/components/descript.vue";
export default {
  components: {
    buyingListHeader,
    buyingListBackFooter,
    buyingListDescript
  }
};
</script>
<style scoped>
.header {
  width: 100%;
  display: flex;
  position: fixed;
  justify-content: center;
  background-color: #404040;
}
.footer {
  width: 100%;
  position: fixed;
  top: calc(100vh - 60px); /*calc(100vh - フッターの高さpx)*/
  z-index: 10;
}
</style>