<template>
    <div id="about-me" style="background-color:rgb(148, 148, 148)">
        <div class='container'>
            <div class="row">
                <div class="col-sm-6">
                    <h1>ABOUT ME</h1>
                <div class='content'>
                   <h3>Hi, im Zharne Desember</h3> 
                   <p>I am an adventurous and open-minded person who is willing to learn new things and skills on a daily basis.I am very ambitious and have set goals for myself to achieve in my career and for personal growth, which I worked hard at achieving.</p>
                </div><br>  
                </div>
                <div class="col-sm-6" style="padding-left:100px">
                  <div class='skills'>
                     <h4>This is my skill level</h4>
                          <!-- <small>RWD</small>
                    <div class="progress mb-3" style="height: 15px">
                      <div>
                        class="progress-bar bg-primary"
                        role="progressbar"
                        style="width: 72%"
                        aria-valuenow="72"
                        aria-valuemin="0"
                        aria-valuemax="100"
                      </div>
                    </div>  -->
                    <small>CSS</small>
                    <div class="progress mb-3" style="height: 15px">
                      <div
                        class="progress-bar bg-primary"
                        role="progressbar"
                        style="width: 89%"
                        aria-valuenow="89"
                        aria-valuemin="0"
                        aria-valuemax="100"
                      ></div>
                    </div>
                    <small>HTML</small>
                    <div class="progress mb-3" style="height: 15px">
                      <div
                        class="progress-bar bg-primary"
                        role="progressbar"
                        style="width: 55%"
                        aria-valuenow="55"
                        aria-valuemin="0"
                        aria-valuemax="100"
                      ></div>
                    </div>
                    <small>JS</small>
                    <div class="progress mb-3" style="height: 15px">
                      <div
                        class="progress-bar bg-primary"
                        role="progressbar"
                        style="width: 60%"
                        aria-valuenow="66"
                        aria-valuemin="0"
                        aria-valuemax="100"
                      ></div>
                    </div> 
                    <small>NODE.JS</small>
                    <div class="progress mb-3" style="height: 15px">
                      <div
                        class="progress-bar bg-primary"
                        role="progressbar"
                        style="width: 70%"
                        aria-valuenow="66"
                        aria-valuemin="0"
                        aria-valuemax="100"
                      ></div>
                    </div>
                    <small>MySQL</small>
                    <div class="progress mb-3" style="height: 15px">
                      <div
                        class="progress-bar bg-primary"
                        role="progressbar"
                        style="width: 80%"
                        aria-valuenow="66"
                        aria-valuemin="0"
                        aria-valuemax="100"
                      ></div>
                    </div>
                  <!-- <button class="custom-btn btn-9">More About Me</button> -->
                </div>
                    <!-- <div class='image'>
                        <img src="https://i.postimg.cc/Gp5rLhQK/me-shot-min.jpg" style="border-radius:50%">
                    </div> -->
                </div>
        </div>
    </div>
    </div>

</template>

<style>
#about-me{
  background-color: rgb(148, 148, 148);
  /* padding-bottom: 30px; */
  height: 100vh;
  width: 100%;
  /* background-color: rgba(52, 73, 94, 0.3); */
}
.container{
    height: 90vh;
    margin-left: 200px;
    /* padding-bottom:30px ; */
}

/* Button */
.frame {
  width: 90%;
  margin: 40px auto;
  text-align: center;
}

/* Progress bar */
.bar{
  box-sizing: border-box;
  display: block;
  line-height: 30px;
  position: static;
  z-index: auto;
}
.background{
    position: relative;
    height: 16px;
    border: 1px solid #7e7e7e;
    padding: 2px;
}
.label{
  font-size: 16px;
  font-weight: 5px;
  display: inline-block;
}
.row{
  display: flex;
}

</style>