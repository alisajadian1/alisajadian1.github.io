<template>
  <section class="resume-area section-padding" id="resume">
    <div class="container">
      <div class="row mb-50">
        <div class="col-lg-12">
          <div class="section-title">
            <h2>Resume</h2>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-lg-3 d-none d-lg-block">
          <nav id="navi">
            <ul>
              <li>
                <a
                  href="#education"
                  :class="{ current: activeSection === 'Education' }"
                  >Education</a
                >
              </li>
              <li>
                <a
                  href="#experience"
                  :class="{ current: activeSection === 'Experience' }"
                  >Experience</a
                >
              </li>
              <li>
                <a
                  href="#skills"
                  :class="{ current: activeSection === 'Skills' }"
                  >Skills</a
                >
              </li>
            </ul>
          </nav>
        </div>
        <div class="col-lg-9 col-md-12">
          <div class="page one" id="page-1">
            <h3 class="heading">Education</h3>
            <div class="resume-wrap transition d-flex">
              <div
                class="icon d-flex align-items-center justify-content-center"
              >
                <span class="icon-graduation">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    width="1.5em"
                    height="1.5em"
                    viewBox="0 0 16 16"
                  >
                    <path
                      fill="white"
                      d="M16 6.28a1.23 1.23 0 0 0-.62-1.07l-6.74-4a1.27 1.27 0 0 0-1.28 0l-6.75 4a1.25 1.25 0 0 0 0 2.15l1.92 1.12v2.81a1.28 1.28 0 0 0 .62 1.09l4.25 2.45a1.28 1.28 0 0 0 1.24 0l4.25-2.45a1.28 1.28 0 0 0 .62-1.09V8.45l1.24-.73v2.72H16zm-3.73 5L8 13.74l-4.22-2.45V9.22l3.58 2.13a1.29 1.29 0 0 0 1.28 0l3.62-2.16zM8 10.27l-6.75-4L8 2.26l6.75 4z"
                    />
                  </svg>
                </span>
              </div>
              <div class="text ps-3">
                <span class="date">2016-2021</span>
                <h4>Bachelor in Mechanical Engineering</h4>
                <span class="position">Shiraz University</span>
                <p>
                  Lorem ipsum, or lipsum as it is sometimes known, is dummy text
                  used in laying out print, graphic or web designs. The passage
                  is attributed to an unknown typesetter in the 15th century who
                  is thought to have.
                </p>
              </div>
            </div>
            <div class="resume-wrap transition d-flex">
              <div
                class="icon d-flex align-items-center justify-content-center"
              >
                <span class="icon-graduation">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    width="1.5em"
                    height="1.5em"
                    viewBox="0 0 16 16"
                  >
                    <path
                      fill="white"
                      d="M16 6.28a1.23 1.23 0 0 0-.62-1.07l-6.74-4a1.27 1.27 0 0 0-1.28 0l-6.75 4a1.25 1.25 0 0 0 0 2.15l1.92 1.12v2.81a1.28 1.28 0 0 0 .62 1.09l4.25 2.45a1.28 1.28 0 0 0 1.24 0l4.25-2.45a1.28 1.28 0 0 0 .62-1.09V8.45l1.24-.73v2.72H16zm-3.73 5L8 13.74l-4.22-2.45V9.22l3.58 2.13a1.29 1.29 0 0 0 1.28 0l3.62-2.16zM8 10.27l-6.75-4L8 2.26l6.75 4z"
                    />
                  </svg>
                </span>
              </div>
              <div class="text ps-3">
                <span class="date">2021-2022</span>
                <h4>Cs50</h4>
                <span class="position">Harvard University</span>
                <p>
                  Lorem ipsum, or lipsum as it is sometimes known, is dummy text
                  used in laying out print, graphic or web designs. The passage
                  is attributed to an unknown typesetter in the 15th century who
                  is thought to have.
                </p>
              </div>
            </div>
            <div class="resume-wrap transition d-flex">
              <div
                class="icon d-flex align-items-center justify-content-center"
              >
                <div
                  class="icon d-flex align-items-center justify-content-center"
                >
                  <span class="icon-graduation">
                    <svg
                      xmlns="http://www.w3.org/2000/svg"
                      width="1.5em"
                      height="1.5em"
                      viewBox="0 0 16 16"
                    >
                      <path
                        fill="white"
                        d="M16 6.28a1.23 1.23 0 0 0-.62-1.07l-6.74-4a1.27 1.27 0 0 0-1.28 0l-6.75 4a1.25 1.25 0 0 0 0 2.15l1.92 1.12v2.81a1.28 1.28 0 0 0 .62 1.09l4.25 2.45a1.28 1.28 0 0 0 1.24 0l4.25-2.45a1.28 1.28 0 0 0 .62-1.09V8.45l1.24-.73v2.72H16zm-3.73 5L8 13.74l-4.22-2.45V9.22l3.58 2.13a1.29 1.29 0 0 0 1.28 0l3.62-2.16zM8 10.27l-6.75-4L8 2.26l6.75 4z"
                      />
                    </svg>
                  </span>
                </div>
              </div>
              <div class="text ps-3">
                <span class="date">2022-2023</span>
                <h4>JavaScript & Vue</h4>
                <span class="position">Udemy</span>
                <p>
                  Lorem ipsum, or lipsum as it is sometimes known, is dummy text
                  used in laying out print, graphic or web designs. The passage
                  is attributed to an unknown typesetter in the 15th century who
                  is thought to have.
                </p>
              </div>
            </div>
          </div>
          <div class="page two" id="page-2">
            <h3 class="heading">Experience</h3>
            <div class="resume-wrap transition d-flex">
              <div
                class="icon d-flex align-items-center justify-content-center"
              >
                <span class="icon-briefcase"></span>
              </div>
              <div class="text ps-3">
                <span class="date">2014-2015</span>
                <h4>Software Developer</h4>
                <span class="position">Mansoura University</span>
                <p>
                  Lorem ipsum, or lipsum as it is sometimes known, is dummy text
                  used in laying out print, graphic or web designs. The passage
                  is attributed to an unknown typesetter in the 15th century who
                  is thought to have.
                </p>
              </div>
            </div>
            <div class="resume-wrap transition d-flex">
              <div
                class="icon d-flex align-items-center justify-content-center"
              >
                <span class="icon-briefcase"></span>
              </div>
              <div class="text ps-3">
                <span class="date">2014-2015</span>
                <h4>Software Developer</h4>
                <span class="position">Mansoura University</span>
                <p>
                  Lorem ipsum, or lipsum as it is sometimes known, is dummy text
                  used in laying out print, graphic or web designs. The passage
                  is attributed to an unknown typesetter in the 15th century who
                  is thought to have.
                </p>
              </div>
            </div>
            <div class="resume-wrap transition d-flex">
              <div
                class="icon d-flex align-items-center justify-content-center"
              >
                <span class="icon-briefcase"></span>
              </div>
              <div class="text ps-3">
                <span class="date">2014-2015</span>
                <h4>Software Developer</h4>
                <span class="position">Mansoura University</span>
                <p>
                  Lorem ipsum, or lipsum as it is sometimes known, is dummy text
                  used in laying out print, graphic or web designs. The passage
                  is attributed to an unknown typesetter in the 15th century who
                  is thought to have.
                </p>
              </div>
            </div>
          </div>
          <div class="page three" id="page-3">
            <h3 class="heading">Skills</h3>
            <div class="row">
              <div class="col-md-6">
                <div class="progress-wrap">
                  <h5>HTML & CSS</h5>
                  <div class="break-line"></div>
                </div>
              </div>
              <div class="col-md-6">
                <div class="progress-wrap">
                  <h5>JavaScript</h5>
                  <div class="break-line"></div>
                </div>
              </div>
              <div class="col-md-6">
                <div class="progress-wrap">
                  <h5>Vue</h5>
                  <div class="break-line"></div>
                </div>
              </div>
              <div class="col-md-6">
                <div class="progress-wrap">
                  <h5>Nuxt</h5>
                  <div class="break-line"></div>
                </div>
              </div>
              <div class="col-md-6">
                <div class="progress-wrap">
                  <h5>Git</h5>
                  <div class="break-line"></div>
                </div>
              </div>
              <!-- <div class="col-md-6">
                <div class="progress-wrap">
                  <h5>Photoshop</h5>
                  <div class="break-line"></div>
                </div>
              </div> -->
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      activeSection: "Education",
    };
  },
  methods: {
    changeResumeSection() {
      const scrollPosition = window.scrollY;
      console.log(scrollPosition);

      if (scrollPosition < 2400) {
        this.activeSection = "Education";
      } else if (2400 < scrollPosition && scrollPosition < 3200) {
        this.activeSection = "Experience";
      } else {
        this.activeSection = "Skills";
      }
    },
  },
  mounted() {
    window.addEventListener("scroll", this.changeResumeSection);
  },
};
</script>

<style>
.resume-area {
  background-color: #fff;
}

.section-padding {
  padding: 90px 0;
}

.mb-50 {
  margin-bottom: 50px;
}

.section-title {
  text-align: center;
}

.section-title h2 {
  color: #222222;
  font-weight: 700;
  position: relative;
  margin-bottom: 70px;
  font-size: 45px;
  line-height: 44px;
}

.section-title h2::before {
  bottom: -31px;
  width: 100px;
  height: 2px;
}

.section-title h2:before,
.section-title h2:after {
  content: "";
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  background-color: #e45447;
}

ul {
  list-style: none;
}

#navi {
  top: 180px;
  position: sticky;
  margin: 0;
}

#navi li {
  font-weight: 700;
  margin-bottom: 10px;
}

#navi li a {
  text-decoration: none;
  color: #000000;
}

#navi li a.current {
  color: #90acd1;
  margin-left: 20px;
  position: relative;
}

#navi li a.current::after {
  position: absolute;
  top: 50%;
  left: -24px;
  width: 20px;
  height: 2px;
  content: "";
  transform: translateY(-50%);
  background: #90acd1;
}

.page {
  width: 100%;
  margin-bottom: 3em;
}

.page .resume-wrap:hover {
  background-color: #90acd1;
  color: #fff;
}

.page .heading {
  font-weight: 700;
  margin-bottom: 30px;
}

h3 {
  font-size: 24px;
  font-family: "Poppins", sans-serif;
  color: #222222;
  line-height: 1.5;
}

.page .resume-wrap {
  width: 100%;
  margin-bottom: 30px;
  background-color: #f9f9ff;
  padding: 40px 30px;
  border-radius: 10px;
}

.transition {
  transition: all 0.3s ease 0s;
}

.page .resume-wrap .icon {
  width: 50px;
  height: 50px;
  background-color: #90acd1;
  border-radius: 50%;
}

.page .resume-wrap:hover .icon {
  background-color: #fff;
}

.page .resume-wrap:hover .icon span svg path {
  /* color: #222222; */
  fill: black;
  font-weight: bold;
}

.page .resume-wrap:hover .date {
  color: #fff;
}

.page .resume-wrap .icon span {
  color: #fff;
  font-size: 20px;
}

.icon-graduation {
  /* font-family: "simple-line-icons"; */
  /* speak: none; */
  /* font-style: normal;
  font-weight: normal;
  text-transform: none;
  line-height: 1; */
}

/* .icon-graduation::before {
  content: "\e019";
} */

.icon-briefcase::before {
  content: "\e04b";
}

.page .resume-wrap .text {
  width: calc(100% - 100px);
  padding: 0 0 10px;
}

.page .resume-wrap .date {
  font-weight: 700;
  font-size: 16px;
  color: #222222;
}

.page .resume-wrap h4 {
  font-size: 20px;
  font-weight: 700;
  font-family: "Poppins", sans-serif;
  line-height: 1.5;
}

.page .resume-wrap .position {
  display: inline-block;
  margin-bottom: 10px;
}

.progress-wrap {
  width: 100%;
  margin-bottom: 20px;
}

.progress-wrap h5 {
  font-size: 16px;
  margin-bottom: 15px;
  font-weight: 500;
}

.break-line {
  box-shadow: none;
  height: 4px;
  background: #90acd1 !important;
  overflow: visible;
  width: 30%;
  border-radius: 10px;
}
</style>
