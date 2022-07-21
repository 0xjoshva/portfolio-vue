<template>
<section id="projects">
<h2 class="display-3 text-white pb-5 pt-5">Projects</h2>
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
    </div>

  


<div class="container">


  <div v-for="project in data" v-bind:key="project.id" class="rect">
    <div id="div-img">
    <img src="{{project.imageURL}}" id="rect-img">
    </div>
    <div id="rect-text">
    <h3 id="title"> {{project.title}}</h3>
    <p id="date">{{project.date}}</p>
    <div id="badges">
      <span id="html">HTML</span>
      <span id="css">CSS</span>
      <span id="git">GIT</span>
    </div>
    <p id="text">{{project.text}}</p>
    <a href="{{project.host}}" id="live-link">View site <i class="fa-solid fa-arrow-up-right-from-square"></i></a>
  </div>
  </div>


  </div>
</section>

    <Experience/>
</template>
<script>
import Experience from "../components/Experience.vue";
import ProjectDB from "C:/Users/Admin/spotify-portfolio-vue/src/components/ProjectDB.json";
export default {
  components: { Experience },
    data() {
        return {
            data: ProjectDB
        }
    }
}
</script>

<style scoped>
#projects{
  width: 100%;
  height: fit-content;
  background: var(--bg-color);
  font-family: 'Montserrat', sans-serif;
  color: var(--white);
}
    #projects h2 {
  font-size: 3rem;
  line-height: 3rem;
  text-align: center;
  font-weight: 400;
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
    color: var(--white);
}
#badges{
  display:flex;
  flex-direction: row;
  column-gap: 5px;
  
}
#badges > span{
  font-size: 10px;
padding: 0.2rem;
color: white;
border-radius: 2px;
background: var(--lgreen);
}
.rect{
display: flex;
flex-direction: row-reverse;
}
#rect-img{
 width: 300px;
}
#date{
  color: rgba(255, 255, 255, 0.174);
  font-weight: 400;
}
#title{
color: var(--white);
}
#rect-text{
  width: 35rem;
  background: var(--dgrey);
  padding: 2rem;
}
#text{
  color: var(--lgrey);
  text-align: justify;
  padding-right: 1rem;
}
#live-link{
  padding: 0.4rem 1rem;
  background: var(--lgreen);
  border: none;
  color:var(--dgrey);
  border-radius: 3px;
  margin-top: 2rem;
   margin-bottom: 1rem;
 font-size: 16px;
 font-weight: 500;
 text-decoration:none;
}
.container{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  row-gap: 2rem;
}
</style>