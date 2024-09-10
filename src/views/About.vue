<template>
  <div style="margin-bottom: 80px;">
    <h1 style="font-size: xxx-large">Hello!</h1>

    <div class="paragraph">
<!--      <div>-->
<!--        I'm <strong style="font-size: x-large">Harsh Rao</strong>, a computer science student who enjoys designing and developing apps and games.<br/>-->
<!--      </div>-->

<!--      <div style="margin-top: 20px;">I've created and contributed heavily to <router-link to="/other-projects">Apps </router-link>and <router-link to="/game-projects">Games</router-link> and worked with Unity and other tech <stacks>  </stacks>.</div>-->

<!--      <div style="margin-top: 40px;">If I'm not busy crafting my next masterpiece, you can find me chugging coffee and scouring the internet for the memes. You can reach me at <a href="mailto:hurshrao@gmail.com">hurshrao@gmail.com</a> or through <router-link to="/contact">here</router-link>.</div>-->

      <h2 style="line-height: 2">I'm <strong>Harsh Rao</strong>, a passionate game and app developer.<br> I thrive on creating innovative solutions that enhance the gaming experience, blending my technical skills with a deep love for game design.</h2>
    </div>

    <div class="photo">
      <img src="img/avatar.png" alt="Avatar" />
    </div>

    <div style="clear:both"></div>

  </div>
</template>

<style scoped>
.paragraph {
  max-width: 700px;
  margin-bottom: 20px;
}

.photo {
  margin-top: 50px;
  text-align: center;
}

@media only screen and (min-width: 620px){
  .paragraph {
    float: left;
  }

  .photo {
    float: left;
    padding: 10px;
    padding-left: 80px;
  }
}

</style>