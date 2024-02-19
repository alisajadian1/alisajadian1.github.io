<template>
  <section class="hero-area sky-blue d-flex align-items-center">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-lg-6 col-md-6">
          <div class="hero-caption">
            <span class="subheading">Hey! I am</span>
            <h1>Ali Sajadian</h1>
            <div>
              I'm a {{ printedSkill }}
              <!-- <span class="LR-C" id="typed" style="white-space: pre"></span> -->
              <span class="typed-cursor" :class="{ 'blink-cursor': showCursor }"
                >|</span
              >
            </div>
            <p>
              Lorem ipsum dolor sit, amet consectetur adipisicing elit.
              Reiciendis molestiae ipsum aliquid explicabo cumque possimus aut
              distinctio eligendi?
            </p>
            <a href="#" class="btn1 radius-btn">Download</a>
          </div>
        </div>
        <div class="col-lg-6 d-none d-lg-block"></div>
      </div>
    </div>
    <div class="hero-shape custom-animation"></div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      mySkills: ["Freelancer.", "Developer.", "Web Designer.", "Marketer."],
      printedSkill: "",
      currentWordIndex: 0,
      showCursor: true,
    };
  },
  /* methods: {
    changeTitle() {
      const printingTiming = setInterval(() => {
        if (this.currentWordIndex < this.mySkills.length) {
          let currentSkill = this.mySkills[this.currentWordIndex];

          if (this.currentLetterIndex < currentSkill.length) {
            this.printedSkill += currentSkill[this.currentLetterIndex];
            this.currentLetterIndex++;
          } else {
            // Pause after finishing the subarray
            setTimeout(() => {
              // Deleting the current letter
              this.printedSkill = this.printedSkill.slice(0, -1);

              if (this.printedSkill === "") {
                this.currentWordIndex++;
                this.currentLetterIndex = 0;
                this.printedSkill += " ";
              }
            }, 800);
          }
        } else {
          this.resetData();
        }
      }, 150);
    },
    resetData() {
      this.currentLetterIndex = 0;
      this.currentWordIndex = 0;
      clearInterval(this.printingTiming);
    },
  }, */

  methods: {
    async writeSkill(currentSkill) {
      return new Promise((resolve) => {
        let currentLetterIndex = 0;
        const writingInterval = setInterval(() => {
          if (this.currentLetterIndex < currentSkill.length) {
            this.printedSkill += currentSkill[this.currentLetterIndex];
            this.currentLetterIndex++;
          } else {
            this.currentLetterIndex = 0;
            clearInterval(writingInterval);
            resolve();
          }
        }, 200);
      });
    },

    async deleteSkill() {
      return new Promise((resolve) => {
        const deletingInterval = setInterval(() => {
          if (this.printedSkill !== "") {
            this.printedSkill = this.printedSkill.slice(0, -1);
          } else {
            clearInterval(deletingInterval);
            resolve();
          }
        }, 50);
      });
    },

    async pause(duration) {
      return new Promise((resolve) => setTimeout(resolve, duration));
    },

    async WriteAndDelete() {
      const currentSkill = this.mySkills[this.currentWordIndex];

      await this.writeSkill(currentSkill);
      await this.pause(800);
      await this.deleteSkill();
      await this.pause(300);

      this.currentWordIndex++;
    },

    async changeTitle() {
      while (this.currentWordIndex < this.mySkills.length) {
        await this.WriteAndDelete();
      }

      this.resetData();
      this.changeTitle();
    },

    resetData() {
      this.currentWordIndex = 0;
    },
  },

  mounted() {
    this.changeTitle();
  },
};
</script>

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

.btn1 {
  background: #90acd1;
  text-transform: capitalize;
  color: #fff;
  cursor: pointer;
  display: inline-block;
  font-size: 16px;
  font-weight: 400;
  letter-spacing: 1;
  line-height: 0;
  position: relative;
  z-index: 1;
  border: 0;
  overflow: hidden;
  text-decoration: none;
}

.radius-btn {
  padding: 25px 43px;
  border-radius: 30px;
}

.btn1::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: -1;
  background-color: #e45447;

  transition: transform 300ms ease-in-out;
  transform: scaleX(0);
  transform-origin: left;
}

.btn1:hover::before,
.btn1:focus::before {
  transform: scaleX(1);
}

.blink-cursor {
  animation: blink 0.3s infinite alternate;
}

@keyframes blink {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
</style>
