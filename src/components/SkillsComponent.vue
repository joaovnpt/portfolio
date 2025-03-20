<script setup></script>

<template>
  <div class="container">
    <div class="main-skills">
      <div class="description">
        <h1>Main skills</h1>
        <p>
          I usually create modern and responsive interfaces using HTML, CSS, JavaScript, Vue.js,
          Tailwind CSS, Figma and sometimes Django for my design-to-code workflows.
        </p>
      </div>
      <div class="icons">
        <img
          src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg"
        />
        <img
          src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg"
        />
        <img
          src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg"
        />
        <img
          src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vuejs/vuejs-original.svg"
        />
        <img
          src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/tailwindcss/tailwindcss-original.svg"
        />
        <img
          src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/figma/figma-original.svg"
        />
        <img
          src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/django/django-plain.svg"
        />
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/git/git-original.svg" />
      </div>
    </div>
    <div class="other-knowledge"></div>
  </div>
</template>

<style scoped>
.container {
  padding: 150px;
  height: 100vh;
  background-color: var(--main-color);
  overflow: hidden;
}
.description {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  width: 400px;
  line-height: 1.4em;
}
h1 {
  color: var(--main-text-color);
}
p {
  color: #ffff;
  font-weight: 300;
}
.icons {
  display: flex;
  margin-top: 2rem;
  gap: 0.8rem;
}
.icons img {
  width: 40px;
  transition: 300ms all;
}
.icons img:hover {
    transform: translateY(-20px);
}
</style>
