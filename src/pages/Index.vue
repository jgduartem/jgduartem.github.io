<template>
 <div>
    <q-layout view="lHh lpr lFf" style="height: 100vh">
      <q-header reveal>
        <q-toolbar class="bg-dark row">
          <div class="row col-1">
          <q-item>
            <q-avatar size="32px" color="deep-purple" text-color="white">JD</q-avatar>
          </q-item>
          </div>
          <div class="row col-11 justify-end">
            <q-item>
              <q-btn class="q-ma-xs q-mr-sm" flat color="grey-3" label="About Me"/>
              <q-btn class="q-mt-xs" flat color="grey-3" label="Contact" />
            </q-item>   
          </div>
        </q-toolbar>
      </q-header>

      <q-page-container>
        <q-page class="">
          <div class="flex bg-dark text-grey-4 " style="height: 100vh">
            <div id='name'>
              <h1>Jose Duarte</h1>
              <h6 class="row col-12 justify-center">Designing and coding responsive websites</h6>
            </div>
          </div>
          <div class="row justify-center">
            <q-img src="responsive.png" style='height: 400px; max-width: 800px'/>
          </div>
          <div class="bg-white row col-12">
            <p class="q-mt-lg q-mb-lg row col-12 justify-center text-h2">About</p>
            <div class="row col-12" >
              <q-card class="row col-xs-12 col-sm-4 col-md-4 col-lg-4 q-pa-md">
                <q-card-section class="row justify-center" >
                  <q-icon class="q-ma-md" size="80px" name="speed" color="deep-purple"/>
                  <p class="text-body1 text-center">Fast load times and lag free interaction, my highest priority.</p>
                </q-card-section>
              </q-card>
              <q-card class="row col-xs-12 col-sm-4 col-md-4 col-lg-4 q-pa-md">
                <q-card-section class="row justify-center">
                  <q-icon class="q-ma-md" size="80px" name="important_devices" color="deep-purple"/>
                  <p class="text-body1 text-center">My layouts will work on any device, big, medium or small.</p>
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
        </q-page>
      </q-page-container>
    </q-layout>
  </div>
</template>

<script>


export default {
  name: 'PageIndex',
  data() {
    return {

    }
  }
}
</script>

<style>
#name{
  margin-top: 30%;
  margin-left: 5%;
}
</style>
