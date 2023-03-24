<template>
  <nav>
    <input type="checkbox" id="check">
    <label for="check" class="checkbtn">
      <i class="fa-solid fa-bars"></i>
    </label>
    <img src="../images/LogoPortfolio.png">
    <label class="logo">E-Portfolio</label>
    <ul>
      <li><a href="#">About</a></li>
      <li><a href="#">My Path</a></li>
      <li><a href="#">My Projects</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>
  <section></section>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Header",

}
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700&display=swap");

:root {
  --blue: #12d2db;
  --white: #fcf2fa;
  --purple: #912a7eaa;
  --purple-blc: #171515;
  --shadow: 0 5px 10px 5px rgba(0,0,0,.3);
  --navColor: linear-gradient(to right, #000000, #333);
}

* {
  padding: 0;
  margin: 0;
  text-decoration: none;
  box-sizing: border-box;
}

body {
  font-family: 'Poppins', sans-serif;
}

nav {
  position: fixed;
  opacity: 65%;
  background: var(--navColor);
  box-shadow: var(--shadow);
  height: 80px;
  width: 100%;
}

label.logo {
  color: var(--white);
  font-size: 30px;
  line-height: 80px;
  padding: 0 80px;
  letter-spacing: -1px;
  font-weight: 800;
  font-style: italic;
  transition: .2s ease;
  text-shadow: 3px 5px 20px #230622aa;
}

img {
  position: absolute;
  width: 75px;
  height: auto;
}

nav ul {
  float: right;
  margin-right: 80px;
}

nav ul li {
  display: inline-block;
  line-height: 80px;
}

nav ul li a {
  color: var(--white);
  font-size: 17px;
  padding: 7px 13px;
  border-radius: 13px;
  font-family: "Montserrat", sans-serif;
  margin: 5px;

}

a.active, a:hover {
  background: var(--purple-blc);
  transition: .5s;
}

.checkbtn {
  line-height: 80px;
  font-size: 30px;
  float: right;
  cursor: pointer;
  margin-right: 40px;
  display: none;
}

.checkbtn i {
  color: var(--white);
  padding: 5px;
  border-radius: 10px;
  transition: .1s ease;
}

.checkbtn i:hover {
  background: var(--purple-blc);
}

#check {
  display: none;
}

/* responsive phone nav */

@media (max-width: 952px) {
  /* table mode */
  label.logo {
    font-size: 25px;
    padding-left: 100px;
  }

  nav ul li a {
    font-size: 14px;
  }
}

@media (max-width: 858px) {
  /* mobile mode */
  .checkbtn {
    display: block;
  }

  nav {
    opacity: 90%;
  }

  nav ul {
    z-index: 10;
    position: fixed;
    width: 100%;
    height: 0;
    background: black;
    top: 80px;
    left: 0;
    text-align: center;
    transition: .5s;
    overflow: hidden;
  }

  nav ul li:first-child {
    margin-top: 25%;
  }

  nav ul li {
    display: block;
    margin: 75px 0;
    line-height: 30px;
  }

  nav ul li a {
    font-size: 20px;
  }

  a.active, a:hover {
    background: #333;
    color: var(--blue);
    text-shadow: 0 10px 15px var(--blue);
  }

  #check:checked ~ ul {
    height: calc(100vh - 80px);
  }

}

</style>