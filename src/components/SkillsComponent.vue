<script setup></script>

<template>
  <div class="skills-container">
    <div class="main-skills">
      <div class="description">
        <h1>Main skills</h1>
        <p>
          I usually create modern and responsive interfaces using HTML, CSS, JavaScript, Vue.js,
          Tailwind CSS, Figma and sometimes Django for my design-to-code workflows.
        </p>
      </div>
      <div class="icons">
        <div class="icon">
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg"
          />
          <p class="text">HTML</p>
        </div>
        <div class="icon">
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg"
          />
          <p class="text">CSS</p>
        </div>
        <div class="icon">
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg"
          />
          <p class="text">JS</p>
        </div>
        <div class="icon">
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vuejs/vuejs-original.svg"
          />
          <p class="text">Vue</p>
        </div>
        <div class="icon">
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/tailwindcss/tailwindcss-original.svg"
          />
          <p class="text">Tailwind</p>
        </div>
        <div class="icon">
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/figma/figma-original.svg"
          />
          <p class="text">Figma</p>
        </div>
        <div class="icon">
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/django/django-plain.svg"
          />
          <p class="text">Django</p>
        </div>
        <div class="icon">
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/git/git-original.svg"
          />
          <p class="text">Git</p>
        </div>
      </div>
      <div class="svg-programmer">
        <img src="/code-thinking-svg.svg" alt="" />
      </div>
    </div>
    <div class="other-knowledge">
      <div class="svg-programmer">
        <img src="/developer-svg.svg" alt="" />
      </div>
      <div class="description other-knowledge-description">
        <h1>Other knowledge</h1>
        <p>
          Because of my classes and personal experience, I also have some other skills, both in and
          outside the programming world. After Effects, Photoshop and SQL are some examples.
        </p>
      </div>
      <div class="icons">
        <div class="icon">
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/photoshop/photoshop-original.svg"
          />
          <div class="text">Photoshop</div>
        </div>
        <div class="icon longer-icon">
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/aftereffects/aftereffects-plain.svg"
          />
          <div class="text">After Effects</div>
        </div>
        <div class="icon longer-icon">
          <img src="/davinci-icon.png" alt="" />
          <div class="text">Davinci Resolve</div>
        </div>
        <div class="icon">
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mysql/mysql-original.svg"
          />
          <div class="text">MySQL</div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.skills-container {
  display: flex;
  justify-content: space-between;
  padding: 150px;
  height: 80vh;
  background-color: var(--main-color);
}
.main-skills {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  height: 620px;
}
.main-skills > div:last-child {
  margin-top: auto;
}
.description {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  width: 400px;
  line-height: 1.4em;
}
h1 {
  color: #e1e1e1;
  border: 2px solid #1d1d1d;
  border-radius: 15px 15px 0;
  width: fit-content;
  padding: 1rem;
}
p {
  color: #ffff;
  font-weight: 300;
}
.icons {
  display: flex;
  margin: 1rem 0 0 -15px;
}
.icon {
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  position: relative;
  text-align: center;
  height: 70px;
  width: 65px;
  cursor: pointer;
}
.icon img {
  width: 40px;
  transition: 300ms all;
}
.icon:hover img {
  transform: translateY(-10px);
}
.longer-icon:hover img {
  transform: translateY(-15px);
}
.icon:hover .text {
  transform: translate(-50%, 0);
  opacity: 1;
}
.text {
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translate(-50%, 100%);
  opacity: 0;
  transition:
    transform 0.3s ease-in-out,
    opacity 0.3s;
  color: #fff;
  padding: 5px 10px 0 10px;
  font-weight: 500;
  font-size: 12px;
}
.other-knowledge {
  display: flex;
  flex-direction: column;
  align-items: start;
  height: 620px;
}
.svg-programmer img {
  width: 420px;
}
.other-knowledge-description {
  margin-top: 60px;
}
</style>
