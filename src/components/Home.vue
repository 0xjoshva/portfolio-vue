<template>
  <section id="home">
    <div id="home-cont">
      <div id="greeting">
        <h1 id="heading">
          <div id="before">
            <span id="fill">hi<span id="comma">,</span> i'm</span>
          </div>
          <div id="after">joshua<span id="comma">;</span></div>
        </h1>
        <p id="subheading">web developer</p>
      </div>
      <div id="image-cont" class="parent">
        <img src="../assets/horse.jpg" alt="" id="abstract" class="image1" />
      </div>

      <div id="mini-p" class="">
        <div class="image2 icons">
          <span><i class="bi bi-instagram"></i></span>
          <span><i class="bi bi-twitter"></i></span>
          <span> <a href="https://www.linkedin.com/in/joshua-steed-1526b6238/" target="_blank"><i class="bi bi-linkedin"></i></a></span>
          <span> <a href="https://github.com/0xjoshva" target="_blank"><i class="bi bi-github"></i></a></span>
        </div>
        <div class="image2 row" id="blurb">
          <p>
            I am an aspiring full-stack web developer, with a passion for design
            and programming.
          </p>
          <a href="" id="about-link" >read more</a>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {};
</script>
<style scoped>
#home {
  /* background-color: var(--bg-color);
  background-image: url(../assets/green-dots.png);
  background-blend-mode: multiply; */
  /* background: radial-gradient(
      ellipse 50% 400px,
      #80ffdb00 50%,
      #101010a2 80%,
      #101010ce,
      #101010
    ),
    url(../assets/green-dots.png); */
    background-color: var(--bg-color);
  background-size: contain;
  width: 100%;
  height: 100vh;
}
#heading {
  color: var(--bg-color);
  text-shadow: -1px -1px 0 var(--white), 1px -1px 0 var(--white),
    -1px 1px 0 var(--white), 1px 1px 0 var(--white);
  font-size: 8rem;
  font-family: "Montserrat", sans-serif;
  font-weight: 700;
  display: flex;
  flex-direction: column;
  line-height: 8rem;
  padding-left: 8rem;
}
#fill {
  color: var(--white);
}
#subheading {
  color: var(--green);
  font-family: "Montserrat", sans-serif;
  font-size: 30px;
  align-self: inherit;
}

#comma {
  color: var(--green);
  text-shadow: none;
}
#greeting {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 500px;
  height: 500px;
}
#abstract {
  width: auto;
  height: 550px;
  border-radius: 10px;
  transition: all 1s ease-in-out;
}
#abstract:hover {
  box-shadow: 10px 10px 10px 0px rgba(29, 29, 29, 0.67);
  -webkit-box-shadow: 10px 10px 10px 0px rgba(29, 29, 29, 0.67);
  -moz-box-shadow: 10px 10px 10px 0px rgba(29, 29, 29, 0.67);
}
#home-cont {
  display: flex;
  flex-direction: row;
}
#image-cont {
  padding-top: 3.5rem;
  margin-left: 30vw;
}

.icons {
  color: var(--lgrey);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  row-gap: 5px;
  width: 45px;
  height: 135px;
  background: rgba(14, 14, 14, 0.2);

  backdrop-filter: blur(11px);
  -webkit-backdrop-filter: blur(11px);
  border: 1px solid rgba(255, 255, 255, 0.18);
  border-radius: 3px;
  transition: box-shadow 0.7s ease-in-out;
  transform: translateX(-7px);
}
.icons:hover {
  box-shadow: 0 8px 32px 0 rgba(128, 128, 128, 0.37);
}
.icons > span:hover {
  color: var(--white);
}
#blurb {
  padding: 10px;
  width: 190px;
  background: rgba(14, 14, 14, 0.2);
  height: 11rem;
  font-family: "Montserrat", sans-serif;
  line-height: 1.1rem;
  backdrop-filter: blur(11px);
  -webkit-backdrop-filter: blur(11px);
  border: 1px solid rgba(255, 255, 255, 0.18);
  border-radius: 3px;
  color: var(--lgrey);
  transition: box-shadow 0.7s ease-in-out;
}
#blurb:hover {
  box-shadow: 0 8px 32px 0 rgba(128, 128, 128, 0.37);
}
#about-link {
  margin-top: 0.5rem;
  width: fit-content;
  text-decoration: none;
  color: var(--white);
  padding: 7px 8px 0px 10px;
  border: 3px solid var(--green);
  border-radius: 20px;
  transition: transform 0.2s ease-in;
}
#about-link:hover {
  transform: translateY(-3px);
  box-shadow: 0 8px 32px 0 rgba(128, 128, 128, 0.37);
}

#mini-p {
  margin-top: 5rem;
  display: flex;
  flex-direction: column;
  row-gap: 50px;
  justify-content: space-between;
  margin-bottom: 1.5rem;
  transform: translateX(-7px);
}
a{
  color: inherit;
}

@media only screen and (max-width: 600px) {
#heading {
font-size: 7rem;
      padding-left: 3rem;
      margin: 0 auto;
}
#abstract{
  display:none;}
#mini-p{
  display: none;
}
#blurb{
  display: none;
}
}
</style>
