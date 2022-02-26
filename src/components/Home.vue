<template>
    <div id='home' style="min-height: 87.2vh; justify-content: center; flex-direction: column; display: flex;"><br>
      <div class='image'>
        <img src="https://i.postimg.cc/Gp5rLhQK/me-shot-min.jpg" style="border-radius:50%">
      </div> 
        <!-- <div class="img-shape aos-init aos-animate" data-aos="fade-up" data-aos-duration="1200"><img src="https://i.postimg.cc/Gp5rLhQK/me-shot-min.jpg" alt="hero image"></div> -->
          <div class="w3-container w3-center w3-animate-top">
            <span class="h1"><h1>Hello! I'm</h1></span> <span class="h2"><h2>ZHARNE DESEMBER</h2></span>
            <span class="h3"><h3>*Web Developer*</h3></span> 
          </div>   
          <div class="row justify-content-center"> <!-- Social Media Links --> 
            <div class="w3-container w3-center w3-animate-bottom">
              <a href="" class="fa fa-instagram" target="_blank"></a>
              <a href="" class="fa fa-github" target="_blank"></a>
            </div>  
          </div>
    </div>
           <h1>I am <span id="text"></span></h1> 
    
  
</template>

<script>

const sentences = [
  "Zharné Desember",
  "an aspiring fullstack developer",
  "enthusiastic about life",
  "a team player",
  "a problem solver",
  "passionate about the great outdoors"
];

function waitForMs(ms) {
  return new Promise((resolve) => setTimeout(resolve, ms));
}

async function typeSentence(sentence, element, delay = 100) {
  const letters = sentence.split("");
  let i = 0;
  while (i < letters.length) {
    await waitForMs(delay);
    document.querySelector(element).append(letters[i]);
    i++;
  }
}

async function deleteSentence(element) {
  const sentence = document.querySelector(element).innerHTML;
  const letters = sentence.split("");
  while (letters.length > 0) {
    await waitForMs(100);
    letters.pop();
    document.querySelector(element).innerHTML = letters.join("");
  }
}


async function sentenceLoop(sentenceList, element) {
  let i = 0;
  while (true) {
    await typeSentence(sentenceList[i], element);
    await waitForMs(1500);
    await deleteSentence(element);
    await waitForMs(500);
    i++;
    if (i >= sentenceList.length) {
      i = 0;
    }
  }
}

sentenceLoop(sentences, "#text");



</script>

<style>
#home{
      /* background: url('https://i.postimg.cc/ryd5c9kk/pexels-tirachard-kumtanom-733857.jpg'); */
      background-size: cover;
      height: 100vh;
      width: 100%;
      /* background:linear-gradient:  ; */
      background-repeat: no-repeat;
      background-attachment: fixed; 
      backface-visibility:visible;
      background-size: 100% 100%;
      /* background-color: darkgray; */
    }

/* .image{
  height: 50vh;
} */
/* #text {
  position: relative;
}

#text:after {
  content: "";
  width: 3px;
  height: 100%;
  background: black;
  position: absolute;
  animation: blink 1s infinite;
} */

@keyframes blink {
  0%,
  49% {
    background: black;
  }
  50%,
  100% {
    background: white;
  }
}


/* .social-icon a {
  color: #fff;
  font-size: 16px;
  margin-right: 15px;
}
.social-icons i {
  height: 40px;
  width: 40px;
  text-align: center;
  line-height: 38px;
  border-radius: 50%;
  /* margin-top: 10vh; */
/* }
.facebook-bg{
  background: #3B5998;
}
.twitter-bg{
  background: #55ACEE;
}
.google-bg{
  background: #DD4B39;
} */ 

</style>