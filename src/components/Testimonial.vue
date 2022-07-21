<template>
  <section id="testimonial">
    <h1>Testimonials</h1>
    <div class="container">
      <hr />
      <!-- item -->
<div v-for="testimonial in data" v-bind:key="testimonial.id" class="item">
        <img v-bind:src="testimonial.imageURL" alt="" />
        <div id="txt-container">
          <h3>{{ testimonial.name }}</h3>
          <h6>{{ testimonial.role }}</h6>
          <p>
            <i class="fa-solid fa-quote-left"></i>{{ testimonial.text
            }}<i class="fa-solid fa-quote-right"></i>
          </p>
          <hr />
        </div>
      </div>
      
    </div>
  </section>
</template>
<script>
import TestimonialDB from ".//TestimonialDB.json"
export default {
    data() {
        return {
            data: TestimonialDB
        }
    }
}

</script>
<style scoped>
#testimonial {
  width: 100%;
  height: fit-content;
  background: var(--bg-color);
  padding-bottom: 6em;
  padding-top: 6em;
  font-family: "Montserrat", sans-serif;
}
#testimonial h1 {
  color: var(--white);
  font-weight: 400;
  text-align: center;
}
.container {
  display: flex;
  flex-direction: column;
  margin: 0 auto;
}
.item {
  display: flex;
  flex-direction: row;
}
hr {
  background: linear-gradient(
    to right,
    var(--bg-color),
    rgb(95, 95, 95),
    var(--bg-color)
  );
  margin-bottom: 2em;
  margin-top: 2em;
}
img {
  margin-right: 1rem;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  box-shadow: -2px 2px 0px 1px rgba(0, 228, 114, 1);
  -webkit-box-shadow: -2px 2px 0px 1px rgba(0, 228, 114, 1);
  -moz-box-shadow: -2px 2px 0px 1px rgba(0, 228, 114, 1);
}
#txt-container h3 {
  color: var(--white);
}
#txt-container h6 {
  color: rgb(218, 218, 218);
  font-size: 20px;
}
#txt-container p {
  color: var(--lgrey);
}
#txt-container i {
  color: var(--green);
}
</style>
