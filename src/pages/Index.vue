<template>
 <div>
    <q-layout view="lHh lpr lFf" style="height: 100vh">
      <q-header reveal>
        <q-toolbar class="bg-dark row col-12 justify-end">
          <q-item>
            <a href="#about">
              <q-btn class="q-ma-xs q-mr-sm" flat color="grey-3" label="About Me"/>
            </a>
            <a href="#projects">
              <q-btn class="q-ma-xs q-mr-sm" flat color="grey-3" label="Projects"/>
            </a>
            <a href="#contact">
              <q-btn class="q-ma-xs q-mr-sm" flat color="grey-3" label="Contact"/>
            </a>
          </q-item>   
        </q-toolbar>
      </q-header>

      <q-page-container>
        <q-page class="">
          <div class="flex bg-dark text-grey-2 " style="height: 100vh">
            <div id='name'>
              <q-intersection>
                <transition appear enter-active-class="animated fadeInLeft">
              <h1>José Duarte</h1>
                </transition>
              </q-intersection>
              <q-intersection>
                <transition appear enter-active-class="animated fadeInLeft">
              <h6 class="row col-12 justify-center">Designing and coding responsive websites and web apps.</h6>
                </transition>
              </q-intersection>
            </div>
          </div>

          <div class="row justify-center bg-dark">
            <q-img src="responsive.png" style='height: auto; max-width: 70%'/>
          </div>

          <q-intersection id="about">
            <transition appear enter-active-class="animated fadeInRight delay-1s" >
          <div  class="bg-grey-2 row col-12">
            <p class="q-mt-lg q-mb-lg row col-12 justify-center text-h2">About</p>
            <div class="row col-12" >
              <q-card class="row col-xs-12 col-sm-4 col-md-4 col-lg-4 q-pa-md">
                <q-card-section class="row justify-center">
                  <q-icon class="q-ma-md" size="80px" name="important_devices" color="deep-purple"/>
                  <p class="text-body1 text-center">My layouts will work on any device, big, medium or small.</p>
                </q-card-section>
              </q-card>
              <q-card class="row col-xs-12 col-sm-4 col-md-4 col-lg-4 q-pa-md">
                <q-card-section class="row justify-center" >
                  <q-icon class="q-ma-md" size="80px" name="speed" color="deep-purple"/>
                  <p class="text-body1 text-center">Fast load times and lag free interaction, my highest priority.</p>
                </q-card-section>
              </q-card>
              <q-card class="row col-xs-12 col-sm-4 col-md-4 col-lg-4 q-pa-md">
                <q-card-section class="row justify-center">
                  <q-icon class="q-ma-md" size="80px" name="emoji_objects" color="deep-purple"/>
                  <p class="text-body1 text-center">Strong preference for easy to use, intuitive UX/UI.</p>
                </q-card-section>
              </q-card>
            </div>
          </div>
            </transition>
          </q-intersection>

          <div class="bg-white row col-12">
            <div class="row col-xs-12 col-sm-6 col-md-6 col-lg-6 justify-center">
              <div class="q-mt-lg flex flex-center">
                <q-avatar class=" bg-deep-purple" size="240px" text-color="white">JD</q-avatar>
                <p class="text-body1 q-ma-md ">I'm a self taught Full-Stack web developer in constant learning. </br>I really enjoy developing web apps and webpages with intuitive user experencie</p>
              </div>
            </div>
            <div class="row col-xs-12 col-sm-6 col-md-6 col-lg-6 justify-center">
              <div class="q-mt-lg row col-12">
                <q-item class="col-12">
                  <q-item-section class="col-2">
                    <q-linear-progress stripe size="25px" :value='1' color="deep-purple" class="q-mt-sm">
                      <div class="absolute-full flex flex-center">
                        <q-badge color="white" text-color="deep-purple" label="HTML" />
                      </div>
                    </q-linear-progress>
                  </q-item-section>
                  <q-item-section class="col-9">
                    <q-linear-progress size="25px" :value="htmlBar" color="deep-purple" class="q-mt-sm"/>
                  </q-item-section>
                </q-item>
                <q-item class="col-12">
                  <q-item-section class="col-2">
                    <q-linear-progress stripe size="25px" :value='1' color="deep-purple" class="q-mt-sm">
                      <div class="absolute-full flex flex-center">
                        <q-badge color="white" text-color="deep-purple" label="CSS" />
                      </div>
                    </q-linear-progress>
                  </q-item-section>
                  <q-item-section class="col-9">
                    <q-linear-progress size="25px" :value="cssBar" color="deep-purple" class="q-mt-sm"/>
                  </q-item-section>
                </q-item>
                <q-item class="col-12">
                  <q-item-section class="col-2">
                    <q-linear-progress stripe size="25px" :value='1' color="deep-purple" class="q-mt-sm">
                      <div class="absolute-full flex flex-center">
                        <q-badge color="white" text-color="deep-purple" label="Javascript" />
                      </div>
                    </q-linear-progress>
                  </q-item-section>
                  <q-item-section class="col-9">
                    <q-linear-progress size="25px" :value="javascriptBar" color="deep-purple" class="q-mt-sm"/>
                  </q-item-section>
                </q-item>
                <q-item class="col-12">
                  <q-item-section class="col-2">
                    <q-linear-progress stripe size="25px" :value='1' color="deep-purple" class="q-mt-sm">
                      <div class="absolute-full flex flex-center">
                        <q-badge color="white" text-color="deep-purple" label="NodeJs" />
                      </div>
                    </q-linear-progress>
                  </q-item-section>
                  <q-item-section class="col-9">
                    <q-linear-progress size="25px" :value="nodejsBar" color="deep-purple" class="q-mt-sm"/>
                  </q-item-section>
                </q-item>
                <q-item class="col-12">
                  <q-item-section class="col-2">
                    <q-linear-progress stripe size="25px" :value='1' color="deep-purple" class="q-mt-sm">
                      <div class="absolute-full flex flex-center">
                        <q-badge color="white" text-color="deep-purple" label="VueJs" />
                      </div>
                    </q-linear-progress>
                  </q-item-section>
                  <q-item-section class="col-9">
                    <q-linear-progress size="25px" :value="vuejsBar" color="deep-purple" class="q-mt-sm"/>
                  </q-item-section>
                </q-item>
                <q-item class="col-12">
                  <q-item-section class="col-2">
                    <q-linear-progress stripe size="25px" :value='1' color="deep-purple" class="q-mt-sm">
                      <div class="absolute-full flex flex-center">
                        <q-badge color="white" text-color="deep-purple" label="UI Design" />
                      </div>
                    </q-linear-progress>
                  </q-item-section>
                  <q-item-section class="col-9">
                    <q-linear-progress size="25px" :value="uiBar" color="deep-purple" class="q-mt-sm"/>
                  </q-item-section>
                </q-item>
                <q-item class="col-12">
                  <q-item-section class="col-2">
                    <q-linear-progress stripe size="25px"  :value='1' color="deep-purple" class="q-mt-sm">
                      <div class="absolute-full flex flex-center">
                        <q-badge color="white" text-color="deep-purple" label="Ruby" />
                      </div>
                    </q-linear-progress>
                  </q-item-section>
                  <q-item-section class="col-9">
                    <q-linear-progress size="25px" :value="rubyBar" color="deep-purple" class="q-mt-sm"/>
                  </q-item-section>
                </q-item>
                <q-item class="col-12">
                  <q-item-section class="col-2">
                    <q-linear-progress stripe size="25px" :value='1' color="deep-purple" class="q-mt-sm">
                      <div class="absolute-full flex flex-center">
                        <q-badge color="white" text-color="deep-purple" label="MongoDB" />
                      </div>
                    </q-linear-progress>
                  </q-item-section>
                  <q-item-section class="col-9">
                    <q-linear-progress size="25px" :value="mongoBar" color="deep-purple" class="q-mt-sm"/>
                  </q-item-section>
                </q-item>
              </div>
            </div> 
          </div>

          <div id="projects" class="q-pa-md text-center bg-grey-2" >
            <h2>Services</h2>
            <div class="row col-12 justify-center">
              <q-card   class="row col-xs-12 col-sm-4 col-md-4 col-lg-4 q-ma-md align-center justify-center" style="height: 400px">
                <q-img src="portfolio.png" style="height: auto; max-width: 100%"/>
                <q-card-section>
                  <div class="text-h6 text-center">Web Pages</div>
                  <div class="text-body2">and landing pages</div>
                  
                </q-card-section>
              </q-card>
              <q-card  class="row col-xs-12 col-sm-4 col-md-4 col-lg-4 q-ma-md align-center justify-center" style="height: 400px">
                <q-img src="web-devices.png" style="height: auto; max-width: 100%"/>
                <q-card-section>
                  <div class="text-h6 text-center">Web Apps</div>
                  <div class="text-body2 text-center">Responsives </div>
                </q-card-section>
                <q-card-section class="flex content-end items-end">
                  
                </q-card-section>
              </q-card>
              <q-card  class="row col-xs-12 col-sm-4 col-md-4 col-lg-4 q-ma-md align-center justify-center" style="height: 400px">
                <q-img src="e-commerce.png" style="height: auto; max-width: 100%"/>
                <q-card-section>
                  <div class="text-h6 text-center">E-Commerce</div>
                  <div class="text-body2 text-center">With shopping cart</div>
                </q-card-section>
                <q-card-section class="flex content-end items-end">
                  
                </q-card-section>
              </q-card>
            </div>
          </div>

          <q-dialog full-width full-height v-model="crm">
            <q-card>
              <q-bar class="bg-deep-purple">
                <q-space />
                <q-btn dense flat icon="close" color="grey-3" v-close-popup>
                  <q-tooltip>Close</q-tooltip>
                </q-btn>
              </q-bar>
              <q-card class="q-ma-xs" style="height: 100vh">
                <q-card-section>
                  <div>
                    <q-carousel
                      swipeable
                      animated
                      v-model="slide"
                      thumbnails
                      infinite
                      height="100vh"
                      width='100vw'
                    >
                      <q-carousel-slide :name="1" img-src="Screenshot1.png" style="height: auto; width: 100%" />
                      <q-carousel-slide :name="2" img-src="Screenshot2.png" style="height: auto; width: 100%" />
                      <q-carousel-slide :name="3" img-src="Screenshot3.png" style="height: auto; width: 100%" />
                      <q-carousel-slide :name="4" img-src="Screenshot4.png" style="height: auto; width: 100%" />
                    </q-carousel>
                  </div>
                </q-card-section>
              </q-card>
            </q-card>
          </q-dialog>

          <q-dialog full-width full-height v-model="empty">
            <q-card class="bg-grey-2">
              <q-bar class="bg-deep-purple">
                <q-space />
                <q-btn dense flat icon="close" color="grey-3" v-close-popup>
                  <q-tooltip>Close</q-tooltip>
                </q-btn>
              </q-bar>
              <q-card-section class="absolute-center text-h2 text-center">
                Our project would be here!
              </q-card-section>
            </q-card>
          </q-dialog>

          <div id="contact" class="flex flex-center content-end items-end bg-dark text-grey-3" >
            <div class="row col-12 justify-between">
              <q-item clickable >
                <q-item-section>
                  <q-icon name="fab fa-instagram" @click="openLink('instagram')" size="24px"/>
                </q-item-section>
              </q-item>
              <q-item clickable >
                <q-item-section>
                  <q-icon name="fab fa-linkedin" @click="openLink('linkedin')" size="24px"/>
                </q-item-section>
              </q-item>
              <q-item clickable >
                <q-item-section>
                  <q-icon name="fab fa-github" @click="openLink('github')" size="24px"/>
                </q-item-section>
              </q-item>
            </div>
          </div>
          <div class="row col-12 text-grey-3 bg-dark justify-center" >Jose Duarte 2020</div>
        </q-page>
      </q-page-container>
    </q-layout>
  </div>
</template>

<script>
export default {
  name: "PageIndex",
  data() {
    return {
      crm: false,
      empty: false,
      slide: 1,
      htmlBar: 0.9,
      cssBar: 0.9,
      javascriptBar: 0.8,
      nodejsBar: 0.7,
      vuejsBar: 0.7,
      uiBar: 0.5,
      rubyBar: 0.5,
      mongoBar: 0.6,
      slide: 1,
    };
  },
  methods: {
    openLink(link) {
      switch (link) {
        case "instagram":
          window.open("https://www.instagram.com/duar.tech");
          break;
        case "linkedin":
          window.open("https://www.linkedin.com/in/-jgduarte/");
          break;
        case "github":
          window.open("https://github.com/jgduartem");
      }
    },
  },
};
</script>

<style>
@media (max-height: 700px) {
  #name {
    margin-top: 30%;
    margin-left: 5%;
  }
}
@media (min-height: 730px) {
  #name {
    margin-top: 35vh;
    margin-left: 5%;
  }
}
@media (min-height: 850px) {
  #name {
    margin-top: 70vh;
    margin-left: 5%;
  }
}
@media (min-height: 1024) {
  #name {
    margin-top: 90%;
    margin-left: 5%;
  }
}
@media (min-height: 1240px) {
  #name {
    margin-top: 60%;
    margin-left: 5%;
  }
}
@media (min-height: 1800px) {
  #name {
    margin-top: 40%;
    margin-left: 5%;
  }
}

#blured {
  filter: blur(3px);
}
#blured:hover {
  filter: blur(0px);
}
a {
  text-decoration: none;
}
#particles-js {
  width: 100%;
  height: 100%;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: 50% 50%;
}
</style>
