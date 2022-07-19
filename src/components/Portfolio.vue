<template>
  <section id="portfolio">
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
 
    <div class="header-cont">
      <div class="headers">
      <h1>Featured</h1>
      <h4><span>Recently Added</span></h4>
      </div>
      <div>
        <i class="fa-solid fa-fire-flame-curved"></i>
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
  height: 100vh;
  width: 100%;
  color: var(--white);
}
#portfolio h1{
  color: var(--white);
  font-family: 'Montserrat', sans-serif;
}
.fa-fire-flame-curved{
background-color: #FAD961;
background-image: linear-gradient(13deg, #FAD961 0%, #F76B1C 70%,  #f72e1c 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-size: 5rem;
  padding-left: 1rem;

}

.header-cont{
  display: flex;
  flex-direction: row;
}
.headers{
  display: flex;
  flex-direction: column;
}
.headers h4{
  align-self: flex-end;
  color:var(--white);
  background: #ff0c0c;
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


</style>