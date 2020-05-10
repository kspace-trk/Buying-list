<template>
  <div>
    <div class="container">
      <input class="name" placeholder="買ってきて欲しいもの" />
    </div>
  </div>
</template>
<style scoped>
.container {
  display: flex;
  justify-content: center;
}
.name {
  width: 90%;
  height: 3.5rem;
  background-color: #ffffff;
  margin-top: 130px;
  padding-left: 1rem;
  border-radius: 10px;
  font-size: 1.5rem;
  font-weight: 600;
  border: 2px solid #d7d7d7;
  color: #404040;
}
::placeholder {
  color: #b0b0b0;
}
</style>