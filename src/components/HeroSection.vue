<template>
  <section class="hero-area sky-blue d-flex align-items-center">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-lg-6 col-md-6">
          <div class="hero-caption">
            <span class="subheading">Hey! I am</span>
            <h1>Karim Ezzat</h1>
            <div>
              "I am a"
              <div id="typed-strings" style="display: none">
                <span>Freelancer</span>
                <span>Web Designer</span>
                <span>Developer</span>
                <span>Marketer</span>
              </div>
              <span class="LR-C" id="typed" style="white-space: pre"></span>
              <span class="typed-cursor"></span>
            </div>
            <p>
              Lorem ipsum dolor sit, amet consectetur adipisicing elit.
              Reiciendis molestiae ipsum aliquid explicabo cumque possimus aut
              distinctio eligendi?
            </p>
            <a href="#" class="btn radius-btn">Download</a>
          </div>
        </div>
        <div class="col-lg-6 d-none d-lg-block"></div>
      </div>
    </div>
    <div class="hero-shape custom-animation"></div>
  </section>
</template>

<style>
.hero-area {
  position: relative;
  min-height: 1000px;
}

.sky-blue {
  background: #f9f9ff;
}

.hero-area .hero-caption {
  width: 100%;
}

.hero-area .hero-caption .subheading {
  text-transform: uppercase;
  font-size: 16px;
  font-weight: 700;
  color: #90acd1;
  letter-spacing: 4px;
}

.hero-area .hero-caption h1 {
  font-family: "Poppins", sans-serif;
  color: #222222;
  font-size: 60px;
  font-weight: 700;
}

.hero-area .hero-caption div {
  color: #e45447;
  font-weight: 400;
  font-size: 30px;
  line-height: 42px;
  margin-bottom: 30px;
}

.hero-area .hero-caption p {
  margin-bottom: 45px;
  padding-right: 155px;
}

.btn::before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background: #e45447;
  z-index: 1;
  border-radius: 5px;
  transition: transform 0.5s;
  transform: scale(0);
  transform-origin: 0 0;
  transition-timing-function: cubic-bezier(02, 1.6, 0.4, 0.7);
}

.btn {
  background: #90acd1;
  text-transform: capitalize;
  color: #fff;
  cursor: pointer;
  display: inline-block;
  font-size: 16px;
  font-weight: 400;
  letter-spacing: 1px;
  line-height: 0;
  transition: 0.4s linear;
  position: relative;
  z-index: 1;
  border: 0;
  overflow: hidden;
}

.radius-btn {
  padding: 250px 43px;
  border-radius: 30px;
}
</style>
