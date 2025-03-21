<script setup>
import ProfileComponent from '@/components/ProfileComponent.vue'
import ProfilePicture from '@/components/ProfilePicture.vue'
import ProjectsComponent from '@/components/ProjectsComponent.vue'
import SkillsComponent from '@/components/SkillsComponent.vue'
</script>

<template>
  <div class="container">
    <main class="main">
      <div class="profile-wrapper">
        <ProfileComponent />
        <ProfilePicture class="profile-picture" />
      </div>
      <div class="arrow-down">
        <router-link to="#skills"><img src="/seta-para-baixo.svg" alt="" /></router-link>
      </div>
    </main>
    <div class="skills" id="skills">
      <SkillsComponent />
    </div>
    <div class="projects" id="projects">
      <ProjectsComponent />
    </div>
  </div>
</template>

<style scoped>
.main {
  padding: 50px 150px 0 150px;
  height: 100vh;
}
.profile-wrapper {
  height: 500px;
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
  position: absolute;
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
