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
export default {
    
}
</script>
<style scoped>
#experience{
 height: fit-content;
  background: var(--bg-color);
}
#blocks{
display:flex;
flex-direction:row;
column-gap: 2rem;
padding-top: 4em;
padding-bottom: 4em;
display: flex;
justify-content: center;
}
.block{
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
.block:hover{
  height: 400px;
  border: 2px solid var(--green);
}
.block i{
font-size: 2.4rem;
padding-right: 1rem;
}
#block-text h3{
  font-size: 3rem;
}
#block-text h6{
  font-size: 1.4rem;
}

#calender{
  padding-top: 0.2rem;
  font-size: 2rem;
}
</style>