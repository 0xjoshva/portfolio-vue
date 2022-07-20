<template>
<section id="contact">
    <h1>Contact</h1>
    <form  action="https://formspree.io/f/xlezqbkp"
  method="POST">
    <label for="namesurname">Full Name <br> <input name="namesurname" type="text" id="fullname"></label>
    <label for="emailaddress">Email Address <br> <input name="emailaddress" type="email" id="email"></label>
    <label for="txtarea" id="txt-lbl">Message <br> <textarea name="txtarea" id="txtarea" cols="60" rows="8"></textarea></label>
    <button type="submit" id="submit-btn">Send Message <i class="bi bi-play-fill"></i></button>
    </form>
</section>
</template>
<script>
export default {
    
}
</script>
<style scoped>
textarea, input:focus{
    resize: none;
    outline: none;
}
    #contact{
        font-family: 'Montserrat', sans-serif;
        background-image: url(../assets/deepmind.jpg);  
        width: 100%;
        height: 100vh;
        color: var(--white);
        padding: 4rem;
    }

    #contact h1{
        font-weight: 600;
        font-size: 60px;
        color: var(--white);
    }
    #submit-btn{
        outline: none;
        border: none;
        font-size: 18px;
        padding: 14px;
        font-weight: 600;
        background: var(--green);
        color: var(--bg-color);
        border-radius: 5px;
        width: fit-content;
        transition: all 0.4s ease-in;
    }
    #submit-btn:hover{
    background: var(--lgreen);
    }
    #fullname{
      background: var(--white);
        width: 20rem;
        height: 3rem;
        border-radius: 5px;
        outline:none;
        border: none;
    }
    #email{
        background: var(--white);
        width: 24rem;
        height: 3rem;
        border-radius: 5px;
        outline:none;
        border: none;
    }

input {
  background-color: rgb(228, 228, 228);
  border: none;
  color: rgb(12, 12, 12);
  font-size: 18px;
  transition: all 0.2s ease-in-out;
  padding-left: 10px;
}
input::after,
input:active,
input:focus {
  border: none;
  outline: none;
  font-size: 22px;
}

#txtarea{
    padding-left: 10px;
    padding-top: 10px;
  background-color: var(--white);
  border: none;
  color: rgb(12, 12, 12);
  transition: all 0.2s ease-in-out;
  border-radius: 10px;
  font-size: 20px;
}
form{
    display: flex;
    flex-direction: column;
    justify-content: center;
    row-gap: 1rem;
    padding-top: 2rem;
    padding-left: 1rem;
}
label{
    font-size: large;
}
label:focus-within > text{
    border: 1px solid var(--green);
}

</style>