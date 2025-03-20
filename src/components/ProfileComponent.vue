<script setup></script>

<template>
  <div class="profile-container">
    <h1 class="presentation">Hi, I'm João</h1>
    <h2>Student and developer</h2>
    <p>I create solid prototypes and websites with great user experiences.</p>
    <div class="more-about squishy-classic">
      <a href="/">More about me</a>
      <svg
        width="24"
        height="24"
        viewBox="0 0 24 24"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M23.0677 11.9929L18.818 7.75739L17.4061 9.17398L19.2415 11.0032L0.932469 11.0012L0.932251 13.0012L19.2369 13.0032L17.4155 14.8308L18.8321 16.2426L23.0677 11.9929Z"
          fill="currentColor"
        />
      </svg>
    </div>
  </div>
</template>

<style scoped>
.profile-container {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
  width: 400px;
}

.more-about {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0.5rem;
  width: 200px;
  height: 50px;
  border: 1px solid black;
  margin-top: 1rem;
  transition: all 250ms;
  cursor: pointer;
}

.squishy-classic {
  background-color: #f0f0f0;
  color: #242424;
  border-radius: 0.5rem;
  box-shadow:
    inset 0 1px 0 0 #f4f4f4,
    0 1px 0 0 #efefef,
    0 2px 0 0 #ececec,
    0 4px 0 0 #e0e0e0,
    0 5px 0 0 #dedede,
    0 6px 0 0 #dcdcdc,
    0 7px 0 0 #cacaca,
    0 7px 8px 0 #cecece;
}

.squishy-classic:hover {
  transform: translateY(4px);
  box-shadow:
    inset 0 1px 0 0 #f4f4f4,
    0 1px 0 0 #efefef,
    0 1px 0 0 #ececec,
    0 2px 0 0 #e0e0e0,
    0 2px 0 0 #dedede,
    0 3px 0 0 #dcdcdc,
    0 4px 0 0 #cacaca,
    0 4px 6px 0 #cecece;
}

.squishy-classic:active {
  transform: translateY(6px);
  box-shadow:
    inset 0 1px 0 0 #f4f4f4,
    0 1px 0 0 #efefef,
    0 1px 0 0 #ececec,
    0 1px 0 0 #e0e0e0,
    0 1px 0 0 #dedede,
    0 2px 0 0 #dcdcdc,
    0 2px 0 0 #cacaca,
    0 2px 4px 0 #cecece;
}

.more-about a {
  text-decoration: none;
  color: #000;
}
</style>
