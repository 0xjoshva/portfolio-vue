<template>
  <section id="footer">
    <div class="center">
      <div class="foot-links">
        <h3>Pages</h3>
        <ul>
          <li><router-link to="/" class="links">Home</router-link></li>
          <li>
            <router-link to="/projects" class="links">Projects</router-link>
          </li>
          <li>
            <router-link to="/contact" class="links">Contact</router-link>
          </li>
        </ul>
      </div>
      <div class="foot-links">
        <h3>Sections</h3>
        <ul>
          <li><a href="" class="links">Landing</a></li>
          <li><a href="" class="links">About</a></li>
          <li><a href="" class="links">Featured</a></li>
          <li><a href="" class="links">Testimonials</a></li>
        </ul>
      </div>

      <div class="info-item" id="newsletter-wrapper">
        <div>
          <h4 class="text-white">Get in touch.</h4>
        </div>
        <form
          id="newsletter"
          action="https://formspree.io/f/mvolebno"
          method="POST"
        >
          <input
            type="email"
            id="email-input"
            name="E-Mail"
            placeholder="Enter your email"
            required
          />
          <button type="submit" id="email-btn">Send!</button>
        </form>
        <div>
          <p class="fw-light text-white" id="newsletter-notice">
            enter your email if you would like me to reach out to you.
          </p>
        </div>
      </div>
    </div>
    <footer id="footer-container">
      <span class="rights text-white"
        >Designed & Built by Joshua Steed <br />
        Copyright © 2022</span
      >
      <img src="../assets/newlogosimple.png" alt="logo" id="logo-footer" />
      <div class="socials-wrapper">
        <p>hosted by <span>Firebase</span></p>
      </div>
    </footer>
  </section>
</template>
<script>
export default {};
</script>
<style scoped>
footer {
  width: 100% !important;
}

#footer-container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  width: 100% !important;
  height: fit-content;
  background-color: #171616;
  padding-top: 1rem;
  padding-bottom: 1rem;
  padding-left: 8rem;
  padding-right: 8rem;
}

#footer {
  background-color: #222222;
}
.info {
  height: 300px;
  background-color: #fefefe;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  width: 100%;
}

.info h4 {
  font-family: "Roboto", sans-serif;
  font-weight: 400;
  font-size: 18px;
}
.socials-wrapper {
  display: flex;
  flex-direction: row;
  width: fit-content;
  vertical-align: middle;
  align-self: center;
  color: var(--lgrey);
  font-family: "Roboto", sans-serif;
}
.socials-wrapper span {
  color: var(--green);
}
#logo-footer {
  width: auto;
  height: 2.5rem;
}

.rights {
  align-self: center;
  font-weight: 300;
  font-family: "Montserrat", sans-serif;
  font-size: 0.8rem;
}

.bi-facebook:hover {
  color: rgb(199, 199, 199);
}
.bi-twitter:hover {
  color: rgb(199, 199, 199);
}
.bi-instagram {
  color: rgb(199, 199, 199);
}
.bi-linkedin {
  color: rgb(199, 199, 199);
}

a,
a:hover,
a:focus,
a:active {
  text-decoration: none !important;
  color: white !important;
}

.cities {
  display: flex;
  flex-direction: column;
  text-decoration: none;
  row-gap: 10px;
}
.bi-caret-right {
  font-size: 10px;
}

.city {
  font-family: "Roboto", sans-serif;
  font-weight: 500;
  font-size: 14px;
}

.city:hover {
  color: silver;
}

.contact {
  display: flex;
  flex-direction: column;
  row-gap: 10px;
  color: white;
  font-family: "Roboto", sans-serif;
  font-weight: lighter;
  font-size: 14px;
}

#email-input {
  border: none;
  background-color: white;
  resize: none;
  outline: none;
  border-radius: 3px 3px;
  height: 36px;
  width: 300px;
  padding-left: 10px;
}

#email-btn {
  width: 150px;
  height: 38px;
  color: white;
  background-color: #4a4a4a;
  border: none;
  border-radius: 3px 3px;
  font-size: 15px;
  font-weight: 600;
}
#newsletter {
  display: flex;
  flex-direction: row;
  row-gap: 10px;
  column-gap: 30px;
}

#newsletter-wrapper {
  display: flex;
  flex-direction: column;
  padding-top: 1rem;
  padding-bottom: 1rem;
  font-family: "Montserrat", sans-serif;
}
#newsletter-notice {
  font-size: 12px;
  width: 300px;
  padding-top: 1%;
}
.center {
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-family: "Montserrat", sans-serif;
  padding-bottom: 1rem;
  padding-top: 1rem;
  margin-left: 8rem;
  margin-right: 8rem;
}
a.links {
  text-decoration: none;
  color: inherit;
  font-size: 0.8rem;
  border-bottom: 2px solid var(--green);
  font-weight: 300;
}
router-link.links {
  text-decoration: none;
  color: inherit;
  font-size: 0.8rem;
  border-bottom: 2px solid var(--green);
  font-weight: 300;
}
.foot-links h3 {
  font-size: 1.2rem;
  color: var(--white);
}
@media only screen and (max-width: 1200px) {
  #newsletter-wrapper {
    display: none;
  }
}
@media only screen and (max-width: 600px) {
  #newsletter-wrapper {
    display: none;
  }
}
</style>
