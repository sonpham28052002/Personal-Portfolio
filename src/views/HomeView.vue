<template>
  <div class="home">
    <div data-aos="zoom-in-right" class="content">
      <h1>Hi, It's <span>PHẠM THANH SƠN</span></h1>
      <h2>You can call me Leon</h2>
      <h3>I'm A <span class="text-animation"></span></h3>
      <p class="summary">
        My name is Loen, I'm a software engineer with a passion for web development. I have
        experience in building web applications using modern technologies. I'm always looking for
        new challenges and opportunities to learn and grow.
      </p>
      <div class="contacts">
        <a href="https://github.com/sonpham28052002" target="_blank"
          ><font-awesome-icon class="icon" :icon="['fab', 'github']"
        /></a>
        <a href="https://www.facebook.com/loenz.2805" target="_blank"
          ><font-awesome-icon class="icon" :icon="['fab', 'facebook']"
        /></a>
        <a href="https://www.instagram.com/loenz.2805/" target="_blank"
          ><font-awesome-icon class="icon" :icon="['fab', 'instagram']"
        /></a>
      </div>
      <div class="btns">
        <button class="btn-hire btn-hover btn-active">HIRE</button>
        <a
          href="https://drive.google.com/uc?export=download&id=1GGr9JuJR15aYel03IKAijADWPTzYnUxb"
          target="_blank"
          ><button class="btn-cv btn-hover btn-active">DOWNLOAD CV</button></a
        >
      </div>
    </div>
    <div
      data-aos="fade-down"
      data-aos-delay="300"
      class="content-image"
    >
      <img src="../assets/DSC_7498-min.jpg" />
    </div>
  </div>
</template>
<style scoped>
@import url('../styles/HomeStyle/HomeStyle.css');
@import url('../styles/HomeStyle/HomeSlyteResponsive.css');
</style>
<script setup>
import AOS from 'aos'
import { onMounted } from 'vue'

onMounted(() => {
  AOS.init()
})
</script>
