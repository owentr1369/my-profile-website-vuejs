<template>
  <div class="profile-wrap">
    <div class="profile-left">
      <div class="avt">
        <img src="../assets/avt.jpg" alt="" />
      </div>
      <div class="name">
        <h2>Tran Tam</h2>
      </div>
      <h3>Frontend Developer</h3>
      <div class="social-media">
        <div>
          <a class="svg-icon" href="#"> <youTube /> </a>
        </div>
        <div>
          <a class="svg-icon" href="#"> <twitter /> </a>
        </div>
        <div>
          <a class="svg-icon" href="#"> <instagram /> </a>
        </div>
        <div>
          <a class="svg-icon" href="#"> <linkedin /> </a>
        </div>
      </div>
    </div>
    <div class="profile-right">
      <h1>Hello</h1>
      <h2>Here's who I am and what I do</h2>
      <div class="profile-button">
        <button>Resume</button>
        <button>Projects</button>
      </div>
      <p>
        Hi! I am passionate about technology, innovation and big challenging
        tasks on my to do list.
        <br />
        I am a novice developer with eager-to-learn attitude. I want to become a
        Front-End Developer with ability to collaborate effectively with
        developers and enrich my technical skills by building awesome projects.
        <br />
        With a passion for both personal growth and for software development, I
        want to have ability to create webapp and mobile app with stunning UI
        and greate UX.
      </p>
    </div>
  </div>
</template>

<script>
import youTube from "../assets/Icons/youtube-brands.svg";
import twitter from "../assets/Icons/twitter-brands.svg";
import instagram from "../assets/Icons/instagram-brands.svg";
import linkedin from "../assets/Icons/linkedin-brands.svg";
export default {
  components: {
    youTube,
    twitter,
    instagram,
    linkedin,
  },
};
</script>

<style lang="scss" scoped>
</style>