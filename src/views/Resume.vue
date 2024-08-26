<template>
  <div>
    <h1>Resume</h1>

    <div class="paragraph">
      I'm <strong>Harsh Rao</strong>, a versatile developer and designer with a passion for app, game and web development and web design, I am eager to explore new opportunities through internships and collaboration with like-minded professionals, including hackathons and competitions.
      <br />
      <br />I am currently seeking internship opportunities where I can further develop my skills and gain valuable real-world experience. I am also open to collaborating with others on projects, whether it's a hackathon, competition, or simply working together on a freelance basis. My passion for technology and design drives me to continually improve and explore new possibilities, and I look forward to contributing my expertise to new and exciting projects. If you have any opportunity feel free to
      <router-link to="/contact">contact me</router-link>.
      <br />
      <br />Besides development, I'm passionate about skateboarding, basketball, anime, gym and food.

      <div style="margin-top:20px; margin-bottom:20px;">
        <a class="download-link" href="d/Harsh_Resume.pdf" target="_blank"><i class="fa fa-download fa-lg fa-fw"></i> Download as PDF</a>
        <div style="clear:both"></div>
      </div>
    </div>
    <div class="photo">
      <img src="img/resume-photo.png" alt="Photo of John" />
    </div>

    <div style="clear:both"></div>

    <div class="full-content">

      <h2>Work experience</h2>


      <h3>Creatosaurus</h3>
      <h4>01/2024-06/2024</h4>
      <br>
      <div>
        <ul>
          <li>Analyzed various open-source image generation model like Stable Diffusion, Craiyon and Invoke.</li>
          <li>Conducted data prepossessing, cleaning, and filtering for creating checkpoints for Stable Diffusion model.</li>
          <li>Deployed a Stable Diffusion model on SageMaker and created API endpoints using FastAPI.</li>
          <li>Prepared user flows, wireframes, prototypes, and design mockups to visualize and iterate on user interface designs of the mobile app.</li>
          <li>Integrated and tested API into prototype mobile app</li>
        </ul>
      </div>
      <br>

      <h3>JIO india</h3>
      <h4>05/2023-07/2023</h4>
      <br>
      <div>
        <ul>
          <li>Led migration from legacy JSP pages to React. </li>
          <li>Implemented RESTful APIs in Spring Boot.</li>
          <li>Reduced page load times by over 30% through efficient component-based architecture.</li>
          <li>Coordinated with cross-functional teams to ensure smooth deployment and integration of new technologies.</li>
        </ul>
      </div>
      <br>





      <h2>Skills</h2>

      <div class="skill-set">
        <h3>Tech</h3>
        <SkillRate name="Flutter" :rate="5" />
        <SkillRate name="React" :rate="4" />
        <SkillRate name="Unity" :rate="5" />
        <SkillRate name="Figma" :rate="4" />
        <SkillRate name="Java" :rate="5" />
        <SkillRate name="DSA" :rate="5" />
      </div>

<!--      <div class="skill-set">-->
<!--        <h3>Non-Tech</h3>-->
<!--        <SkillRate name="Binge watching" :rate="5" />-->
<!--        <SkillRate name="Skateboarding" :rate="4" />-->
<!--        <SkillRate name="" :rate="1" />-->
<!--        <SkillRate name="Sense of humor" :rate="4" />-->
<!--      </div>-->
      <div style="clear:both" />

      <h2>Education</h2>

      <h3>B.Tech (2024-Present)</h3>
      <h4>Ms. Computer Science (Santa Clara University, CA)</h4>
<!--      <div>CGPA - 4</div>-->

      <h3>B.Tech (2020-2024)</h3>
      <h4>B.Tech Computer Science (IIIT, Surat)</h4>
      <div>CGPA - 8.93</div>

      <h3>High School</h3>
      <h4>Edunova (Ahmedabad)</h4>
      <div>percentage - 80%</div>



      <h2>Besides...</h2>
      <div>
        <h3>I ❤️</h3>
        <div>Gaming</div>
        <div>Working Out</div>
        <div>Cooking</div>
        <div>Go-Karting</div>

      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import SkillRate from "@/components/SkillRate.vue";

export default Vue.extend({
  name: "Resume",
  components: {
    SkillRate,
  },
});
</script>

<style scoped>
h2 {
  font-weight: 100;
  font-size: 2em;
  margin: 0px;
  padding: 0px;
  padding-top: 50px;
}
h3 {
  font-weight: 100;
  font-size: 1.6em;
  margin: 0px;
  padding: 0px;
  padding-top: 30px;
}
h4 {
  font-weight: 100;
  font-size: 1.3em;
  margin: 0px;
  padding: 0px;
  padding-top: 15px;
  font-style: italic;
}

.paragraph {
  max-width: 700px;
}

.download-link {
  float:left;
  margin-right: 50px;
}

.full-content div {
  max-width: 800px;
}

.skill-set h3 {
  padding-bottom: 10px;
}

.photo img {
  height: 300px;
  width: 300px;
}

.tech-stack {
  font-style: italic;
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
    padding: 30px;
    padding-left: 80px;
  }

  .skill-set {
    float: left;
    padding-right: 60px; 
  }
}
</style>