<template>
  <section id="experience">
    <div id="blocks">
      <div class="block">
        <div id="block-text">
          <h3>4</h3>
          <h6>Languages</h6>
        </div>
        <i class="bi bi-code-square"></i>
      </div>

      <div class="block">
        <div id="block-text">
          <h3>6</h3>
          <h6>Months</h6>
        </div>
        <i class="bi bi-calendar4" id="calender"></i>
      </div>

      <div class="block">
        <div id="block-text">
          <h3>20</h3>
          <h6>Projects</h6>
        </div>
        <i class="bi bi-lightning-charge"></i>
      </div>
    </div>
  </section>
</template>
<script>
export default {};
</script>
<style scoped>
#experience {
  height: fit-content;
  background: var(--bg-color);
}
#blocks {
  display: flex;
  flex-direction: row;
  column-gap: 2rem;
  padding-top: 4em;
  padding-bottom: 4em;
  display: flex;
  justify-content: center;
}
.block {
  color: var(--white);
  font-family: "Montserrat", sans-serif;
  display: flex;
  flex-direction: row-reverse;
  border: 1px solid var(--lgrey);
  padding: 3em 8em 3em 8em;
  border-radius: 10px;
  height: 200px;
  background: var(--bg-color);
  transition: all 1s ease-in-out;
}
.block:hover {
  border: 1px solid var(--green);
}
.block i {
  font-size: 2.4rem;
  padding-right: 1rem;
}
#block-text h3 {
  font-size: 3rem;
}
#block-text h6 {
  font-size: 1.4rem;
}

#calender {
  padding-top: 0.2rem;
  font-size: 2rem;
}
@media only screen and (max-width: 1200px){
    /*Tablets [601px -> 1200px]*/
  #blocks {
    display: flex;
    flex-direction: column;
    row-gap: 2rem;
    padding-left: 2rem;
    align-items: center;
  }
  .block {
  color: var(--white);
  font-family: "Montserrat", sans-serif;
  display: flex;
  flex-direction: row-reverse;
  border: 1px solid var(--lgrey);
  padding-left: 20rem;
  padding-right: 20rem;
  padding-top: 4rem;
  padding-bottom: 4rem;
  margin: 0;
  border-radius: 10px;
  height: fit-content;
  background: var(--bg-color);
  transition: all 1s ease-in-out;
  width: 13rem;
 justify-content: center;}
}

@media only screen and (max-width: 600px) {
  #blocks {
    display: flex;
    flex-direction: column;
    row-gap: 2rem;
    padding-left: 2rem;
    padding-right: 1rem;
  }
    .block {
  color: var(--white);
  font-family: "Montserrat", sans-serif;
  display: flex;
  flex-direction: row-reverse;
  border: 1px solid var(--lgrey);
  padding-left: 13rem;
  padding-right: 13rem;
  padding-top: 4rem;
  padding-bottom: 4rem;
  margin: 0;
  border-radius: 10px;
  height: fit-content;
  background: var(--bg-color);
  transition: all 1s ease-in-out;
  width: 13rem;
 justify-content: center;
 }
}

@media only screen and (max-width: 425px){
    .block {
  color: var(--white);
  font-family: "Montserrat", sans-serif;
  display: flex;
  flex-direction: row-reverse;
  border: 1px solid var(--lgrey);
  padding-left: 10rem;
  padding-right: 10rem;
  padding-top: 4rem;
  padding-bottom: 4rem;
  margin: 0;
  border-radius: 10px;
  height: fit-content;
  background: var(--bg-color);
  transition: all 1s ease-in-out;
  width: 13rem;
 justify-content: center;
 }
}
</style>
