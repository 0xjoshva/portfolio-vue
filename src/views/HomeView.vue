<template>
  <section id="home">
 <div id="home-cont">   
    <div id="greeting">
  <h1 id="heading">
    <div id="before"><span id="fill">Hi<span id="comma">,</span> I'm</span></div>
  <div id="after">Joshua<span id="comma">;</span></div></h1>
  <p id="subheading">web developer</p>
  </div>
  <div id="image-cont" class="parent">
  <img src="../assets/horse.jpg" alt="" id="abstract" class="image1">
  </div>
  
  <div id="mini-p" class="">
  <div class="image2 icons">
    <span><i class="bi bi-instagram"></i></span>
    <span><i class="bi bi-twitter"></i></span>
    <span><i class="bi bi-linkedin"></i></span>
    <span><i class="bi bi-github"></i></span>
  </div>
  <div class="image2 row" id="blurb">
    <p>i am an aspiring full-stack web developer,
    with a passion for design and programming.</p>
    <a href="/about" id="about-link">read more</a>
  </div>
  </div>

  </div>

  </section>
</template>

<script>
// @ is an alias to /src

export default {
}
</script>

<style scoped>
#home{
background: var(--bg-color);
width: 100%;
height: 100vh;
}
#heading{
  color: var(--bg-color);
  text-shadow: -1px -1px 0 var(--white), 1px -1px 0 var(--white), -1px 1px 0 var(--white), 1px 1px 0 var(--white);
  font-size: 120px;
  font-family: 'Palanquin', sans-serif;
  font-weight: 700;
  display: flex;
  flex-direction: column;
  line-height: 120px;
}
#fill{
  color: var(--white);
}
#subheading{
color:var(--green);
font-family: 'Palanquin', sans-serif;
font-size: 30px;
align-self: inherit;
}

#comma{
  color:var(--green);
  text-shadow: none;
}
#greeting{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 500px;
  height: 500px;
}
#abstract{
  width: auto;
  height: 600px;
  border-radius: 10px;
  transition: all 1s ease-in-out;
  
}
#abstract:hover{
box-shadow: 10px 10px 10px 0px rgba(29,29,29,0.67);
-webkit-box-shadow: 10px 10px 10px 0px rgba(29,29,29,0.67);
-moz-box-shadow: 10px 10px 10px 0px rgba(29,29,29,0.67);
transform: translateY(-5px);


}
#home-cont{
  display: flex;
  flex-direction: row;
}
#image-cont{
padding-top: 3.5rem;
margin-left: 20%;
}

.icons{
  color: var(--lgrey);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  row-gap: 5px;
  width: 45px;
  height: 135px;
  background: rgba( 14, 14, 14, 0.2 );

backdrop-filter: blur( 11px );
-webkit-backdrop-filter: blur( 11px );
border: 1px solid rgba( 255, 255, 255, 0.18 );
border-radius: 3px;
transition: box-shadow 0.7s ease-in-out;
transform: translateX(-7px);
}
.icons:hover{
box-shadow: 0 8px 32px 0 rgba(128, 128, 128, 0.37);

}
.icons > span:hover{
    color: var(--white);
}
#blurb{
  padding: 20px;
  width: 190px;
    background: rgba( 14, 14, 14, 0.2 );
    height: 220px;

backdrop-filter: blur( 11px );
-webkit-backdrop-filter: blur( 11px );
border: 1px solid rgba( 255, 255, 255, 0.18 );
border-radius: 3px;
color: var(--lgrey);
transition: box-shadow 0.7s ease-in-out;
}
#blurb:hover{
  box-shadow: 0 8px 32px 0 rgba(128, 128, 128, 0.37);
}
#about-link{
  margin-top: 0.5rem;
  width: fit-content;
  text-decoration: none;
  color: var(--white);
  padding: 2px 8px;
  border: 3px solid var(--green);
  border-radius: 20px;
  transition: box-shadow 0.8s ease-in;
  transition: transform 0.5s ease-in;
}
#about-link:hover{
  box-shadow: 3px 8px 12px 0 var(--green) inset;
  transform: translateY(-3px);
}

#mini-p{
  margin-top: 5rem;
  display: flex;
  flex-direction: column;
  row-gap: 50px;
  justify-content: space-between;
  margin-bottom: 1.5rem;
  transform: translateX(-7px);
}
</style>
