<template>
  <div class="content">
    <div data-aos="fade-right" class="textBox">
      <h1 class="text">Welcome to my portfolio!</h1>
      <p class="bio">
        My name is Koen Martens, I am 19 years old and I am currently a student
        in my 2nd year of becoming a full stack developer.
      </p>
    </div>
    <div class="skills">
      <div class="skillsRow">
        <div class="circleSkill">
          <h1>HTML</h1>
          <p>80%</p>
        </div>
        <div class="circleSkill">
          <h1>CSS</h1>
          <p>80%</p>
        </div>
        <div class="circleSkill">
          <h1>Javascript</h1>
          <p>75%</p>
        </div>
        <div class="circleSkill">
          <h1>Vue</h1>
          <p>70%</p>
        </div>
      </div>
      <div class="skillsRow">
        <div class="circleSkill">
          <h1>Java</h1>
          <p>75%</p>
        </div>
        <div class="circleSkill">
          <h1>C#</h1>
          <p>40%</p>
        </div>
        <div class="circleSkill">
          <h1>Python</h1>
          <p>60%</p>
        </div>
        <div class="circleSkill">
          <h1>MySQL</h1>
          <p>70%</p>
        </div>
      </div>
    </div>

    <div class="path" data-aos="fade-down">
      <h1>My path</h1>
      <p >My education & work history</p>
    </div>
    <div class="pathDown">
      <div class="highschool" data-aos="fade-right">
        <h2>Highschool</h2>
        <p class="school">Campus de Helix</p>
        <p class="location">Te Maasmechelen</p>
        <p class="periode">2015 - 2021</p>
        <p class="uitleg">Business Education followed by Accounting and Computer Science</p>
      </div>

      <div data-aos="fade-top" class="line-1"></div>
      <div data-aos="fade-top" class="circle">
        <i class="fa-solid fa-school" style="color: #ffffff;"></i>
      </div>

      <div class="jumbo" data-aos="fade-left">
        <h2>Student job</h2>
        <p class="school">Jumbo</p>
        <p class="location">Te Lanaken</p>
        <p class="periode">12/2019 - Now</p>
        <p class="uitleg">I am a stock clerk</p>
      </div>

      <div data-aos="fade-top" class="line-1"></div>
      <div data-aos="fade-top" class="circle">
        <i class="fa-solid fa-shop" style="color: #ffffff;"></i>
      </div>

      <div class="college" data-aos="fade-right">
        <h2>College</h2>
        <p class="school">University College PXL</p>
        <p class="location">Te Hasselt</p>
        <p class="periode">2021 - Now</p>
        <p class="uitleg">Professional Bachelor in Applied Information Technology - Application-Development
        </p>
      </div>

      <div data-aos="fade-top" class="line-1"></div>
      <div data-aos="fade-top" class="circle">
        <i class="fa-solid fa-graduation-cap" style="color: #ffffff;"></i>
      </div>

    </div>
  </div>

  <div class="container">
    <ul>
      <li><a class="github" href="https://github.com/KoenMartensPXL"><i class="fab fa-github" aria-hidden="true"></i></a></li>
      <li><a class="linkedin" href="https://www.linkedin.com/in/koen-martens1/"><i class="fa-brands fa-linkedin-in" aria-hidden="true"></i></a></li>
      <li><a class="twitter" href="https://twitter.com/KoenMartens8"><i class="fab fa-twitter" aria-hidden="true"></i></a></li>
      <li><a class="instagram" href="https://www.instagram.com/koentjuh.m/"><i class="fab fa-instagram" aria-hidden="true"></i></a></li>
    </ul>
  </div>

  <div style="height:1000px;">Test</div>
</template>

<script>
import '@fortawesome/fontawesome-free/css/all.css'

export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Home",

}
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.textBox {
  z-index: -1;
  position: absolute;
  top: 25%;
  left: 10%;
}

.text{
  color: transparent;
  font-size: 38px;
  white-space: nowrap;
  font-family: monospace;
  background-image: linear-gradient(90deg, #4d78ef, #709df7, #7ed4fd);
  -webkit-background-clip: text;
  width: 24ch;
  animation: typing 3s steps(24);
}

.bio {
  color: white;
  margin-top: 25px;
  font-size: 20px;
  width: 50ch;
  white-space: normal;
}


@keyframes typing {
  from {
    width: 0%;
  }
}
.skills {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 35%;
}

.skillsRow {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  margin-top: 100px;
  color: white;
  font-family: "Montserrat", sans-serif;
}

.circleSkill h1 {
  font-size: 20px;
  font-weight: 600;
  position: relative;
  margin-top: 35%;
  text-align: center;
}

.circleSkill p {
  font-size: 16px;
  font-weight: 500;
  position: relative;
  margin-left: 40%;
}

.circleSkill {
  display: inline-block;
  position: relative;
  justify-content: center;
  align-items: center;
  border-radius: 50%;
  width: 150px;
  height: 150px;
  border: 10px solid white;
  background-color: rgba(255, 255, 255, .05);
  opacity: 50%;
  box-shadow: 0 0 5px rgba(0, 0, 0, 0.15);
  backdrop-filter: blur(10px);
  margin-top: 100px;
}

body {
  display: grid;
  place-items: center;
  min-height: 100vh;
  font-size: 16px;
}

.path {
  color: white;
  position: relative;
  margin-top: 18%;
  margin-left: 15%;
  font-family: "Montserrat", sans-serif;
}

.path h1{
  font-size: 48px;
}

.path p {
  margin-left: -25px;
  font-size: 20px;
  color: white;
}

.highschool, .jumbo, .college {
  width: 20%;
  height: auto;
  padding: 20px;
  background-color: rgba(255, 255, 255, .05);
  box-shadow: 0 0 5px rgba(0, 0, 0, 0.15);
  backdrop-filter: blur(10px);
  border-radius: 8px;
}

.location {
  font-size: 12px;
}

.highschool {
  margin-top: 75px;
  margin-left: 20%;
}

.jumbo {
  margin-top: 75px;
  margin-left: 50%;
}

.college {
  margin-top: 75px;
  margin-left: 20%;
}

.periode {
  margin-top: 25px;
}

.uitleg {
  margin-top: 10px;
  font-size: 18px;
}

.pathDown {
  font-family: "Montserrat", sans-serif;
  color: white;
}

.line-1 {
  width: 5px;
  height: 375px;
  margin-top: -11%;
  margin-left: 45%;
  z-index: -1;
  border: 0;
  background: white;
}

.circle {
  display: flex;
  justify-content: center;
  align-items: center;
  position: absolute;
  margin-left: 43.65%;
  margin-top: -9%;
  border: 5px solid white;
  border-radius: 50%;
  width: 75px;
  height: 75px;
  background-color: #333;
}

.fa-school, .fa-graduation-cap, .fa-shop {
  font-size: 25px;
}

.container {
  position: fixed;
  bottom: 0;
  margin-bottom: 25px;
  left: 50%;
  transform: translateX(-50%);
}

ul {
  display: flex;
  gap: 2rem;
  list-style:none;
}

ul li a {
  position: relative;
  display: block;
  width: 5rem;
  height: 5rem;
  text-align: center;
  line-height: 5rem;
  background: #171515;
  border-radius: 10px;
  font-size: 2.2rem;
  color: #949292;
  transition: .5s;
}

ul li a:before {
  content: '';
  position: absolute;
  top:0;
  left:0;
  width:100%;
  height:100%;
  border-radius: 10px;
  transition: .5s;
  transform: scale(.9);
  z-index: -1;
}

ul li a:hover:before {
  transform: scale(1.2);
  box-shadow:
      0 0 15px #0197fc;
  filter: blur(3px);
}

ul li a:hover {
  box-shadow:
      0 0 15px #0197fc;
  text-shadow:
      0 0 15px #0197fc;
}

 ul li .instagram:before {
   background: radial-gradient(circle at 30% 107%, #fdf497 0%, #fdf497 5%, #fd5949 45%,#d6249f 60%,#285AEB 90%);
}

ul li .instagram:hover:before {
  box-shadow:
      0 0 15px black;
}
ul li .instagram:hover {
  box-shadow:
      0 0 15px black;
}

ul li .github:before {
  background: #333;
}

ul li .github:hover:before {
  box-shadow:
      0 0 15px black;
}
ul li .github:hover {
  box-shadow:
      0 0 15px black;
}

ul li .linkedin:before {
  background: #0077B5;
}

ul li .linkedin:hover:before {
  box-shadow:
      0 0 15px black;
}
ul li .linkedin:hover {
  box-shadow:
      0 0 15px black;
}

ul li .twitter:before {
  background: #1DA1F2;
}

.skills {
  position: relative;
  left: 50%;
}

@media (max-width: 858px) {
  /* mobile mode */

  .bio {
    white-space: normal;
    width: 40ch;
  }

  img {
    width: 50%;
    height: auto;
  }
}
</style>