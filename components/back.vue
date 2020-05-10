<template>
  <div>
    <nuxt-link to="/" tag="div" class="container">
      <button class="contents">
        <p>戻 る</p>
      </button>
    </nuxt-link>
  </div>
</template>
<style scoped>
.container {
  height: 60px;
  width: 100%;
  background-color: #d7d7d7;
  justify-content: center;
  align-items: center;
  display: flex;
}
.contents {
  width: 90%;
  height: 50px;
  background-color: #f45727d6;
  justify-content: center;
  align-items: center;
  display: flex;
  border-radius: 10px;
}
.contents p {
  font-size: 1.4rem;
  font-weight: 900;
  color: #f7f7f7;
}
</style>