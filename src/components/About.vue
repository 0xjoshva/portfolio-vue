<template>
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
        <!-- <h2 id="heading">Interpersonal Skills</h2> -->
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
</style>
