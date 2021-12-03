<template>
  <div id="app">

    <div id="head">
      <nav>
        <div class="home"><a href="#home">Home</a></div>
        <div class="work"><a href="#work">My work</a></div>
        <div class="about"><a href="#about">About</a></div>
        <div class="contact"><a href="#contact">Contact</a></div>
      </nav>
    </div>


    <div id="home">
      <img src="@/assets/img/logo.png" alt="logo" id="logo">
      <h1>Hi, I'm <span class="tonic">Charles</span>.</h1>
      <div id="introduction">I like creating things 😃</div>
      <div class="tonic slash">Front-end Development</div>
      <div class="tonic slash">UX / UI Design</div>
    </div>


    <div id="work">
      <div>
        <h2 class="tonic title">Dev projects</h2>
        <div class="project-container">
          <div class="project project-1">
            <h3 class="sub-title">AI, a not so bright futur?</h3>
            <div class="project-desc">
              <p>AI is all around us, yet few people are aware of its presence. Is AI a blessing or a malediction for mankind? Find the answer to this and much more on "AI, a not so bright futur?".</p>
              <p>One of the first websites I created. Part of an assignment in DUT MMI.</p>
            </div>
          </div>
          <div class="project project-2">
            <h3 class="sub-title">AlterinGames</h3>
            <div class="project-desc">
              <p></p>
            </div>
          </div>
          <div class="project project-3">
            <h3 class="sub-title">Gears of Society</h3>
            <div class="project-desc">###</div>
          </div>
          <div class="project project-4">
            <h3 class="sub-title">Comming soon</h3>
            <div class="project-desc">###</div>
          </div>
        </div>
      </div>
      <div>
        <h2 class="tonic title">Design projects</h2>
        <div class="project-container">
          <div class="project project-5">
            <h3 class="sub-title">Landscapes</h3>
            <div class="project-desc">###</div>
          </div>
          <div class="project project-6">
            <h3 class="sub-title">BUG DAYS</h3>
            <div class="project-desc">###</div>
          </div>
          <div class="project project-7">
            <h3 class="sub-title">Space Being</h3>
            <div class="project-desc">###</div>
          </div>
          <div class="project project-8">
            <h3 class="sub-title">Comming soon</h3>
            <div class="project-desc">###</div>
          </div>
        </div>
      </div>
      <div id="resume"><a href="#" class="tonic">> Get my resume</a></div>
    </div>


    <div id="about">
      <div id="picture">
        <img src="@/assets/img/picture.png" alt="that's me!" id="charles">
        <div id="legend" class="tonic">Doing the things I love, while trying to better the world around me.</div>
      </div>

      <div>
        <h2 class="tonic title">Who I am</h2>
        <div class="paragraph">My name is Charles Mangin, I'm 23 years old and I am a multimedia student based in France.</div>
        <div class="paragraph">I always liked to create stuff, and now I do it as a job!</div>
      </div>

      <div>
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
        <h2 class="tonic title">Tools I use</h2>
        <div class="tools">
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
        <div class="tools">
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
      <h2 class="tonic title">Want to get in touch?</h2>
      <div>
        <div class="social">LinkedIn</div>
        <div class="social">Gmail</div>
        <div class="social">GitHub</div>
        <div class="social">Instagram</div>
      </div>
    </div>

    <div id="footer">© 2021 Copyright: charlesmangin.fr</div>

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
      else if (scroll > 25 && scroll <= 50) {
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