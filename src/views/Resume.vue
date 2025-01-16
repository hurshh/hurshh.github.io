<template>
  <div>
    <h1>Resume</h1>

    <div class="paragraph">
      I'm <strong>Harsh Rao</strong>, a developer and designer with passion for app, game and web development and web design, I am exploring new opportunities through internships and collaboration with professionals, including hackathons and competitions.
      <br />
      <br />I’ve worked on projects using Unreal Engine, Flutter, and React, building a solid foundation in game development. I’m excited about AI and machine learning in games and have experience with databases, scripting, and web scraping.
      <br />
      <br />I am currently seeking internship opportunities where I can gain real-world experience. My passion for technology and design drives me to continually improve and explore new possibilities, and I look forward to contributing my expertise to new and exciting projects. If you have any opportunity feel free to
      <router-link to="/contact">contact me</router-link>.
      <br />
      <br />Besides development, I'm passionate about skateboarding, basketball, anime, powerlifting.

      <div style="margin-top:20px; margin-bottom:20px;">
        <a class="download-link" href="d/harsh_resume.pdf" target="_blank"><i class="fa fa-download fa-lg fa-fw"></i> Download as PDF</a>
        <div style="clear:both"></div>
      </div>
    </div>
    <div class="photo">
      <img src="img/avv.png" alt="Photo of John" />
    </div>

    <div style="clear:both"></div>

    <div class="full-content">

      <h2>Work experience</h2>


      <h3>Creatosaurus</h3>
      <h4>Software Developer Intern</h4>
      <h4>01/2024-06/2024</h4>
      <br>
      <div>
        <ul>
          <li>Contributed in development of an image generation and visual detection on augmented reality app.</li>
          <li>Analyzed data on entity count, shade detection, activity patterns and enhanced image segmentation algorithms (YOLOv8) to
            improve accuracy by 15%.</li>
          <li>Migrated 1 of 3 Alteryx workflows to a Lambda function using Python (Boto3, Connectorx, Pandas), S3, and Redshift to
            enable independence from Altery, resulting in annual savings of $8,000 per license</li>
          <li>Developed AWS Lambda functions for MFT-to-S3 data transfer and real-time Redshift partition updates, used Terraform to
            create S3 event notifications and DynamoDB items for workflow triggers and data partitioning, and integrated tables into
            Redshift with PostgreSQL</li>
        </ul>
      </div>
      <br>

      <h3>Indian Institute of Information Technology</h3>
      <h4>Student Researcher</h4>
      <h4>07/2023-01/2024</h4>
      <br>
      <div>
        <ul>
          <li>Developed a molecular diffusion model for graph models research, enhancing trajectory prediction 25%.</li>
          <li>Leveraged NVIDIA HGX supercomputer GPU cluster, reducing computational time by 35% while gaining expertise in
            high-performance computing and large-scale machine learning deployment.</li>
          <li>Implemented parallel Graph Attention Networks to mimic mixture of experts modelling seen in foundation LLMs, Increasing
            model accuracy and efficiency in predicting molecular interations</li>
        </ul>
      </div>
      <br>

      <h3>JIO india</h3>
      <h4>Software Developer Intern</h4>
      <h4>05/2023-07/2023</h4>
      <br>
      <div>
        <ul>
          <li>Implemented Apache Kafka as an indexer in Jenkins Logstash plugin with java, routing over 10,000 daily Jenkins build logs
            directly to Elasticsearch Kibana, enhancing CI/CD reliability and monitoring.</li>
          <li>Adapted the core rebalanced Python script, which allocates OpenStack Nova compute to Jenkins build nodes by adjusting
            Openstack quota, to run as a daemon, boosting responsiveness by 50%.</li>
          <li>Developed a full-stack Flask application on top of rebalancer to monitor 5000 Jenkins build notes, manage OpenStack quota
            requests, track project-specific rebalancer errors and integrated with a grafana dashboard for critical infrastructure
            monitoring.</li>
          <li>Productionalized the rebalancer application with robust error handling and deployment using Docker into a Kubernetes
            cluster.</li>
        </ul>
      </div>
      <br>





      <h2>Skills</h2>

      <div class="skill-set">
<!--        <h3>Tech</h3>-->
        <SkillRate name="Flutter" />
        <SkillRate name="React" />
        <SkillRate name="Unity" />
        <SkillRate name="Figma" />
        <SkillRate name="Java"  />
        <SkillRate name="DSA" />
      </div>

<!--      <div class="skill-set">-->
<!--        <h3>Non-Tech</h3>-->
<!--        <SkillRate name="Binge watching" :rate="5" />-->
<!--        <SkillRate name="Skateboarding" :rate="4" />-->
<!--        <SkillRate name="Seduction" :rate="1" />-->
<!--        <SkillRate name="Sense of humor" :rate="4" />-->
<!--      </div>-->
      <div style="clear:both" />

      <h2>Education</h2>

      <h3>M.S (2024-Present)</h3>
      <h4>Computer Science and Engineering (Santa Clara University, CA)</h4>
      <div>CGPA - 4</div>

      <h3>B.Tech (2020-2024)</h3>
      <h4>Computer Science and Engineering(IIIT, Surat)</h4>
      <div>CGPA - 8.97</div>

      <h3>High School</h3>
      <h4>Edunova (Ahmedabad)</h4>
      <div>percentage - 83%</div>



      <h2>Besides...</h2>
      <div>
        <h3>I love️</h3>
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