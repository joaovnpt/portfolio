<script setup>
import ProfileComponent from '@/components/ProfileComponent.vue'
import ProfilePicture from '@/components/ProfilePicture.vue'
</script>

<template>
  <main class="main">
    <ProfileComponent />
    <ProfilePicture class="profile-picture" />
  </main>
  <div class="arrow-down"><img src="../assets/seta-para-baixo.svg" alt="" /></div>
</template>

<style scoped>
.main {
  padding: 50px 150px 150px 150px;
  height: 400px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}
.profile-picture {
  margin-top: 50px;
}
.arrow-down {
  color: var(--main-color);
  display: flex;
  justify-content: center;
  align-items: center;
  position: fixed;
  top: 90%;
  left: 50%;
  transform: translate(-50%, -50%);
  transition: all 200ms;
  cursor: pointer;
}
.arrow-down img {
  width: 50px;
}
.arrow-down:hover {
  transform: translate(-50%, -50%) scale(1.1);
}
</style>
