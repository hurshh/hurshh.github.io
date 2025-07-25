<template>
  <div style="margin-bottom: 80px;">
    <h1 style="font-size: xxx-large; margin-bottom: 30px;">Hello!</h1>

    <div class="content-wrapper">
      <div class="paragraph">
        <h2 style="line-height: 2; margin-top: 0;">I'm <strong>Harsh Rao</strong>, a passionate game and app developer.<br> I thrive on creating innovative solutions that enhance the gaming experience, blending my technical skills with a deep love for game design.</h2>
      </div>

      <div class="photo">
        <img src="img/avv.png" alt="Avatar" class="profile-image" />
      </div>

      <div style="clear:both"></div>
    </div>
  </div>
</template>

<style scoped>
.content-wrapper {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  gap: 40px;
  margin-top: 0;
}

.paragraph {
  max-width: 700px;
  margin-bottom: 20px;
  flex: 1;
  min-width: 300px;
}

.photo {
  text-align: center;
  margin: 0;
}

.profile-image {
  width: 300px;
  height: 300px;
  transition: all 0.3s ease;
  border-radius: 5px;
}

@media only screen and (max-width: 620px) {
  .content-wrapper {
    flex-direction: column;
    align-items: center;
    gap: 20px;
  }

  .paragraph {
    text-align: center;
    margin-bottom: 0;
  }

  .profile-image {
    width: 280px;
    height: 280px;
  }
}

@media only screen and (min-width: 620px) {
  .paragraph {
    margin-bottom: 0;
  }

  .photo {
    padding: 0;
  }
}

@media only screen and (min-width: 1200px) {
  .profile-image {
    width: 320px;
    height: 320px;
  }
}
</style>