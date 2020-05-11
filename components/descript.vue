<template>
  <div>
    <div class="container">
      <input class="name" placeholder="買ってきて欲しいもの" />
      <textarea class="descript" placeholder="どんなやつ？" />
      <div class="who-name">
        <p>だれ？：{{nakao}}</p>
        <div class="who-wrapper">
          <button v-on:click="muneki" class="who">むねき</button>
          <button v-on:click="makiko" class="who">まきこ</button>
          <button v-on:click="akari" class="who">あかり</button>
          <button v-on:click="keigo" class="who">けいご</button>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      nakao: ""
    };
  },
  methods: {
    muneki: function() {
      this.nakao = "むねき";
    },
    makiko: function() {
      this.nakao = "まきこ";
    },
    akari: function() {
      this.nakao = "あかり";
    },
    keigo: function() {
      this.nakao = "けいご";
    }
  }
};
</script>
<style scoped>
.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.name {
  width: 90%;
  height: 3.5rem;
  background-color: #ffffff;
  margin-top: 80px;
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
.descript {
  width: 90%;
  height: 20rem;
  background-color: #ffffff;
  margin-top: 2rem;
  padding-left: 1rem;
  border-radius: 10px;
  font-size: 1.5rem;
  font-weight: 600;
  border: 2px solid #d7d7d7;
  color: #404040;
}
.who-wrapper {
  display: flex;
  padding-top: 0.5rem;
}
.who {
  width: 5.2rem;
  height: 4rem;
  border-radius: 10px;
  background-color: #ffffff;
  border: 2px solid #d7d7d7;
}
.who-name p {
  font-size: 1.3rem;
  font-weight: 700;
  color: #707070;
}
</style>