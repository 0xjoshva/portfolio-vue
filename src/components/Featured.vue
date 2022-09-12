<template>
  <section id="portfolio">
    <div id="featured">
      <div class="header-cont">
        <div class="headers">
          <h1>featured projects</h1>
          <!-- <i class="fa-solid fa-fire-flame-curved"></i> -->
        </div>
        <div>
          <router-link id="btn-view" to="/projects"
            >view all projects</router-link
          >
        </div>
      </div>

      <div id="container">
        <div id="feat-item">
          <img src="../assets/realestate.png" alt="" id="feat-img" />
          <h2 id="feat-h2">Real Estate Website</h2>
          <p id="feat-p">
            This project was made with goal of having a property listing
            website, with most of the functionality. A user can delete, sort,
            and add properties on the admin panel. A functional UI,
            and a filtering options on the home page.
          </p>
          <p id="date">July 2022</p>
        </div>
        <div id="feat-item">
          <img src="../assets/ecommerceapp.png" alt="" id="feat-img" />
          <h2 id="feat-h2">Ecommerce Store</h2>
          <p id="feat-p">
            I was paired with a partner and tasked to do an ecommerce website.
            We decided to make a store which sells electronics for gaming, such
            as computer parts and peripherals.
          </p>
          <p id="date">August 2022</p>
        </div>
        <div id="feat-item">
          <img src="../assets/cryptoexchange.png" alt="" id="feat-img" />
          <h2 id="feat-h2">Crypto Exchange Website</h2>
          <p id="feat-p">
            This was my final capstone project. I decided to create a web 3.0
            inspired crypto exchange website, where users can purchase crypto
            and read up on trending articles.
          </p>
          <p id="date">September 2022</p>
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
  padding-bottom: 15em;
}
#portfolio h1 {
  color: var(--white);
  font-family: "Montserrat", sans-serif;
  padding-top: 2rem;
  padding-bottom: 1rem;
  font-size: 4rem;
  font-weight: 700;
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
  justify-content: space-around;
  align-items: center;
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
  padding-right: 2rem;
  max-width: 522px;
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
  justify-content: space-between;
  margin-left: 8rem;
  margin-right: 8rem;
  column-gap: 2rem;
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
  padding-bottom: 2rem;
  transition: all 0.3s ease-in-out;
}

#feat-item:hover {
  transform: scale(1.1);
  box-shadow: 0 10px 40px 0 rgba(160, 160, 160, 0.4);
  z-index: 3;
}

#feat-img {
  width: fit-content;
  height: auto;
  filter: brightness(70%);
  transition: 0.4s all ease-in-out;
}
#feat-img:hover {
  filter: brightness(100%);
}
#btn-view {
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

#date {
  color: rgba(255, 255, 255, 0.174);
  font-weight: 400;
  padding-left: 2rem;
}

@media only screen and (max-width: 1200px) {
  /*Tablets [601px -> 1200px]*/
  #container {
    flex-direction: column;
    row-gap: 2rem;
  }
  #portfolio h1 {
    padding-left: 2rem;
    font-size: 3rem;
    width: min-content;
  }
  #container {
    margin: 0;
  }
}

@media only screen and (max-width: 600px) {
  /*Big smartphones [426px -> 600px]*/
  #container {
    flex-direction: column;
    row-gap: 2rem;
  }
  #portfolio h1 {
    padding-left: 2rem;
    font-size: 3rem;
    width: min-content;
  }
}
@media only screen and (max-width: 425px) {
  /*Small smartphones [325px -> 425px]*/
  .header-cont {
    display: flex;
    flex-direction: column;
    row-gap: 1rem;
  }
  #portfolio h1 {
    padding-left: 0;
    font-size: 3rem;
    width: min-content;
  }
}
</style>
