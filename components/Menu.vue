<template>
  <div class="container">
    <div class="top-bar">
      <div class="logo-container"><img src="/logo.png" alt="" /></div>
      <div class="background"><img src="/photp.png" alt="" /></div>
      <nav class="menu">
        <ul>
          <li>
            <span class="nav-number">1. </span>
            <span class="nav-text">home</span>
          </li>
          <li>
            <span class="nav-number">2. </span>
            <span class="nav-text">About</span>
          </li>
          <li>
            <span class="nav-number">3. </span>
            <span class="nav-text">Services</span>
          </li>
          <li>
            <span class="nav-number">4. </span>
            <span class="nav-text">Contact</span>
          </li>
        </ul>
        <ul></ul>
      </nav>

      <!-- refactor -->
    </div>
    <div class="intro-container">
      <div>
        <img src="/Cover.png" alt="" />
      </div>
      <div class="intro-details">
        <div class="intro-text">
          <h3>Hi, I'm Narendra</h3>
          <h1>Freelance Full Stack Designer</h1>
          <q>perfection is a lot of little things done right</q>
        </div>
        <div class="intro-buttons">
          <button type="button" class="button1">My Work</button>
          <button type="button" class="button2">Let's Talk</button>
        </div>
      </div>
    </div>
    <div class="services-grid">
      <h2 class="services-header">What I do</h2>

      <div class="flexbox-item">
        <img src="/mobile_web_design.png" alt="" />
        <h4>Mobile & Web Design</h4>
        <p>
          Need a website or mobile app? I can create <br />
          beautiful websites or mobile apps based on <br />
          your content, or redesign your old website <br />
          to improve user engagement or achieve <br />
          your business goals.
        </p>
      </div>

      <div class="flexbox-item">
        <svg
          width="73"
          height="55"
          viewBox="0 0 73 55"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M9.75107 25.7976L12.8781 10.1611C13.2363 8.37116 15.5495 7.84647 16.6455 9.30631L25.908 21.6564C27.3777 23.617 25.5597 24.074 19.4664 31.589C11.3929 27.6298 9.22919 28.4069 9.75107 25.7976Z"
            fill="#336699"
          />
          <path
            d="M52.8906 31.589C46.7635 24.2348 44.7987 23.6677 46.3079 21.6564L55.5705 9.30631C56.665 7.84647 58.9796 8.37116 59.3378 10.1611L62.4649 25.7976C63.0079 28.5184 60.3929 27.83 52.8906 31.589Z"
            fill="#336699"
          />
          <path
            fill-rule="evenodd"
            clip-rule="evenodd"
            d="M53.6839 28.6086L68.8338 17.3404C70.4262 16.157 72.6364 17.6323 72.1484 19.559L66.3655 42.3072L63.6094 44.4229L65.2907 46.5386L63.5445 53.4062C63.3062 54.3427 62.4613 55 61.4937 55H10.7223C9.75471 55 8.90984 54.3427 8.67147 53.4062L6.9253 46.5386L9.67996 44.6119L5.85193 42.3086L0.0689913 19.5604C-0.419032 17.6366 1.78695 16.1542 3.38219 17.3404L18.5307 28.6086L34.2716 1.06491C34.6778 0.355439 35.3943 0 36.1094 0C36.8259 0 37.5396 0.355439 37.9444 1.06491L53.6839 28.6086ZM37.9212 22.1797L44.2669 32.7569C44.6689 33.4268 44.6689 34.2647 44.2669 34.9346L37.9212 45.5118C37.5121 46.193 36.8097 46.5372 36.1087 46.5386C35.4077 46.5386 34.7053 46.1973 34.2934 45.5118L27.9477 34.9346C27.5457 34.2647 27.5457 33.4268 27.9477 32.7569L34.2934 22.1797C34.7025 21.497 35.4063 21.1529 36.1087 21.1529C36.8097 21.1529 37.5093 21.4942 37.9212 22.1797Z"
            fill="#FF6666"
          />
          <path
            d="M21.2988 44.4229C21.2988 45.5907 20.3509 46.5386 19.1831 46.5386H6.92463L5.84985 42.3072H19.1831C20.3509 42.3072 21.2988 43.255 21.2988 44.4229Z"
            fill="#336699"
          />
          <path
            d="M66.3635 42.3072L65.2887 46.5386H53.0303C51.8624 46.5386 50.9146 45.5907 50.9146 44.4229C50.9146 43.255 51.8624 42.3072 53.0303 42.3072H66.3635Z"
            fill="#336699"
          />
        </svg>

        <h4>Graphic Design</h4>
        <p>
          Need art for your project? I can create <br />
          beautiful art, designs based on your project <br />
          requirements such as business cards, digital <br />
          banners, icons, logos, hand-drawn <br />
          characters, abstracts, textures, etc.
        </p>
      </div>
      <div class="flexbox-item">
        <img src="frontend.png" alt="" />
        <h4>Frontend development</h4>
        <p>
          Already have the design? I can create static <br />
          websites such as landing pages, company <br />
          sites, and custom websites with minimal <br />
          javascript. Will deliver a well-documented <br />
          code.
        </p>
      </div>
    </div>
    <div class="clients"></div>
  </div>
</template>
<style scoped>
.services-grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  column-gap: 16px;
}

@media screen and (max-width: 912px) {
  .services-grid {
    grid-template-columns: 1fr;
  }

  .services-grid > .services-header {
    grid-column: unset;
  }
}

.services-header {
  grid-column: span 3;
}

.intro-container {
  display: flex;
  justify-content: center;
  gap: 32px;
}
.top-bar {
  align-items: center;
  width: 100%;
  max-width: 1200px;
  display: flex;
  justify-content: space-between;
  margin-bottom: 156px;
}

h3 {
  width: 271px;
  font-weight: 600;
  line-height: 36px;
  font-size: 26px;
  color: #f9f9f9;
}
h1 {
  font-weight: 600;
  line-height: 54px;
  font-size: 36px;
  color: #f9f9f9;
}
q {
  font: Hind;
  font-size: 20px;
  color: #a4a4a4;
  font-weight: 400;
  line-height: 32.02px;
}

ul {
  display: inline-flex;
  gap: 24px;
}
li {
  display: inline-block;
  font-family: 'Roboto', sans-serif;
  font-style: normal;
  font-weight: 600;
  font-size: 20px;
  line-height: 22px;
}
.background {
  display: inline-block;
}
.button1 {
  background-color: #336699;
  display: inline-flex;
  padding: 10px 30px;
  border: none;
  font-size: 20px;
  font-weight: 500;
  font-family: 'Roboto';
  font-style: normal;
  color: #ffffff;
  border-radius: 5px;
  margin-right: 7px;
  margin-left: 5px;
  margin-top: 50px;
}

.button2 {
  background-color: var(--color-primary);
  display: inline-flex;
  padding: 10px 27px;
  border: none;
  font-size: 20px;
  font-weight: 600;
  font-family: 'Roboto';
  font-style: normal;
  border-radius: 5px;
  margin-left: 20px;
  margin-top: 50px;
}
.flexbox-container {
  display: inline-flex;
  top: 700px;
  align-items: center;
  font-size: 20px;
  font-weight: 400;
}

/*
.services1 {
  position: absolute;
  top: 700px;
  left: 300px;
  font: hind;
  font-weight: 400;
  font-size: 20px;
  color: #a4a4a4;
}
*/
h2 {
  color: #ffffff;
  margin-bottom: 50px;
}
h4 {
  color: #ffffff;
  margin-bottom: 25px;
  margin-top: 15px;
}
/*
.services2 {
  top: 780px;
  position: absolute;
  left: 700px;
  font: hind;
  font-weight: 400;
  font-size: 20px;
  color: #a4a4a4;
}
.services3 {
  top: 780px;
  position: absolute;
  left: 1100px;
  font: hind;
  font-weight: 400;
  font-size: 20px;
  color: #a4a4a4;
}
*/

.nav-text {
  color: var(--color-primary);
}
.nav-number {
  color: #336699;
}
</style>
