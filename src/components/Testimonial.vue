<template>
  <section id="testimonial">
    
    <div class="container">
      <h1>testimonials</h1>
      <hr />
      <!-- item -->
      <div v-for="testimonial in data" v-bind:key="testimonial.id" class="item">
        <img v-bind:src="testimonial.imageURL" alt="" />
        <div id="txt-container">
          <h3>{{ testimonial.name }}</h3>
          <h6>{{ testimonial.role }}</h6>
          <p>
            <i class="fa-solid fa-quote-left"></i> {{ testimonial.text }}
            <i class="fa-solid fa-quote-right"></i>
          </p>
          <hr />
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import TestimonialDB from "/data/TestimonialDB.json";
export default {
  data() {
    return {
      data: TestimonialDB,
    };
  },
};
</script>
<style scoped>
#testimonial {
  width: 100%;
  height: fit-content;
  background: var(--bg-color);
  padding-bottom: 6em;
  padding-top: 6em;
  font-family: "Montserrat", sans-serif;
  padding-top: 10em;
}
#testimonial h1 {
  color: var(--white);
  font-family: "Montserrat", sans-serif;
  padding-top: 2rem;
  padding-bottom: 1rem;
  font-size: 4rem;
  font-weight: 700;
}
.container {
  display: flex;
  flex-direction: column;
  margin: 0;
  width: 100%;
  margin-left: 8rem;
  margin-right: 8rem;
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
  width: 60px;
  height: 60px;
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

@media only screen and (max-width: 425px){
	/*Small smartphones [325px -> 425px]*/
  #testimonial h1{
        padding-top: 2rem;
  padding-bottom: 1rem;
  font-size: 3rem;
  font-weight: 700;
  }
}
p{
  width: 100%;
}
</style>
