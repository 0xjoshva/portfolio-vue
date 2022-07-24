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

<p id="content">I am an enthusiastic student at <span>Life Choices Academy</span> where I have been learning full-stack web development for the past 4 months. I have been taught   <span>HTML</span>, <span>CSS</span>, <span>MySQL</span>, <span>Git</span>, and <span>JavaScript</span> including frameworks <span>Bootstrap 5</span>, <span>Node.js</span> and <span>Vue.js</span>. I have made projects with with all of the above mentioned and I am constantly improving with time. I try to keep pushing my limits on every single project I make because I am passionate about programming and eager to start working, which is the next step in my path to reaching my full potential as a web developer.
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
    height: 110%;
    object-fit: cover;
    filter: brightness(10%);
    display: block;
    transform: translateY(-3.5rem);
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


@media only screen and (max-width: 1200px){
    /*Tablets [601px -> 1200px]*/
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
@media only screen and (max-width: 600px) {
  /*Big smartphones [426px -> 600px]*/
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
@media only screen and (max-width: 425px){
  #resume{
    padding-left: 2rem;
  }
  #header{
    padding-left: 0px;
  }
}
</style>