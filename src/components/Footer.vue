<template>
  <div class="footer">
    <div class="footer-content">
      <div class="left"><strong>Made with ❤️ by Harsh</strong></div>
      <div class="right"><strong>Reach me at <a href="mailto:hurshrao@gmail.com">hurshrao@gmail.com</a> or <router-link to="/contact">through here</router-link></strong></div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "Footer"
});
</script>

<style scoped lang="less">
@import '../css/variables.less';

.footer {
  background-color: #F5F2EE;  // Light beige background
  width: 100%;
  margin-top: 40px;
  border-top: 1px solid rgba(166, 127, 93, 0.1);  // Subtle separator
}

.footer-content {
  color: #A67F5D;
  width: 100%;
  font-size: 0.8em;
  opacity: 1;
  padding-bottom: 30px;
  max-width: 1200px;
  margin: 0 auto;

  * {
    color: #A67F5D;
  }

  strong {
    font-weight: 500;
    opacity: 1;
    color: #A67F5D !important;
  }

  a, router-link {
    color: #A67F5D !important;
    transition: all 0.3s ease;
    text-decoration: none;
    border-bottom: 1px solid transparent;
    opacity: 1 !important;
    font-weight: 600 !important;

    &:hover {
      opacity: 0.8 !important;
      border-bottom-color: #A67F5D;
    }
  }
}

.left, .right {
  padding-top: 10px;
  text-align: center;
  color: #A67F5D;
}

// Mobile view
@media only screen and (max-width: 620px) {
  .footer {
    background-color: #F5F2EE !important;  // Keep light beige in mobile
  }

  .footer-content {
    padding: 20px 10px;
    
    .left, .right {
      float: none;
      width: 100%;
      text-align: center;
      padding: 10px 0;
      
      strong {
        color: #A67F5D !important;
        font-weight: 500;
      }

      a, router-link {
        color: #A67F5D !important;
        font-weight: 600 !important;
        display: inline-block;
        margin: 0 2px;
        
        &:hover {
          opacity: 0.8 !important;
          border-bottom-color: #A67F5D;
        }
      }
    }
  }
}

// Desktop view
@media only screen and (min-width: 621px) {
  .footer-content {
    padding: 0;
  }

  .left, .right {
    padding: 20px;
  }

  .left {
    float: left;
  }

  .right {
    float: right;
  }
}
</style>