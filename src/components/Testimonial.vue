<template>
<section id="testimonial">
    <h1>Testimonials</h1>
<div class="container">
    <hr>
    <div class="item">
        <img src="../assets/jason.jpg" alt="">
        <div id="txt-container">
        <h3>Jason Wandrag</h3>
        <h6>Lecturer</h6>
        <p><i class="fa-solid fa-quote-left"></i> Joshua Steed has shown great dedication to constantly improving himself and his work. He is consistent and hardworking, which shows in the quality of work he produces. <i class="fa-solid fa-quote-right"></i></p>
        <hr>
        </div>
    </div>
    <div class="item">
        <img src="../assets/vusumzi.jpg" alt="">
        <div id="txt-container">
        <h3>Vusumzi Msengana</h3>
        <h6>Classmate</h6>
        <p><i class="fa-solid fa-quote-left"></i> Joshua is a hardworking and consistent person, he likes thinking outside the box and has great creative abilities. <i class="fa-solid fa-quote-right"></i></p>
        <hr>
        </div>
    </div>
    <div class="item">
        <img src="../assets/lihle.jpg" alt="">
        <div id="txt-container">
        <h3>Lihle Goliath</h3>
        <h6>Classmate</h6>
        <p><i class="fa-solid fa-quote-left"></i> Focused and diligent to his work. Has a great eye for creativity and visualization towards his ideas, this means he knows what he want in life. He would be a great assert wherever he goes. <i class="fa-solid fa-quote-right"></i></p>
        <hr>
        </div>
    </div>
    <div class="item">
        <img src="../assets/sindile.jpg" alt="">
        <div id="txt-container">
        <h3>Sindile Kula</h3>
        <h6>Classmate</h6>
        <p><i class="fa-solid fa-quote-left"></i> Joshua is a bright young man with a creative mind. He like to accomplish things at his own pace and according to his own preferences. He is highly diligent and hardworking when it comes to his career. <i class="fa-solid fa-quote-right"></i></p>
        <hr>
        </div>
    </div>
    <div class="item">
        <img src="../assets/raaid.jpg" alt="">
        <div id="txt-container">
        <h3>Raaid Abdullatief</h3>
        <h6>Classmate</h6>
        <p><i class="fa-solid fa-quote-left"></i> One of the most hardworking and committed people I've worked with. You can see the passion in his projects as you scroll down the page. Always a pleasure to work with. <i class="fa-solid fa-quote-right"></i></p>
        <hr>
        </div>
    </div>
    <div class="item">
        <img src="../assets/tristan.jpg" alt="tristan">
        <div id="txt-container">
        <h3>Tristan Daniels</h3>
        <h6>Classmate</h6>
        <p><i class="fa-solid fa-quote-left"></i> Joshua is a passionate and  goal-driven person. He always focuses on the task at hand and works to the best of his ability <i class="fa-solid fa-quote-right"></i></p>
        <hr>
        </div>
    </div>

</div>
</section>
</template>
<script>
export default {

}
</script>
<style scoped> 
    #testimonial{
        width: 100%;
        height: fit-content;
        background: var(--bg-color);
        padding-bottom: 6em;
        padding-top: 6em;
        font-family: 'Montserrat', sans-serif;
    }
 #testimonial h1{
    color: var(--white);
    font-weight: 400;
    text-align:center;
 }
 .container{
display: flex;
flex-direction: column;
margin: 0 auto;
}
 .item{
display: flex;
flex-direction:row;

 }
hr{
    background: linear-gradient(to right,var(--bg-color), rgb(95, 95, 95), var(--bg-color));
    margin-bottom: 2em;
    margin-top:2em;
}
img{
    margin-right: 1rem;
    width: 50px;
    height: 50px;
    border-radius: 50%;
box-shadow: -2px 2px 0px 1px rgba(0,228,114,1);
-webkit-box-shadow: -2px 2px 0px 1px rgba(0,228,114,1);
-moz-box-shadow: -2px 2px 0px 1px rgba(0,228,114,1);
}
#txt-container h3{
    color: var(--white);
}
#txt-container h6{ 
color: rgb(218, 218, 218);
    font-size: 20px;
}
 #txt-container p{
    color: var(--lgrey);
 }
#txt-container i{
    color: var(--green);
}
</style>