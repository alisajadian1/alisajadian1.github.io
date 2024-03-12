<template>
  <section class="about-area section-padding sky-blue" id="about">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-lg-6 d-none d-lg-block">
          <div class="img-about">
            <img src="@/assets/aboutphoto.jpg" alt="" class="img-fluid" />
          </div>
        </div>
        <div class="col-lg-6 col-md-12">
          <div class="about-details">
            <div class="section-title mb-50">
              <h2>About Me</h2>
            </div>
            <p>
              I'm Ali Sajadian, a Frontend Developer passionate about creating
              seamless digital experiences. With a background in HTML, CSS, and
              JavaScript, I specialize in the Vue.js framework. Formerly a
              Content Specialist and Graphic Designer, I bring a unique blend of
              creativity and technical expertise to my work.
            </p>
            <ul class="about-info mt-4">
              <li>
                <span>Name:</span>
                <span>Ali Sajadian</span>
              </li>
              <li>
                <span>Age:</span>
                <span>26 Years Old</span>
              </li>
              <li>
                <span>Location:</span>
                <span>Shiraz - Iran</span>
              </li>
              <li>
                <span>Email:</span>
                <span>alisajadian98@gmail.com</span>
              </li>
            </ul>
            <div class="download-btn mt-5">
              <a href="#" class="btn1 radius-btn">Download CV</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script></script>

<style>
:root {
  --primary-color: #3498db; /*(a shade of blue)*/
  --accent-color: #e74c3c; /*(a shade of red)*/
  --background-color: #ecf0f1; /*(a light gray/blue) */
  --text-color: #2c3e50; /*(a dark gray/blue) */
}

section {
  display: block;
}

.about-area {
  background-color: var(--background-color);
  /* background-color: #f9f9ff; */
}

.section-padding {
  padding: 90px 0;
}

.about-area .img-about img {
  outline: 10px solid var(--accent-color);
  /* outline: 10px solid #90acd1; */
  outline-offset: -54px;
  border: 44px solid transparent;
  border-width: 0px 10px 0px 85px;
  vertical-align: middle;
}

.img-fluid {
  max-width: 100%;
  height: auto;
}

.about-area .section-title {
  text-align: left;
}

.section-title h2 {
  color: #222222;
  font-weight: 700;
  position: relative;
  margin-bottom: 70px;
  font-size: 45px;
  line-height: 44px;
}

.about-area .section-title h2::before,
.about-area .section-title h2::after {
  left: 0;
  transform: translateX(0);
}

.section-title h2:before {
  bottom: -31px;
  width: 100px;
  height: 2px;
}

.section-title h2:before,
.section-title h2:after {
  content: "";
  position: absolute;
  background-color: #e45447;
}

.section-title h2:after {
  bottom: -35px;
  width: 10px;
  height: 10px;
  border-radius: 8px;
}

ul {
  list-style: none;
}

.about-area .about-details .about-info li {
  display: flex;
  margin-bottom: 10px;
}

.about-area .about-details .about-info li span:first-child {
  font-size: 16px;
  font-weight: 600;
  color: #222222;
  width: 100px;
}

.about-area .about-details .about-info li span {
  width: calc(100% - 100px);
}
</style>
