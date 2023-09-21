<template>
  <div class="about">
    <h1 class="main-text">Your messeage has been sent!</h1>
    <button class="send_button" @click="goBack">Go Back</button>
  </div>
</template>

<script>
export default{
  name:"ContactView",
  methods:{
    goBack() {
      this.$router.go(-1);
    }
  }
}
</script>

<style>

.about{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  height: 100vh;
}
.main-text{
  font-size: 30pt;
  color: #263228;
  display: flex;
}
</style>
