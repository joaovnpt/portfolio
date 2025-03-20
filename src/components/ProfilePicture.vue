<script setup></script>

<template>
  <div class="profile-container">
    <img src="../../public/pfp sem fndo.png" alt="" />
  </div>
  <div class="pfp-effect">
    <img src="../../public/pfp fx.png" alt="" />
  </div>
</template>

<style scoped>
.profile-container {
  position: relative;
  width: fit-content;
  height: fit-content;
  border: 1px solid #000;
  border-radius: 100%;
}
.profile-container img {
  display: block;
  width: 350px;
  height: 350px;
  border-radius: 100%;
}
.pfp-effect {
  position: absolute;
  top: 0;
  right: 0;
  width: fit-content;
  height: fit-content;
  z-index: -1;
}
.pfp-effect img {
  width: 580px;
}
</style>
