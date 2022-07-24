<!-- <template>
  <section id="about">
    <marquee behavior="alternate" direction="left" id="scroll-text"
      ><p id="scroll-p">
        • ABOUT • ABOUT • ABOUT • ABOUT • ABOUT • ABOUT • ABOUT • ABOUT • ABOUT
        • ABOUT • ABOUT • ABOUT • ABOUT • ABOUT • ABOUT • ABOUT • ABOUT • ABOUT
        • ABOUT • ABOUT • ABOUT • ABOUT •
      </p></marquee
    >

    <div class="pwrapper">
      <div id="panel2-container">
        <div id="panel2">
          <a href="" id="resume-link"
            ><i class="fa-solid fa-arrow-up-right-from-square"></i>
            <span id="res-txt">Resume</span>
          </a>

          <div class="info-links">
            <a href="mailto:joshuasteed123@gmail.com" id="email"
              ><i class="fa-solid fa-at"></i>
              <span id="res-txt"> joshuasteed123@gmail.com</span>
            </a>
            <a href="tel:+27624597038" id="phone"
              ><i class="fa-solid fa-hashtag"></i>
              <span id="res-txt"> +27 62 459 7038</span>
            </a>
          </div>
          <div class="text-info">
            <p>Name: Joshua Steed</p>
            <p>Age: 19</p>
            <p id>Cape Town, WC</p>
          </div>
        </div>
        <h2 id="soft-skills">SOFT SKILLS</h2>
      </div>

      <div id="panel1">
        <div id="softskills-wrapper">
          <div class="p1-item px-3">
            <i class="fa-solid fa-brain icon"></i>
            <h3>Problem-solving</h3>
            <p>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Tempore
              incidunt error placeat pariatur maiores. Accusamus, optio! Numquam
              incidunt<span id="point">.</span>
            </p>
          </div>
          <div class="p1-item">
            <i class="fa-solid fa-wand-magic-sparkles icon"></i>
            <h3>Creativity</h3>
            <p>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Tempore
              incidunt error placeat pariatur maiores. Accusamus, optio! Numquam
              incidunt<span id="point">.</span>
            </p>
          </div>
          <div class="p1-item px-3">
            <i class="fa-solid fa-comment-dots icon"></i>
            <h3>Communication</h3>
            <p>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Tempore
              incidunt error placeat pariatur maiores. Accusamus, optio! Numquam
              incidunt<span id="point">.</span>
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {};
</script>
<style scoped>
#about {
  background: var(--bg-color);
  width: 100%;
  height: 100vh;
}
.pwrapper {
  display: flex;
  flex-direction: column;
  row-gap: 50px;
}
#panel1 {
  float: right;
  margin-left: auto;
  order: 2;
  width: 69%;
  height: 20rem;
  border-top-left-radius: 10px;
  border-bottom-left-radius: 10px;
  background: var(--dgrey);
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  /* border-top: 0.3px solid var(--green);
  border-left: 0.3px solid var(--green);
  border-bottom: 0.3px solid var(--green); */
}
#panel2 {
  float: left;
  width: 30%;
  height: 20rem;
  border-top-right-radius: 10px;
  border-bottom-right-radius: 10px;
  background: var(--dgrey);
  padding-top: 2rem;
  font-family: "Montserrat", sans-serif;

  /* border-top: 0.3px solid var(--green);
  border-right: 0.3px solid var(--green);
  border-bottom: 0.3px solid var(--green); */
}
#panel2 p {
  color: var(--white);
}

#softskills-wrapper {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  column-gap: 4em;
}

.p1-item h3 {
  color: var(--white);
  padding: 1rem 0 0.5rem 0;
  font-family: "Montserrat", sans-serif;
}
.p1-item p {
  font-family: "Roboto", sans-serif;
  color: var(--lgrey);
  text-align: justify;
  /* width: 300px; */
  font-size: 1rem;
}
.icon {
  color: var(--dgrey);
  /* chrome gradient */
  /* background: linear-gradient(90deg, #7e7e7e 0%,
#e3e3e3 25%,
#787878 50%,
#e3e3e3 75%,
#7e7e7e 100%); */
  background: rgb(75, 75, 75);
  font-size: 21px;
  padding: 13px;
  border-radius: 50%;
}
#heading {
  background: -webkit-linear-gradient(
    280deg,
    rgba(255, 255, 255, 1) 0%,
    rgba(250, 250, 250, 0) 100%
  );
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
  padding: 1rem 0rem 1.5rem 2.5rem;
}
#point {
  color: var(--green);
}

#resume-link {
  background: var(--green);
  color: var(--dgrey);
  font-weight: 500;
  padding: 5px 20px 5px 20px;
  border-radius: 0px 20px 20px 0;
  text-decoration: none;
  transition: all 0.6s ease-in-out;
  font-family: "Montserrat", sans-serif;
}
#resume-link:hover {
  /* border-right: var(--green) 2px solid;
border-bottom: var(--green) 2px solid;
border-top: var(--green) 2px solid;
background: var(--dgrey);
color: var(--white);
font-weight: 400; */
  padding: 5px 20px 5px 50px;
}
#email {
  background: var(--lgrey);
  color: var(--dgrey);
  font-weight: 500;
  padding: 5px 20px 5px 20px;
  border-radius: 0px 20px 20px 0;
  text-decoration: none;
  transition: all 0.6s ease-in-out;
  font-family: "Montserrat", sans-serif;
  width: fit-content;
}
#email:hover {
  padding: 5px 20px 5px 50px;
}
#phone {
  background: var(--lgrey);
  color: var(--dgrey);
  font-weight: 500;
  padding: 5px 20px 5px 20px;
  border-radius: 0px 20px 20px 0;
  text-decoration: none;
  transition: all 0.6s ease-in-out;
  font-family: "Montserrat", sans-serif;
  width: fit-content;
}
#phone:hover {
  padding: 5px 20px 5px 50px;
}
.fa-arrow-up-right-from-square {
  font-size: 14px;
}
#res-txt {
  padding-right: 0.6rem;
}
#scroll-text {
  color: var(--white);
  font-weight: bold;
  font-family: "Montserrat", sans-serif;
}
#soft-skills {
  color: var(--bg-color);
  text-shadow: -0.7px -0.7px 0 var(--white), 0.7px -0.7px 0 var(--white),
    -0.7px 0.7px 0 var(--white), 0.7px 0.7px 0 var(--white);
  font-family: "Montserrat", sans-serif;
  font-size: 100px;
  line-height: 20px;
  font-weight: 900;
  filter: opacity(0.7);
  float: right;
  transform: translateY(21rem);
}

marquee {
  width: 30%;
}

.info-links {
  padding-top: 1rem;
  display: flex;
  width: fit-content;
  flex-direction: column;
  row-gap: 1rem;
}
.info-links a {
  color: var(--green);
  text-decoration: none;
}
.text-info {
  padding-top: 1rem;
  padding-left: 1rem;
}
</style> -->


<template>
<section id="about">
  <figure id="img-div">
  <img src="../assets/torso.jpg" id="pic">
  <figcaption class="text-block">
    <h1>Joshua Steed</h1>
    <p>web developer</p>
  </figcaption>
  </figure>
  <div id="resume">
<h2 id="header">about me</h2>
<h6><span>19 years</span> / <span>Cape Town</span> / <span>Student</span></h6>

<p id="content">I am an enthusiastic student at <span>Life Choices Academy</span> where I have been learning full-stack web development for the past 4 months. I have been taught   <span>HTML</span>, <span>CSS</span>, <span>MySQL</span>, <span>Git</span>, and <span>JavaScript</span> including frameworks <span>Bootstrap 5</span>, <span>Node.js</span> and <span>Vue.js</span>. I have made projects with with all of the above mentioned and I am constantly improving with time. I believe that being committed, hard-working and consistent is the key to success and it is something I strive for every. single. day.
I am eager to start an internship to hone my craft and to attain the skills to be the best web developer I have the potential to become. I have many aspirations and the ability to create something from nothing will allow me to make them come to fruition.
</p>

<hr/>

<h4 id="skills-header">skills</h4>
<div id="wrapper">
            <div id="wrapper2">
            <div class="item">
            <i class="fa-solid fa-brain icon"></i>
            <h3>problem-solving</h3>
            <p>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Tempore
              incidunt error placeat pariatur maiores. Accusamus, optio! Numquam
              incidunt<span id="point">.</span>
            </p>
          </div>
          <div class="item">
            <i class="fa-solid fa-wand-magic-sparkles icon"></i>
            <h3>creativity</h3>
            <p>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Tempore
              incidunt error placeat pariatur maiores. Accusamus, optio! Numquam
              incidunt<span id="point">.</span>
            </p>
          </div>
          </div>
          
          <div id="wrapper2">
          <div class="item">
            <i class="fa-solid fa-comment-dots icon"></i>
            <h3>communication</h3>
            <p>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Tempore
              incidunt error placeat pariatur maiores. Accusamus, optio! Numquam
              incidunt<span id="point">.</span>
            </p>
          </div>
          <div class="item">
            <i class="fa-solid fa-map icon"></i>
            <h3>leadership</h3>
            <p>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Tempore
              incidunt error placeat pariatur maiores. Accusamus, optio! Numquam
              incidunt<span id="point">.</span>
            </p>
          </div>
          </div>
</div>

<div id="container">
  <label for="html">
    html
<div class="progress" name="html">
  <div id="html" class="progress-bar" role="progressbar" aria-valuenow="25" aria-valuemin="0" aria-valuemax="100">%</div>
</div>
</label>

<label for="css">
    css
<div class="progress" name="css">
  <div id="css" class="progress-bar" role="progressbar" aria-valuenow="25" aria-valuemin="0" aria-valuemax="100">%</div>
</div>
</label>

<label for="js">
    js
<div class="progress" name="js">
  <div id="js" class="progress-bar" role="progressbar" aria-valuenow="25" aria-valuemin="0" aria-valuemax="100">%</div>
</div>
</label>

<label for="mysql">
    mysql
<div class="progress" name="mysql">
  <div id="mysql" class="progress-bar" role="progressbar" aria-valuenow="25" aria-valuemin="0" aria-valuemax="100">%</div>
</div>
</label>
</div>
</div>
</section>
</template>
<script>
export default {
  
}
</script>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300&display=swap');
#about{
  background: var(--dgrey);
  width: 100%;
  height: fit-content;
  font-family: 'Montserrat', sans-serif;
  display: flex;
  flex-direction: row;
}
#pic{
    width: auto;
    height: 103%;
    object-fit: cover;
    filter: brightness(10%);
    display: block;
  }
  #img-div{
    position: relative;
  }
.text-block {
  position: absolute;
  bottom:8rem;
  color: var(--white);
  padding-left: 20px;
  padding-right: 20px;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  row-gap: 0.2rem;
}
.text-block h1{
  font-weight: 700;
  font-size: 4rem;
  font-family: 'Roboto', sans-serif;
}
.text-block p{
 font-size: 1.3rem;
  font-family: 'Roboto', sans-serif;
  color: var(--lgreen);
  font-weight: 500;
}
  #resume{
    padding-left: 4rem;
    width: 50%;
  }
#header{
  color: white;
}
#content{
  color: var(--lgrey);
text-align: justify;
  margin: 0 auto;
  padding-right: 3rem;
}
#content span{
  color: var(--green);
}
h2{
  padding-top: 2rem;
  padding-bottom: 2rem;
  font-size: 4rem;
  font-weight: 700;
}
h6{
  color: var(--lgrey);
  padding-bottom: 1rem;
}
h6 span{
  color: var(--green);
  font-weight: 600;
}

hr{
  margin: 3rem 3rem;
  color: var(--lgrey);
  width: 80%;
  	margin: 3rem auto;
}
#skills-header{
    font-size: 2rem;
  font-weight: 600;
  color: var(--white);
  padding-bottom: 1rem;
}

/* progress */
.progress{
  height: 0.4rem;
  display: flex;
  align-items: center;
  background: var(--lgrey);
  width: 20rem;
  border-radius: 0 !important;
}

.progress-bar{
  text-align: center;
  background: var(--green);
  color: var(--green);
}

label{
  color: var(--white);
}
#container{
  padding-top: 3rem;
  display: flex;
  flex-direction: column;
  row-gap: 1.5rem;
  padding-bottom: 3rem;
  padding-left: 1rem;
}
#html.progress-bar{
  width: 50% !important;
}
#css.progress-bar{
  width: 35% !important;
}
#js.progress-bar{
  width: 10% !important;
}
#mysql.progress-bar{
  width: 30% !important;
}

/* soft skills */
#wrapper{
  display: flex;
  flex-direction: row;
  column-gap: 2rem;
}
#wrapper2{
  display: flex;
  flex-direction: column;
  row-gap: 2rem;
}
.item{
border-radius: 10px;
background: var(--dgrey);
transition: all 0.5s ease-in-out;
padding: 1rem;
}
.item:hover{
  background: rgba(255, 255, 255, 0.123);
}
.item h3{
color: var(--white);
font-size: 1.3rem;
padding-top: 1rem;
}
.item p{
  color: var(--lgrey);
  font-size: 0.9rem;
  padding-right: 1rem;
  text-align: left;
}
.icon {
  color: var(--dgrey);
  background: rgb(75, 75, 75);
  font-size: 1.2rem;
  padding: 0.5rem;
  border-radius: 50%;
}

@media only screen and (max-width: 600px) {
  #wrapper{
    flex-direction: column;
  }
    #wrapper2{
    flex-direction: column;
  }
  #resume{
  width: 100%;
  margin: 0 auto;
  }
  #img-div{
    display:none;
  }
}
</style>