<template>
  <div style="margin-bottom: 80px;">
    <h1 style="font-size: xxx-large">Hello!</h1>

    <div class="paragraph">
      <div>
        I'm <strong style="font-size: x-large">Harsh Rao</strong> a slightly off-kilter Game, App & Web developer. I love discussing, designing and developing apps, websites and games in general.<br/>
      </div>

      <div style="margin-top: 20px;">I've worked on  <router-link to="/other-projects">Apps </router-link>and on <router-link to="/game-projects">Games</router-link> (either to release them, to showcase my capabilities, or just to play around), and enjoyed some <router-link to="/resume">tech stacks</router-link> at a few places.</div>

      <div style="margin-top: 40px;">If i'm not busy crafting their next masterpiece, you can find me chugging coffee and scouring the internet for the memes. You can reach me at <a href="mailto:hurshrao@gmail.com">hurshrao@gmail.com</a> or through <router-link to="/contact">here</router-link>.</div>
    </div>

    <div class="photo">
      <img src="img/avatar-tiffany.png" alt="Avatar" />
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