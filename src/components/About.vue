<template>
  <section id="about">
    <marquee behaviour="scroll" direction="left" id="scroll-text"
      ><p id="scroll-p">
        • ABOUT • ABOUT • ABOUT • ABOUT • ABOUT • ABOUT •
      </p></marquee
    >

    <div class="pwrapper">
      <div id="panel2-container">
        <div id="panel2">
          <a href="" id="resume-link"
            ><span id="res-txt">Resume</span
            ><i class="fa-solid fa-arrow-up-right-from-square"></i>
          </a>
        </div>
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
  height: 130vh;
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
  /* border-top: 0.3px solid var(--green);
  border-right: 0.3px solid var(--green);
  border-bottom: 0.3px solid var(--green); */
}
#softskills-wrapper {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  column-gap: 4em;
}
.p1-item {
}
.p1-item h3 {
  color: var(--white);
  font-family: "Palanquin", sans-serif;
  padding: 1rem 0 0.5rem 0;
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
  font-family: "Roboto", sans-serif;
  text-decoration: none;
  transition: all 0.6s ease-in-out;
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

marquee {
  width: 30%;
}
</style>
