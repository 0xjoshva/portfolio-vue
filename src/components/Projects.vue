<template>
 <section id="projects">
    <h2 class="display-3 text-white pb-5 pt-5" id="header">Projects</h2>
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
          <img v-bind:src="project.imageURL" id="rect-img" />
        </div>
        <div id="rect-text">
          <h3 id="title">{{ project.title }}</h3>
          <p id="date">{{ project.date }}</p>
          <div id="badges">
            <span id="html">HTML</span>
            <span id="css">CSS</span>
            <span id="git">GIT</span>
          </div>
          <p id="text">{{ project.text }}</p>
          <div class="project-btn">
            <a v-bind:href="project.hosting" target="_blank" id="live-link"
              ><span>View site</span>
              <i class="fa-solid fa-arrow-up-right-from-square"></i
            ></a>

            <a v-bind:href="project.repo" target="_blank" id="live-link">
              <span>Repository</span> <i class="bi bi-github"></i
            ></a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import ProjectDB from "/data/ProjectDB.json";
export default {
    data() {
    return {
      data: ProjectDB,
    };
  },
}
</script>

<style scoped>
#projects {
  width: 100%;
  height: fit-content;
  background: var(--bg-color);
  font-family: "Montserrat", sans-serif;
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
.select-wrapper {
  display: flex;
  flex-direction: row;
  justify-content: center;
  margin-bottom: 4rem;
  column-gap: 2rem;
}
label {
  border-bottom: 2px solid var(--green);
}

label i {
  padding-right: 0.5rem;
  color: var(--white);
}
#badges {
  display: flex;
  flex-direction: row;
  column-gap: 5px;
}
#badges > span {
  font-size: 10px;
  padding: 0.2rem;
  color: white;
  border-radius: 2px;
  background: var(--lgreen);
}
.rect {
  display: flex;
  flex-direction: row-reverse;
}
#rect-img {
  width: 500px;
  height: 100%;
  object-fit: cover;
  transition: all 1s ease-in-out;
}

#rect-img:nth-child(even) {
  width: 500px;
  height: 100%;
  object-fit: cover;
  transition: all 1s ease-in-out;
}
#date {
  color: rgba(255, 255, 255, 0.174);
  font-weight: 400;
}
#title {
  color: var(--white);
}
#rect-text {
  width: 35rem;
  background: var(--dgrey);
  padding: 2rem;
}
#text {
  color: var(--lgrey);
  text-align: justify;
  padding-right: 1rem;
  padding-bottom: 1rem;
}
#live-link {
  padding: 0.4rem 1rem;
  background: var(--lgreen);
  border: none;
  color: var(--dgrey);
  border-radius: 3px;
  font-size: 16px;
  font-weight: 500;
  text-decoration: none;
}
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  row-gap: 2rem;
}
.project-btn {
  display: flex;
  flex-direction: row;
  width: fit-content;
  column-gap: 0.5rem;
}
.project-btn span {
  margin-right: 0.3rem;
}
.rect:nth-child(even) {
  display: flex;
  flex-direction: row;
}

@media only screen and (max-width: 600px) {
  .rect {
    flex-direction: column;
  }

  .rect:nth-child(even) {
    display: flex;
    flex-direction: column;
  }
  #rect-text {
    width: 90vw;
    background: var(--dgrey);
    padding: 2rem;
  }
  #rect-img {
    width: 90vw;
    height: 100%;
    object-fit: cover;
  }
  .select-wrapper {
    padding-left: 2rem;
    display: flex;
    flex-direction: column;
    row-gap: 1rem;
  }
  #projects h2 {
    text-align: left;
    padding-left: 1rem;
  }
}
</style>