<template>
  <div id="app" class="noselect">

    <div id="head">
      <nav class="slideV">
        <div class="home active"><a href="#">Home</a></div>
        <div class="work"><a href="#work">My work</a></div>
        <div class="about"><a href="#about">About</a></div>
        <div class="contact"><a href="#contact">Contact</a></div>
      </nav>
    </div>

    <div id="welcome" class="fadeIn">
      <div class="flex-contain">
        <img src="img/logo.png" alt="logo" id="logo" class="flex-item">
        <div class="flex-item">
          <h2><span class="thin">CHARLES</span> <span class="bold">MANGIN</span></h2>
          <h2>WEB <span class="tonic">DEVELOPER</span> - UX/UI <span class="tonic">DESIGNER</span></h2>
        </div>
      </div>

      <div class="welcome-nav">
        <a href="#work" class="hover-color"><h2>Discover my works<span class="tonic">.</span></h2></a>
        <a href="#about" class="hover-color"><h2>Who am I<span class="tonic">?</span></h2></a>
        <a href="#contact" class="hover-color"><h2>Want to get in touch<span class="tonic">?</span></h2></a>
      </div>

      <div class="text-anim fadeIn">
        <div class="tags-full">Web Developement | Design | Communication | Marketing | SEO | UX/UI | Law | Management |
          Web Developement | Design | Communication | Marketing | SEO | UX/UI | Law | Management
        </div>
        <div class="tags-empty">Web Developement | Design | Communication | Marketing | SEO | UX/UI | Law | Management |
          Web Developement | Design | Communication | Marketing | SEO | UX/UI | Law | Management
        </div>
      </div>
    </div>

    <div id="work">
      <div class="fadeIn test">
        <h2 class="tonic title">{{ content.work.devTitle }}</h2>
        <div class="project-container" v-for="project in content.work.devProjects" :key="project.id">
          <div class="project">
            <img :src="project.img" :alt="project.title">
            <h3 class="sub-title">{{ project.title }}</h3>
            <a :href="project.link" target="_blank">
              <div class="project-desc">
                <p class="used-tech">{{ project.tech }}</p>
                <p class="details">{{ project.date }} ({{ project.time }} - {{ project.team }})</p>
                <p class="desc">{{ project.desc }}</p>
              </div>
            </a>
          </div>
        </div>
      </div>
      <div class="fadeIn">
        <h2 class="tonic title">{{ content.work.designTitle }}</h2>

        <div class="project-container" v-for="project in content.work.designProjects" :key="project.id">
          <div class="project">
            <img :src="project.img" :alt="project.title">
            <h3 class="sub-title">{{ project.title }}</h3>
            <a :href="project.link" target="_blank">
              <div class="project-desc">
                <p class="used-tech">{{ project.tech }}</p>
                <p class="details">{{ project.date }} ({{ project.time }} - {{ project.team }})</p>
                <p class="desc">{{ project.desc }}</p>
              </div>
            </a>
          </div>
        </div>
      </div>
      <div id="resume"><a href="assets/CV_MANGIN-Charles.pdf" download class="tonic">> Download my resume</a></div>
    </div>

    <div id="about">
      <div class="fadeIn">
        <h2 class="tonic title">{{ content.about.who.title }}</h2>
        <div class="paragraph">{{ content.about.who.txt1 }}</div>
        <div class="paragraph">{{ content.about.who.txt2 }}</div>
      </div>

      <div id="picture" class="fadeIn">
        <div id="charles"></div>
        <div id="legend" class="tonic">Doing the things I love, while trying to better the world around me.</div>
      </div>

      <div class="fadeIn">
        <h2 class="tonic title">{{ content.about.what.title }}</h2>
        <div class="paragraph">{{ content.about.what.txt1 }}</div>
        <div class="paragraph">{{ content.about.what.txt2 }}</div>
        <h3 class="tonic sub-title">{{ content.about.what.multimedia.title }}</h3>
        <ul>
          <li v-for="item in content.about.what.multimedia.list" :key="item.id">{{ item }}</li>
        </ul>

        <h3 class="tonic sub-title">{{ content.about.what.managementLaw.title }}</h3>
        <ul>
          <li v-for="item in content.about.what.managementLaw.list" :key="item.id">{{ item }}</li>
        </ul>
      </div>

      <div>
        <h2 class="tonic title fadeIn">{{ content.about.tools.title }}</h2>
        <div class="tools fadeIn">
          <h3 class="tonic sub-title">{{ content.about.tools.programming.title }}</h3>
          <div class="skill-container">
            <p>HTML</p>
            <div class="container">
              <div class="skills html">95%</div>
            </div>
          </div>
          <div class="skill-container">
            <p>CSS</p>
            <div class="container">
              <div class="skills css">85%</div>
            </div>
          </div>
          <div class="skill-container">
            <p>JavaScript (& Vue.JS)</p>
            <div class="container">
              <div class="skills js">70%</div>
            </div>
          </div>
          <div class="skill-container">
            <p>PHP</p>
            <div class="container">
              <div class="skills php">40%</div>
            </div>
          </div>
          <div class="skill-container">
            <p>SQL</p>
            <div class="container">
              <div class="skills sql">40%</div>
            </div>
          </div>
          <div class="skill-container">
            <p>C#</p>
            <div class="container">
              <div class="skills c-sharp">20%</div>
            </div>
          </div>
        </div>

        <div class="tools fadeIn">
          <h3 class="tonic sub-title">{{ content.about.tools.softwares.title }}</h3>
          <div class="skill-container">
            <p class="skill-name">JetBrains</p>
            <div class="container">
              <div class="skills jetbrains">80%</div>
            </div>
          </div>
          <div class="skill-container">
            <p class="skill-name">Visual Studio</p>
            <div class="container">
              <div class="skills vsc">70%</div>
            </div>
          </div>
          <div class="skill-container">
            <p class="skill-name">Wordpress</p>
            <div class="container">
              <div class="skills wordpress">65%</div>
            </div>
          </div>
          <div class="skill-container">
            <p class="skill-name">Adobe Suite</p>
            <div class="container">
              <div class="skills adobe">75%</div>
            </div>
          </div>
          <div class="skill-container">
            <p class="skill-name">Microsoft Office Suite</p>
            <div class="container">
              <div class="skills office">95%</div>
            </div>
          </div>
          <div class="skill-container">
            <p class="skill-name">Google Suite</p>
            <div class="container">
              <div class="skills google">95%</div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div id="contact">
      <h2 class="tonic title fadeIn">{{ content.about.contact.title }}</h2>
      <div class="fadeIn">
        <div class="social"><a href="https://www.linkedin.com/in/charles-m-9014a4151/" target="_blank"><i class="fab fa-linkedin"></i>LinkedIn</a></div>
        <div class="social"><a href="mailto:charlesmangin.98@gmail.com" target="_blank"><i class="fas fa-at"></i>Gmail</a></div>
        <div class="social"><a href="https://github.com/Ezellix" target="_blank"><i class="fab fa-github"></i>GitHub</a></div>
        <div class="social"><a href="https://www.instagram.com/charles_0229/" target="_blank"><i class="fab fa-instagram"></i>Instagram</a></div>
      </div>
    </div>

    <div id="more"><p>(More projects and updates coming very soon!)</p></div>

    <div id="footer">© {{ year.getYear() + 1900 }} Copyright: charlesmangin.fr</div>

  </div>
</template>

<script>
import axios from 'axios';

export default {
  name: 'App',

  data() {
    return {
      content: {},
      active: false,
      year: 0
    }
  },

  created () {
    axios.get('content.json').then(function (response) {
      console.log(response.data);
      this.content = response.data;
    }.bind(this))
        .catch(function (error) {
          console.log(error);
        });

    window.addEventListener('scroll', this.scrollPercentage);

    this.year = new Date();
  },

  destroyed () {
    window.removeEventListener('scroll', this.scrollPercentage);
  },

  methods: {
    scrollPercentage () {
      let scroll = (document.documentElement.scrollTop + document.body.scrollTop) / (document.documentElement.scrollHeight - document.documentElement.clientHeight) * 100;

       if (window.innerWidth > 875) {
        if (scroll > 95) {
          document.querySelector('.contact').classList.add("active");
          document.querySelector('.about').classList.remove("active");
          document.querySelector('.work').classList.remove("active");
          document.querySelector('.home').classList.remove("active");
        } else if (scroll > 51 && scroll <= 95) {
          document.querySelector('.about').classList.add("active");
          document.querySelector('.contact').classList.remove("active");
          document.querySelector('.work').classList.remove("active");
          document.querySelector('.home').classList.remove("active");
        } else if (scroll > 14 && scroll <= 51) {
          document.querySelector('.work').classList.add("active");
          document.querySelector('.about').classList.remove("active");
          document.querySelector('.contact').classList.remove("active");
          document.querySelector('.home').classList.remove("active");
        } else {
          document.querySelector('.home').classList.add("active");
          document.querySelector('.about').classList.remove("active");
          document.querySelector('.work').classList.remove("active");
          document.querySelector('.contact').classList.remove("active");
        }
      } else if (window.innerWidth < 650 && window.innerWidth > 450) {
        if (scroll > 95) {
          document.querySelector('.contact').classList.add("active");
          document.querySelector('.about').classList.remove("active");
          document.querySelector('.work').classList.remove("active");
          document.querySelector('.home').classList.remove("active");
        } else if (scroll > 52 && scroll <= 95) {
          document.querySelector('.about').classList.add("active");
          document.querySelector('.contact').classList.remove("active");
          document.querySelector('.work').classList.remove("active");
          document.querySelector('.home').classList.remove("active");
        } else if (scroll > 13 && scroll <= 52) {
          document.querySelector('.work').classList.add("active");
          document.querySelector('.about').classList.remove("active");
          document.querySelector('.contact').classList.remove("active");
          document.querySelector('.home').classList.remove("active");
        } else {
          document.querySelector('.home').classList.add("active");
          document.querySelector('.about').classList.remove("active");
          document.querySelector('.work').classList.remove("active");
          document.querySelector('.contact').classList.remove("active");
        }
      } else {
         if (scroll > 96) {
           document.querySelector('.contact').classList.add("active");
           document.querySelector('.about').classList.remove("active");
           document.querySelector('.work').classList.remove("active");
           document.querySelector('.home').classList.remove("active");
         } else if (scroll > 41 && scroll <= 96) {
           document.querySelector('.about').classList.add("active");
           document.querySelector('.contact').classList.remove("active");
           document.querySelector('.work').classList.remove("active");
           document.querySelector('.home').classList.remove("active");
         } else if (scroll > 8 && scroll <= 41) {
           document.querySelector('.work').classList.add("active");
           document.querySelector('.about').classList.remove("active");
           document.querySelector('.contact').classList.remove("active");
           document.querySelector('.home').classList.remove("active");
         } else {
           document.querySelector('.home').classList.add("active");
           document.querySelector('.about').classList.remove("active");
           document.querySelector('.work').classList.remove("active");
           document.querySelector('.contact').classList.remove("active");
         }
       }
    }
  }
}
</script>

<style>
  @import './assets/styles/style.css';
</style>