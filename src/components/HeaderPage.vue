<template>
  <div class="container">
    <div class="logo">
      <img src="../assets/images/logo.svg" alt="" />
    </div>
    <nav class="links">
      <button class="buger-button" @click="toggleMenu = !toggleMenu">
        <img src="../assets/images/icon-hamburger.svg" alt="" />
      </button>
      <ul :class="{ hide: toggleMenu }">
        <li><a href="#about">About</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact" class="active">Contact</a></li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  data() {
    return {
      toggleMenu: true,
    };
  },
};
</script>
