<template>
  <section id="portfolio">
 
 <div id="featured">
    <div class="header-cont">
      <div class="headers">
      <h1>Featured</h1>
      <h4><span>Recently Added</span></h4>
      </div>
      <div>
        <i class="fa-solid fa-fire-flame-curved"></i>
      </div>
    </div>
    <div id="content-container">
    <div id="feat-img"></div>
    <div id="container">
    <div id="feat-txt">
    <h2 id="feat-h2">Real Estate Website</h2>
    <p id="feat-p">My most recent website.
      It features a beautiful landing page aswell as a property section, where clients can browse/filter active listings.
      The site also has an admin panel where listings can be added, sorted and deleted.
    </p>
    </div>
    <div id="link-container">
      <!-- <a href="" class="btn-three"><i class="bi bi-globe2"></i> Website</a>
      <a href="" class="btn-three"><i class="bi bi-github"></i> Github</a> -->
      
      <div id="lang">
      <ul>
        <li><i class="fa-brands fa-js-square"></i> JavaScript</li>
        <li><i class="fa-brands fa-html5"></i> HTML</li>
        <li><i class="fa-brands fa-css3-alt"></i> CSS</li>
        <li><i class="fa-brands fa-bootstrap"></i> Bootstrap 5</li>

      </ul>
      </div>
    </div>
    </div>
    </div>
</div>

    <!-- <h2 class="display-3 text-white pb-5 pt-5">PORTFOLIO</h2>
<div class="select-wrapper">
    <div id="select-field">
      <label for="dateSelect"
        ><i class="bi bi-calendar4-week"></i>
        <select name="dateSelect" id="">
          <option value="" selected disabled>Sort by Date</option>
          <option value="">Date Created</option>
          <option value="">Recently Added</option>
        </select>
        </label>
    </div>
    
    <div id="select-field">
      <label for="dateSelect"
        ><i class="bi bi-clock-history"></i>
        <select name="dateSelect" id="">
          <option value="" selected disabled>Sort Language</option>
          <option value=""></option>
          <option value="">Recently Added</option>
          <option value="">Recently Added</option>
        </select>
        </label>
    </div>

    <div id="select-field">
      <label for="alphaSelect"
        ><i class="bi bi-sort-alpha-down"></i>
        <select name="alphaSelect" id="">
          <option value="" selected disabled>Sort Alphabetically</option>
          <option value="">Sort A-Z</option>
          <option value="">Sort Z-A</option>
        </select>
        </label>
    </div>
    </div> -->


  </section>
</template>
<script>
export default {};
</script>
<style scoped>
#portfolio {
  background: var(--bg-color);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  height: fit-content;
  width: 100%;
  color: var(--white);
}
#portfolio h1{
  color: var(--white);
  font-family: 'Montserrat', sans-serif;
}
.fa-fire-flame-curved{
background-color: #FAD961;
background-image: linear-gradient(13deg, var(--green) 0%, #1cf74f 70%,  #11cd24 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-size: 5rem;
  padding-left: 1rem;

}

.header-cont{
  display: flex;
  flex-direction: row;
  margin-bottom: 1.5em;
    display: flex;
justify-content: center;
align-items: center;
padding-top: 10em;
}
.headers{
  display: flex;
  flex-direction: column;
}
.headers h4{
  align-self: flex-end;
  color:var(--white);
  background: var(--green);
  padding: 5px;
  border-radius: 5px;
  font-size: 1rem;
}
/* 
MODAL MODAL MODAL
#portfolio h2 {
  font-family: 'Palanquin', sans-serif;
  font-size: 100px;
  line-height: 100px;
  text-align: center;
  font-weight: 700;
}

select {
  background: var(--bg-color);
  color: var(--white);
  border: none;
  font-family: "Roboto", sans-serif;
  font-size: 16px;
}

select:focus {
  outline: none;
}
.select-wrapper{
  display: flex;
  flex-direction: row;
  justify-content: center;
  margin-bottom: 5%;
  column-gap: 2rem;
}
label{
    border-bottom: 2px solid var(--green);
}

label i{
    padding-right: 0.5rem;
} */
#feat-img{
margin-top: 2rem;
height: 30rem;
width: auto;
background: var(--dgrey);
padding-left: 2rem;
padding-right: 2rem;
background-image: url(../assets/realestatewebsite.png);
background-size: cover;
background-attachment:scroll;

}

#feat-p{
color: var(--lgrey);
  font-family: 'Montserrat', sans-serif;
  padding-bottom: 2rem;
  padding-left: 2rem;
  width: 30rem;
  padding-top: 0.5rem;
}

#feat-h2{
  color: var(--white);
  font-family: 'Montserrat', sans-serif;
  width: 21rem;
  padding-top: 0.5rem;
  margin-left: 2rem;
  border-bottom: 4px solid var(--green);
}

#featured{
  margin-left: 2%;
}
#content-container{
  background: var(--dgrey);
  width: 60rem;
  height: fit-content;
  border-radius: 10px 10px;
}
#container{
  display: flex;
  flex-direction: row;
  width:fit-content;
}
#feat-link{
  width: fit-content;
  height: fit-content;
}

#feat-text{
  padding-right: 20rem;
}

#link-container{
  display: flex;
  justify-content: flex-end;
  align-items: flex-end;
  flex-direction: column;
}
#lang{
border-radius: 7px;
background: linear-gradient(145deg, #1a1a1a, #1f1f1f);
border: 1px solid grey;
box-shadow:  8px 8px 16px #161616,
             -8px -8px 16px #242424;
            padding: 1rem;
            margin: 1.3rem;
            margin-left: 19rem;
            font-family: 'Montserrat', sans-serif;
}
#lang i{
  color:var(--green);
}
</style>