<template>
  <q-page class="bg-secondary">


<div class="bg-primary">
          <div class="row q-gutter-md">
            <div class=" text-white col-12 col-md-6 q-pt-md text-center q-mt-xl">
              <p class="text-accent text-h5 text-weight-bolder">
                 &lt; Hello World! /&gt;
              </p>
              <p class="text-h6 text-bold"> It's </p>
              <p translate="no" class="text-bold gt-sm text-h2 text-center">
                Michael
                <p class="text-orange text-weight-regular">Iheajumbu</p>
              </p>

                <!-- mobile -->
              <p translate="no" class="text-bold lt-sm text-h2 text-center">
                Michael
                <p class="text-orange text-weight-regular">Iheajumbu</p>
              </p>
              <h1 class="text-italic">
                I'm a
                <span class="typed-text text-weight-bolder">
                  {{ typeValue }}
                </span>
                <span class="cursor" :class="{ typing: typeStatus }"
                  >&nbsp;</span
                >
              </h1>

              <!-- Hero Contact me button  -->
              <div class="q-gutter-md">
                <q-btn
                  color="accent"
                  label="Contact Me"
                  outline
                  rounded
                  size="xl"
                  type="a"
                  target="_blank"
                   href="mailto:michaeliheajumbu@gmail.com"
                  no-caps
                  style="width: 280px"
                >

                </q-btn>
                <q-btn
                  color="white"
                  rounded
                  no-caps
                  flat
                  type="a"
                  href="#services"
                  push
                  icon="fas fa-chevron-circle-down"
                  text-color="accent"
                  label="Ways I can help you"
                />
              </div>
            </div>
            <div class="bg lt-sm col-12 col-md-6 q-pl-xl">
              <q-avatar   size="245px">
                <img alt="Michael Iheajumbu" src="~assets/me.png" />
              </q-avatar>
            </div>
            <div class="bg gt-sm col-12 col-md">
              <q-avatar  size="500px">
                <img alt="Michael Iheajumbu" src="~assets/me.png"  />
              </q-avatar>
            </div>
          </div>
</div>
    <div class="q-ma-none">
      <img alt="wave" src="~assets/wave.svg" class="bg-primary" />
    </div>

    <!-- portfolio section -->
    <div class="bg-secondary q-p-lg text-black">
      <q-card flat class="transparent">
        <p class="text-center text-bold text-h3 q-pt-md">Portfolio</p>

        <q-card-section class="row">
          <q-card-section class="col-12 col-md-4">
            <q-img class="col-12" src="~assets/dev.svg" />
          </q-card-section>
          <q-card-section class="q-my-md col-12 col-md">
            <q-option-group
              v-model="Portfolio"
              inline
              size="lg"
              color="accent"
              :options="[
                { label: 'About Me', value: 'aboutMe' },
                { label: 'Skill', value: 'skill' },
                { label: 'Education', value: 'education' },
              ]"
            />

            <q-tab-panels v-model="Portfolio" animated class="transparent">
              <q-tab-panel name="aboutMe">
                <div class="q-pa-md text-justify">
                  <p>
                    Hello, my name is
                    <b>Michael,</b>
                  </p>
                  <p class="my-font text-weight-light">
                    I work as a resourceful and customer-focused Product
                    Designer and Software Developer. I can assist you in
                    digitalizing your idea or company's brand while increasing sales and
                    reach.
                  </p>
                  <p class="text-weight-light">
                    My strengths as an individual are analytical thinking and a
                    constant desire to learn new technologies. I enjoy being a
                    part of any creative team that allows me to hone my
                    communication and coding abilities.
                  </p>

                  <div>
                    <q-btn
                      outline
                      rounded
                      color="accent"
                      type="a"
                      href="#contact"
                      push
                      label="Contact"
                    />
                  </div>
                </div>
              </q-tab-panel>

              <q-tab-panel name="skill">
                <div>
                  <p class="text-weight-light text-right">
                    Don't worry much about this... It just shows that I'm
                    constantly learning and keeping up with the latest
                    technologies so that I can choose the best tech for the job.
                  </p>
                </div>
                <div class="q-gutter-sm">
                  <q-chip
                    clickable
                    outline
                    class="shadow-4"
                    color="accent"
                    text-color="white"
                    icon="fab fa-figma"
                    >Figma</q-chip
                  >
                  <q-chip
                    clickable
                    outline
                    class="shadow-4"
                    color="accent"
                    text-color="white"
                    icon="fab fa-html5"
                    >HTML</q-chip
                  >
                  <q-chip
                    clickable
                    outline
                    class="shadow-4"
                    color="accent"
                    text-color="white"
                    icon="fab fa-css3-alt"
                    >CSS</q-chip
                  >
                  <q-chip
                    clickable
                    outline
                    class="shadow-4"
                    color="accent"
                    text-color="white"
                    icon="fab fa-js-square"
                    >Javascript</q-chip
                  >
                  <q-chip
                    clickable
                    outline
                    class="shadow-4"
                    color="accent"
                    text-color="white"
                    icon="fab fa-vuejs"
                    >VueJs</q-chip
                  >
                  <q-chip
                    clickable
                    outline
                    class="shadow-4"
                    color="accent"
                    text-color="white"
                  >
                    <img alt="quasar logo" src="~assets/quasar.svg" />
                    Quasar Framework
                  </q-chip>
                </div>
              </q-tab-panel>

              <q-tab-panel name="education">
                <q-card flat class="my-card transparent">
                  <q-card-section>
                    <q-timeline color="accent">
                      <q-timeline-entry
                        title="HIGHER NATIONAL DIPLOMA IN COMPUTER SCIENCE"
                        side="left"
                        subtitle="2018 - 2020"
                      >
                        <div class="text-weight-light text-italic">
                          Federal Polytechnic Bida, Niger State, Nigeria
                          <div class="text-subtitle1">
                            Upper Credit With a CGPA of 3.3/4.0.
                          </div>
                        </div>
                      </q-timeline-entry>
                      <q-timeline-entry
                        title="NATIONAL DIPLOMA IN COMPUTER SCIENCE"
                        side="right"
                        subtitle=" 2014 - 2016"
                      >
                        <div class="text-weight-light text-italic">
                          Federal Polytechnic Bida, Niger State, Nigeria
                          <div class="text-subtitle1">
                            Upper Credit With a CGPA of 3.4/4.0.
                          </div>
                        </div>
                      </q-timeline-entry>
                      <q-timeline-entry>
                         <q-btn color="accent" rounded outline label="View my Resume" />

                      </q-timeline-entry>
                    </q-timeline>
                  </q-card-section>
                </q-card>
              </q-tab-panel>
            </q-tab-panels>
          </q-card-section>
        </q-card-section>
      </q-card>
    </div>

    <!-- services I offer section -->
    <div id="services" class="q-my-xl q-mx-md q-pt-md">
      <p class="text-h3 q-mt-xl text-bold q-ml-xl">Ways I can help you</p>

      <div class="q-py-xl">
        <div class="row q-pa-md q-gutter-s">
          <!-- design -->
          <div class="col-12 col-md-3 ">
            <q-card bordered class="transparent firstCard">
              <q-card-section class="q-pt-xl q-mt-xl q-pl-xl">
                <img alt="figma logo" src="~assets/figma.svg" />
              </q-card-section>

              <q-card-section class="q-pl-xl q-mb-xl">
                <div class="text-h5 q-my-lg q-mb-xs text-bold">
                  Designing a digital product for you
                </div>
                <div class="text-weight-light text-justify">
                  From product design (UI/UX) to strategy, I use design to
                  prototype solutions to complex problems and assist you in
                  meeting your business objectives.
                </div>
              </q-card-section>
            </q-card>
          </div>

          <div class="col-12 col-md-3">
            <q-card bordered flat class="secondCard transparent myCard">
              <q-card-section class="q-pt-xl q-mt-xl q-pl-xl">
                <img
                  alt="employee Management logo"
                  src="~assets/employeeManagement.png"
                  style="height: 60px; width: 70px"
                />
              </q-card-section>

              <q-card-section class="q-pl-xl q-mb-xl">
                <div class="text-h5 q-my-lg q-mb-xs text-bold">
                  Developing a userfriendly digital workspace
                </div>
                <div class="text-weight-light text-justify">
                  Yes, I can create an easy-to-use organisational platforms that
                  can be used to solve complex everyday business problems while
                  having an easy sync of information across multiple
                  departments/outlets in your organization, thus helping you
                  achieve your business goals faster and more effienciently.
                </div>
              </q-card-section>
            </q-card>
          </div>

          <div class="col-12 col-md-3">
            <q-card bordered class="thirdCard transparent myCard">
              <q-card-section class="q-pt-xl q-mt-xl q-pl-xl">
                <img
                  alt="ecommerce logo"
                  src="~assets/ecommerce.png"
                  style="height: 60px; width: 100px"
                />
              </q-card-section>

              <q-card-section class="q-pl-xl q-mb-xl">
                <div class="text-h5 q-my-lg q-mb-xs text-bold">
                  Building an effiecient ecommerce platform
                </div>
                <div class="text-weight-light text-justify">
                  I build high-quality visually appealing ecommerce platforms
                  that significantly boost your sales. Remember that no matter
                  what you're selling, an ecommerce platform can help you easily
                  reach your potential customers faster with ease. The best part
                  is that the ecommerce platforms will be equipped with payment
                  processors that will allow you to receive funds in any
                  currency of your choosing.
                </div>
              </q-card-section>
            </q-card>
          </div>

          <div class="col-12 col-md-3">
            <q-card bordered flat class="fourthCard transparent q-pb-md">
              <q-card-section class="q-pt-xl q-mt-xl q-pl-xl">
                <img
                  alt="system management logo"
                  src="~assets/sysmgt.png"
                  style="height: 60px; width: 90px"
                />
              </q-card-section>

              <q-card-section class="q-pl-xl q-mb-xl">
                <div class="text-h5 q-my-lg q-mb-xs text-bold">
                  Manage and Maintain the digital product for you
                </div>
                <div class="text-weight-light">
                  What happens after you've created your website? Of course,
                  management! My website management services ensure that you are
                  always online, 24 hours a day, seven days a week. Never let a
                  sale or an inquiry from a client pass you by. One of the
                  services I provide under management is the addition of content
                  to your website upon request, among other things. Contact me
                  today and let's get your website up to speed and in good
                  health.
                </div>
              </q-card-section>
            </q-card>
          </div>
        </div>
      </div>
    </div>



    <!-- contact me form -->
    <div id="contact" class="q-pa-xl q-gutter-xs text-center">
      <div>
        <p class="text-h3 text-bold">
          That’s it! Now it’s your turn to say hi.
        </p>
        <div class="text-weight-light">
          Feel free to just click and send me an email or contact me via my
          social handles. &#128522;
        </div>

        <div class="q-mt-md">
          <q-list padding>
            <q-item
              clickable
              v-ripple
              tag="a"
              target="_blank"
              href="mailto:michaeliheajumbu@gmail.com"
            >
              <q-item-section avatar>
                <q-icon color="primary" name="far fa-envelope-open" />
              </q-item-section>
              <q-item-section>
                <q-item-label overline>Email</q-item-label>
                <q-item-label>michaeliheajumbu@gmail.com</q-item-label>
              </q-item-section>
            </q-item>
          </q-list>
          <q-list padding>
            <q-item
              clickable
              v-ripple
              tag="a"
              target="_blank"
              href="https://www.linkedin.com/in/michael-iheajumbu-69a43b19a"
            >
              <q-item-section avatar>
                <q-icon color="primary" name="fab fa-linkedin-in" />
              </q-item-section>
              <q-item-section>
                <q-item-label overline>Linkedin Profile</q-item-label>
                <q-item-label>Michael Iheajumbu</q-item-label>
              </q-item-section>
            </q-item>
          </q-list>
          <q-list padding>
            <q-item
              clickable
              v-ripple
              tag="a"
              target="_blank"
              href="https://github.com/thri60"
            >
              <q-item-section avatar>
                <q-icon color="primary" name="fab fa-github" />
              </q-item-section>
              <q-item-section>
                <q-item-label overline>Github</q-item-label>
                <q-item-label>@thri60</q-item-label>
              </q-item-section>
            </q-item>
          </q-list>
          <q-list padding>
            <q-item
              clickable
              v-ripple
              tag="a"
              target="_blank"
              href="https://twitter.com/thri60"
            >
              <q-item-section avatar>
                <q-icon color="primary" name="fab fa-twitter" />
              </q-item-section>
              <q-item-section>
                <q-item-label overline>Twitter</q-item-label>
                <q-item-label>@thri60</q-item-label>
              </q-item-section>
            </q-item>
          </q-list>
        </div>
      </div>
    </div>

 <!-- place QPageScroller at end of page -->
          <q-page-scroller position="bottom-right" :scroll-offset="150" :offset="[18, 18]">
            <q-btn fab icon="keyboard_arrow_up" color="accent" />
          </q-page-scroller>
  </q-page>
</template>

<script>
import { defineComponent, ref } from "vue";
import useClipboard from "vue-clipboard3";

export default defineComponent({
  components: {},

  setup() {

    return {
      typeValue: ref(""),
      typeStatus: ref("false"),
      typeArray: ref(["Product Designer", "Software Developer", "Freelancer"]),
      typingSpeed: ref(100),
      erasingSpeed: ref(100),
      newTextDelay: ref(2000),
      typeArrayIndex: ref(0),
      charIndex: ref(0),

      services: ref("writing"),
      slide: ref(1),
      skill: ref("ContentWriting"),
      autoplay: ref("true"),
      Portfolio: ref("aboutMe"),


    };
  },
  methods: {
    typeText() {
      if (this.charIndex < this.typeArray[this.typeArrayIndex].length) {
        if (!this.typeStatus) this.typeStatus = true;

        this.typeValue += this.typeArray[this.typeArrayIndex].charAt(
          this.charIndex
        );
        this.charIndex += 1;

        setTimeout(this.typeText, this.typingSpeed);
      } else {
        this.typeStatus = false;
        setTimeout(this.eraseText, this.newTextDelay);
      }
    },
    eraseText() {
      if (this.charIndex > 0) {
        if (!this.typeStatus) this.typeStatus = true;

        this.typeValue = this.typeArray[this.typeArrayIndex].substring(
          0,
          this.charIndex - 1
        );
        this.charIndex -= 1;
        setTimeout(this.eraseText, this.erasingSpeed);
      } else {
        this.typeStatus = false;
        this.typeArrayIndex += 1;
        if (this.typeArrayIndex >= this.typeArray.length)
          this.typeArrayIndex = 0;

        setTimeout(this.typeText, this.typingSpeed + 500);
      }
    },
  },

  created() {
    setTimeout(this.typeText, this.newTextDelay + 100);
  },
});
</script>

<style lang="scss" scoped>
.bg {
  background: url("../assets/blob.svg") center no-repeat;
  height: 100%;
}

/* begining of Typer writer effect*/

h1 {
  font-size: 2rem;
  font-weight: bolder;
  text-shadow: 40;

  span.typed-text {
    color: #fca311;
  }
  span.cursor {
    display: inline-block;
    margin-left: 3px;
    width: 4px;
    background-color: #fff;
    animation: cursorBlink 1s infinite;
  }

  span.cursor.typing {
    animation: none;
  }
}
/* End of Typer writer effect*/

.firstCard{
  height: 550px;
}
.secondCard{
  height: 650px;
}
.thirdCard{
  height: 750px;
}
.fourthCard{
  height: 850px;
}





@keyframes cursorBlink {
  49% {
    background-color: #fff;
  }
  50% {
    background-color: transparent;
  }
  99% {
    background-color: transparent;
  }
}
</style>
