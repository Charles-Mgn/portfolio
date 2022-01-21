<template>
  <div id="app">

    <div id="head">
      <nav class="slideV">
        <div class="home"><a href="#home">Home</a></div>
        <div class="work"><a href="#work">My work</a></div>
        <div class="about"><a href="#about">About</a></div>
        <div class="contact"><a href="#contact">Contact</a></div>
      </nav>
    </div>


    <div id="home" class="fadeIn">
      <img src="@/assets/img/logo.png" alt="logo" id="logo">
      <h1>Hi, I'm <span class="tonic">Charles</span>.</h1>
      <div id="introduction">I like creating things 😃</div>
      <div class="tonic slash">Front-end Development</div>
      <div class="tonic slash">UX / UI Design</div>
    </div>


    <div id="work">
      <div class="fadeIn">
        <h2 class="tonic title">Dev projects</h2>
        <div class="project-container">
          <a href="https://architech.charlesmangin.fr" target="_blank" class="project project-dev-5">
            <h3 class="sub-title">Architech</h3>
            <div class="project-desc">
              <p>A website made over the course of a 2 days challenge! From designing to the integration with Vue.js, everything was made in about 20 hours.</p>
              <p>Discover an unknown artist of great talent: Jean-Pierre Ugarte.</p>
            </div>
          </a>
          <a href="https://projetmemo.nikolag25.fr" target="_blank" class="project project-dev-4">
            <h3 class="sub-title">"Maison des étudiants de Montbéliard"</h3>
            <div class="project-desc">
              <p>The "Maison des étudiants de Montbéliard" is a student association based in Montbéliard, France. As of today, this association has only a presence on social medias. But as they grow in size, developing a website became a necessity.</p>
            </div>
          </a>
          <a href="https://projets1.charlesmangin.fr" target="_blank" class="project project-dev-1">
            <h3 class="sub-title">AI, a not so bright futur?</h3>
            <div class="project-desc">
              <p>AI is all around us, yet few people are aware of its presence. Is AI a blessing or a malediction for mankind? Find the answer to this and much more on "AI, a not so bright futur?".</p>
            </div>
          </a>
          <a href="https://alteringames.charlesmangin.fr" target="_blank" class="project project-dev-2">
            <h3 class="sub-title">AlterinGames</h3>
            <div class="project-desc">
              <p>Ever wondered how you should spend your saturday afternoon? Maybe you've got some boardgames, but you've already played them a bit too much? With AlterinGames, rediscover your favorite boardgames with brand new house rules.</p>
            </div>
          </a>
          <a href="https://s3-wp.charlesmangin.fr" target="_blank" class="project project-dev-3">
            <h3 class="sub-title">Mountain Climber (a Wordpress Landing Page)</h3>
            <div class="project-desc">
              <p>A small responsive landing page made with Wordpress.</p>
              <p>For this project, a model was given to us. The aim was to get as close as to the original as possible.</p>
            </div>
          </a>
        </div>
      </div>
      <div class="fadeIn">
        <h2 class="tonic title">Design projects</h2>
        <div class="project-container">
          <a href="https://youtu.be/VNLcxtOo9d4" target="_blank" class="project project-5">
            <h3 class="sub-title">Landscapes</h3>
            <div class="project-desc">
              <p>I grew up in a city called Belfort. The aim of this small project was to showcase the main landmarks of Belfort, which includes The Lion of Belfort (made by Bartholdi, the creator of the Statue of Liberty), the Atria Hotel, and the Tower of the Miotte.</p>
            </div>
          </a>
          <a href="https://youtu.be/R5D16f5Xb9A" target="_blank" class="project project-6">
            <h3 class="sub-title">BUG DAYS</h3>
            <div class="project-desc">
              <p>BUG DAYS is a fictional e-sport event for which a created an animated logo as well as a landing page.</p>
            </div>
          </a>
          <a href="https://youtu.be/iBnIJ5YoUYE" target="_blank" class="project project-8">
            <h3 class="sub-title">Monogramme</h3>
            <div class="project-desc">
              <p>Creating an animation of your initials. What's better than a dragon? 🔥🔥</p>
            </div>
          </a>
          <a href="#" target="_blank" class="project project-7">
            <h3 class="sub-title">Space Being (coming soon)</h3>
            <div class="project-desc">
              <p>A small project that I made using Adobe After Effects. I started with an existing image, modified it, and animated it to give it a false 3D perspective.</p>
            </div>
          </a>
        </div>
      </div>
      <div id="resume"><a href="assets/CV_MANGIN-Charles.pdf" download class="tonic">> Download my resume</a></div>
    </div>


    <div id="about">
      <div class="fadeIn">
        <h2 class="tonic title">Who I am</h2>
        <div class="paragraph">My name is Charles Mangin, I'm 23 years old and I am a multimedia student based in France.</div>
        <div class="paragraph">I always liked to create stuff, and now I do it as a job!</div>
      </div>

      <div id="picture" class="fadeIn">
        <div id="charles"></div>
        <div id="legend" class="tonic">Doing the things I love, while trying to better the world around me.</div>
      </div>

      <div class="fadeIn">
        <h2 class="tonic title">What I do</h2>
        <div class="paragraph">I am fairly polyvalent. I have a degree in management, I studied law, and I will soon have a degree in multimedia.</div>
        <div class="paragraph">Here's what I know:</div>
        <h3 class="tonic sub-title">Multimedia</h3>
        <ul>
          <li>Development: How to create websites from A to Z, using multiple programming languages (see below).</li>
          <li>Design: How to create visual identities (including, but not limited to: mock-ups, landing pages, logos, animations).</li>
          <li>Audio-visual: How to film and edit videos.</li>
          <li>Communication: How to communicate on the internet, while keeping in mind SEO challenges.</li>
        </ul>

        <h3 class="tonic sub-title">Management and law</h3>
        <ul>
          <li>Team management: How to organize and manage projects and teams.</li>
          <li>Communication & marketing: Analysing markets, choosing the best strategies to adopt based on the needs of the client.</li>
          <li>Accounting & finance: Analysing costs, knowing how to keep up with a budget.</li>
          <li>Law: French business laws and administrative laws.</li>
        </ul>
      </div>

      <div>
        <h2 class="tonic title fadeIn">Tools I use</h2>
        <div class="tools fadeIn">
          <h3 class="tonic sub-title">Programming languages</h3>
          <ul>
            <li>HTML</li>
            <li>CSS</li>
            <li>JS (w/ Vue.JS)</li>
            <li>SQL</li>
            <li>C#</li>
            <li>PHP</li>
          </ul>
        </div>
        <div class="tools fadeIn">
          <h3 class="tonic sub-title">Softwares</h3>
          <ul>
            <li>JetBrains</li>
            <li>Visual Studio</li>
            <li>Wordpress</li>
            <li>Adobe Suite</li>
            <li>Microsoft Office Suite</li>
            <li>Google Suite</li>
          </ul>
        </div>
      </div>
    </div>

    <div id="contact">
      <h2 class="tonic title fadeIn">Want to get in touch?</h2>
      <div class="fadeIn">
        <div class="social"><a href="https://www.linkedin.com/in/charles-m-9014a4151/" target="_blank"><i class="fab fa-linkedin"></i>LinkedIn</a></div>
        <div class="social"><a href="mailto:charlesmangin.98@gmail.com" target="_blank"><i class="fas fa-at"></i>Gmail</a></div>
        <div class="social"><a href="https://github.com/Ezellix" target="_blank"><i class="fab fa-github"></i>GitHub</a></div>
        <div class="social"><a href="https://www.instagram.com/charles_0229/" target="_blank"><i class="fab fa-instagram"></i>Instagram</a></div>
      </div>
    </div>

    <div id="more"><p>(More projects and updates coming very soon!)</p></div>

    <div id="footer">© 2022 Copyright: charlesmangin.fr</div>

  </div>
</template>

<script>
export default {
  name: 'App',
  created () {
    window.addEventListener('scroll', this.scrollPercentage);
  },
  destroyed () {
    window.removeEventListener('scroll', this.scrollPercentage);
  },
  methods: {
    scrollPercentage () {
      let scroll = (document.documentElement.scrollTop + document.body.scrollTop) / (document.documentElement.scrollHeight - document.documentElement.clientHeight) * 100;
      if (scroll > 95) {
        document.querySelector('.contact').classList.add("active");
        document.querySelector('.about').classList.remove("active");
        document.querySelector('.work').classList.remove("active");
        document.querySelector('.home').classList.remove("active");
      }
      else if (scroll > 50 && scroll <= 95) {
        document.querySelector('.about').classList.add("active");
        document.querySelector('.contact').classList.remove("active");
        document.querySelector('.work').classList.remove("active");
        document.querySelector('.home').classList.remove("active");
      }
      else if (scroll > 20 && scroll <= 50) {
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
    },
  }
}
</script>

<style>
  @import './assets/styles/style.css';
</style>