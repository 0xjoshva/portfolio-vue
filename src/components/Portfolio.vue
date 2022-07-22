<template>
  <section id="portfolio">
    <div id="featured">
      <div class="header-cont">
        <div class="headers">
          <h1>Featured Projects</h1>
          <!-- <i class="fa-solid fa-fire-flame-curved"></i> -->
        </div>
        <div>
          <router-link id="btn-view" to="/projects">All Projects</router-link>
        </div>
      </div>

      <div id="container">
        <div id="feat-item">
          <img src="../assets/realestate.png" alt="" id="feat-img"/>
          <h2 id="feat-h2">Real Estate Website</h2>
          <p id="feat-p">
            My most recent website. It features a beautiful landing page aswell
            as a property section, where clients can browse/filter active
            listings. The site also has an admin panel where listings can be
            added, sorted and deleted.
          </p>
          <p id="date">July 2022</p>
        </div>
                <div id="feat-item">
          <img src="../assets/blob.png" alt="" id="feat-img"/>
          <h2 id="feat-h2">Blob Portfolio</h2>
          <p id="feat-p">
            My most recent website. It features a beautiful landing page aswell
            as a property section, where clients can browse/filter active
            listings. The site also has an admin panel where listings can be
            added, sorted and deleted.
          </p>
          <p id="date">April 2022</p>
        </div>
        <div id="feat-item">
          <img src="../assets/artgallery.png" alt="" id="feat-img"/>
          <h2 id="feat-h2">Les Chévres: Art Gallery</h2>
          <p id="feat-p">
            My most recent website. It features a beautiful landing page aswell
            as a property section, where clients can browse/filter active
            listings. The site also has an admin panel where listings can be
            added, sorted and deleted.
          </p>
          <p id="date">July 2022</p>
        </div>

      </div>
    </div>
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
#portfolio h1 {
  color: var(--white);
  font-family: "Montserrat", sans-serif;
}
.fa-fire-flame-curved {
  background-color: #fad961;
  background-image: linear-gradient(
    13deg,
    var(--green) 0%,
    #1cf74f 70%,
    #11cd24 100%
  );
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
  font-size: 3rem;
  padding-left: 1rem;
}

.header-cont {
  display: flex;
  flex-direction: row;
  margin-bottom: 1.5em;
  display: flex;
  justify-content: space-around;
  align-items: center;
  padding-top: 10em;
}
.headers {
  display: flex;
  flex-direction: row;
}
.headers h4 {
  align-self: flex-end;
  color: var(--white);
  background: var(--green);
  padding: 5px;
  border-radius: 5px;
  font-size: 1rem;
}

#feat-p {
  color: var(--lgrey);
  font-family: "Montserrat", sans-serif;
  padding-bottom: 2rem;
  padding-left: 2rem;

  padding-top: 0.5rem;
}

#feat-h2 {
  color: var(--white);
  font-family: "Montserrat", sans-serif;
  padding-top: 0.5rem;
 margin-left: 2rem;
 width: fit-content;
  border-bottom: 4px solid var(--green);
}

#container {
  display: flex;
  flex-direction: row;
  width: fit-content;
  justify-content: space-evenly;
}
#feat-link {
  width: fit-content;
  height: fit-content;

}

#link-container {
  display: flex;
  justify-content: flex-end;
  align-items: flex-end;
  flex-direction: column;
}
#lang {
  width: fit-content;
  border-radius: 7px;
  background: linear-gradient(145deg, #1a1a1a, #1f1f1f);
  font-family: "Montserrat", sans-serif;
}
#lang i {
  color: var(--green);
}

#feat-item {
  display: flex;
  flex-direction: column;
  background: var(--dgrey);
  border-radius: 10px;
  margin-left: 2rem;
  margin-right: 2rem;
  padding-bottom: 2rem;
}

#feat-img{
width: fit-content;
height: auto;
border-top-right-radius: 10px;
border-top-left-radius:10px ;
filter: brightness(70%);
}
#feat-img:hover{
  filter: brightness(100%);
}
#btn-view{
  background: var(--bg-color);
  border: none;
  border: 2px solid var(--green);
  border-radius: 30px 30px;
  color: white;
  font-size: 18px;
  padding: 0.6rem 1rem;
  transition: all 1s ease-out;
  text-decoration: none;
}


#date{
  color: rgba(255, 255, 255, 0.174);
  font-weight: 400;
  padding-left: 2rem;
}

@media only screen and (max-width: 600px) {
 #container{
 flex-direction: column;
 row-gap: 2rem;
  }
}
</style>



