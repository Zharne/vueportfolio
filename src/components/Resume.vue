<template>

  <div id='resume'>
      <div class="main-container">
      <div class="row">
        <div class="col">
          <h1 class="blue-text lighten-1 header">RESUME</h1>
          <hr style="">
          <ul class="timeline">
            <li class="event" data-date="2015">
              <h3>National Senior Certificate(NSC)</h3>
              <h5>Oude Molen Technical High School</h5>
              <p>
                Afrikaans, English, Life Science, Mathematics, Life Orientation, Mechanical Technology, Business Studies.
              </p>
            </li>
            <li class="event" data-date="2016">
              <h3>Internship</h3>
              <h5>Martin & East Pty(Ltd)</h5>
              <p>
                I completed a 1 year interneshhip as a workshop trainee.
              </p>
              <p>Since graduating from university, I have also undertaken responsibilities for designing a product for the company. The roles I have been given have provided the perfect opportunity to implement the skills I have gained throughout my higher
                education, as well as experiencing the running of a successful business.</p>
            </li>
            <li class="event" data-date="2017">
              <h3>N1-N3 Engineering Welding</h3>
              <h5>False Bay TVET College</h5>
              <p>My Nated 3 diploma is incomplete.
              </p>
            </li>
            <li class="event" data-date="2018-2020">
              <h3>Bachelors of Commerce(Gen)</h3>
              <h5>Pearson Institute of Higher Learning</h5>
              <p>I completed my degree </p>
            </li>
            <li class="event" data-date="2021/Present">
              <h3>Coding</h3>
              <h5>Life Choices Coding Academy</h5>
              <p>This is where my interest in building things for interactive media began. During my first computing course I studied a range of core topics including multimedia design, database design, computer games development, computer networks and object
                oriented programming.</p>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

</script>

<style scoped>


.main-container {
  margin-top: 2rem;
  display: flex;
  /* background-color: darkgray; */
  width: 100%;
  justify-content: center;
  align-items: center;
}
.row{
  margin: 2rem;
  width: 80%;
  display: flex;
  justify-content: center;
  align-items: center;
}
#content {
  margin-top: 50px;
  text-align: center;
  margin-left: 300px;
}

section.timeline-outer {
  width: 80%;
  margin: 0 auto;
}

h1.header {
  font-size: 50px;
  line-height: 70px;
}
h3{
  color: blue;
}

/* Timeline */

.timeline {
  border-left: 8px solid #42A5F5;
  border-bottom-right-radius: 2px;
  border-top-right-radius: 2px;
  box-shadow: 0 2px 5px 0 rgba(0, 0, 0, 0.16), 0 2px 10px 0 rgba(0, 0, 0, 0.12);
  color: #333;
  margin: 50px auto;
  letter-spacing: 0.5px;
  position: relative;
  line-height: 1.4em;
  padding: 20px;
  list-style: none;
  text-align: left;
}

.timeline h1,
.timeline h2,
.timeline h3 {
  font-size: 1.4em;
}

.timeline .event {
  border-bottom: 1px solid rgba(160, 160, 160, 0.2);
  padding-bottom: 15px;
  margin-bottom: 20px;
  position: relative;
}

.timeline .event:last-of-type {
  padding-bottom: 0;
  margin-bottom: 0;
  border: none;
}

.timeline .event:before,
.timeline .event:after {
  position: absolute;
  display: block;
  top: 0;
}

.timeline .event:before {
  left: -177.5px;
  color: #212121;
  content: attr(data-date);
  text-align: right;
  /*  font-weight: 100;*/
  
  font-size: 16px;
  min-width: 120px;
}

.timeline .event:after {
  box-shadow: 0 0 0 8px #42A5F5;
  left: -30px;
  background: #212121;
  border-radius: 50%;
  height: 11px;
  width: 11px;
  content: "";
  top: 5px;
}
/**/
/*——————————————
Responsive Stuff
———————————————*/

@media (max-width: 945px) {
  .timeline .event::before {
    left: 0.5px;
    top: 20px;
    min-width: 0;
    font-size: 13px;
  }
  .timeline h3 {
    font-size: 16px;
  }
  .timeline p {
    padding-top: 20px;
  }
  section.lab h3.card-title {
    padding: 5px;
    font-size: 16px
  }
}

@media (max-width: 768px) {
  .timeline .event::before {
    left: 0.5px;
    top: 20px;
    min-width: 0;
    font-size: 13px;
  }
  .timeline .event:nth-child(1)::before,
  .timeline .event:nth-child(3)::before,
  .timeline .event:nth-child(5)::before {
    top: 38px;
  }
  .timeline h3 {
    font-size: 16px;
  }
  .timeline p {
    padding-top: 20px;
  }
}
</style>