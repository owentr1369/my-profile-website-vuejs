<template>
  <div class="parallax-wrapper">
    <section>
      <img src="../assets/images/stars.png" id="stars" alt="" />
      <img src="../assets/images/moon.png" id="moon" alt="" />
      <img
        src="../assets/images/mountains_behind.png"
        id="mountains_behind"
        alt=""
      />
      <h2 id="text">Moon Light</h2>
      <a href="#sec" id="btn">Explore</a>
      <img
        src="../assets/images/mountains_front.png"
        id="mountains_front"
        alt=""
      />
    </section>
    <div class="sec" id="sec">
      <h2>Parallax Scrolling Effect</h2>
      <p>
        I Don't Get 'Over' things, I Get 'Through' them. There's a difference.
        It'sI didn't say it was your fault, I said I was blaming you. Don't Get
        'Over' things, I Get 'Through' them. There's a difference. It'sI didn't
        say it was your fault, I said I was blaming you. Don't Get 'Over'
        things, I Get 'Through' them. There's a difference. It'sI didn't say it
        was your fault, I said I was blaming you. I Don't Get 'Over' things, I
        Get 'Through' them. There's a difference. It'sI didn't say it was your
        fault, I said I was blaming you. Don't Get 'Over' things, I Get
        'Through' them. There's a difference. It'sI didn't say it was your
        fault, I said I was blaming you. Don't Get 'Over' things, I Get
        'Through' them. There's a difference. It'sI didn't say it was your
        fault, I said I was blaming you.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "ParallaxScroller",
};
</script>

<style lang="scss" scoped>
@import url("https://fonts.googleapis.com/css2?family=Montserrat&family=Source+Sans+Pro&family=Source+Serif+Pro:wght@200&display=swap");

body {
  min-height: 100vh;
  background: linear-gradient(#2b1055, #7597de);
  overflow-x: hidden;
}

section {
  position: relative;
  width: 100%;
  height: 100vh;
  padding: 100px;
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden;
}
section::before {
  content: "";
  position: absolute;
  bottom: 0;
  width: 100%;
  height: 100px;
  background: linear-gradient(to top, #1c0522, transparent);
  z-index: 1000;
}
section img {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  pointer-events: none;
}

section img#moon {
  mix-blend-mode: screen;
}

section img#mountains_front {
  z-index: 10;
}

#text {
  position: absolute;
  right: -350px;
  color: #fff;
  white-space: nowrap;
  font-size: 7.5vw;
  z-index: 9;
}

#btn {
  text-decoration: none;
  display: inline-block;
  padding: 8px 30px;
  border-radius: 40px;
  background: #fff;
  color: #2b1055;
  font-size: 1.5em;
  z-index: 9;
  transform: translateY(100px);
}
.sec {
  position: relative;
  padding: 100px;
  background-color: #1c0522;
}
.sec h2 {
  font-size: 3.5rem;
  margin-bottom: 10px;
  color: #fff;
}
.sec p {
  font-size: 1.2em;
  color: #fff;
}
</style>