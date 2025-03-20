<script setup>
const navName = '<João/>'
</script>

<template>
  <div class="container">
    <div class="nav-container">
      <a class="name">{{ navName }}</a>
      <a href="" class="nav-item">Skills</a>
      <a href="" class="nav-item">Projects</a>
      <a href="" class="nav-item">About</a>
    </div>
  </div>
</template>

<style scoped>
.nav-container {
  display: flex;
  justify-content: space-between;
  width: 100%;
  flex-direction: row;
  gap: 2rem;
}

.name {
  cursor: pointer;
}

.nav-container > a:first-child {
  margin-right: auto;
}

.nav-container a {
  text-decoration: none;
  color: #000;
}

.nav-item {
  width: 150px;
  height: 30px;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  overflow: hidden;
  border-radius: 15px;
  transition: all 0.5s ease;
}

.nav-item::before {
  content: '';
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: linear-gradient(0deg, transparent, transparent 30%, var(--main-color));
  transform: rotate(-45deg);
  transition: all 0.5s ease;
  opacity: 0;
}

.nav-item:hover {
  transform: scale(1.05);
  box-shadow: #7b8ba54e 0px 2px 8px 0px;
}

.nav-item:hover::before {
  opacity: 1;
  transform: rotate(-45deg) translateY(100%);
}
</style>
