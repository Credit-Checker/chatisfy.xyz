<template>
  <div class="banner-wrapper">
    <v-container>
      <!-- -----------------------------------------------
            Start Banner
        ----------------------------------------------- -->
      <v-row justify="center">
        <v-col cols="12" sm="7" lg="6" class="d-flex align-center">
          <div class="text-sm-left text-center">
            <h1 class="banner-title font-weight-bold text-white">
              Chatisfy.xyz
            </h1>
            <h4 class="banner-subtitle white--text font-weight-regular text-white">
              Automate your instagram business chat.
            </h4>
            <div class="mt-md-16 mt-10 d-sm-flex d-block">
              <v-btn
                color="error"
                class="mr-0 mr-sm-5 mb-5 mb-sm-0 btn-custom-md d-sm-flex d-block btn-100"
                size="large"
                flat
              >
                 <NuxtLink to="https://www.wrappixel.com/templates/nextkit-nuxtjs-free-uikit/" target="_blank" class="text-decoration-none  text-white">
                  Get started
                 </NuxtLink>
              </v-btn>
              <v-btn
                size="large"
                to="/coming-soon"
                class="btn-custom-md d-sm-flex d-block"
                variant="outlined"
                color="white"
                flat
              >
                See pricing
              </v-btn>
            </div>
          </div>
        </v-col>
        <v-col cols="12" sm="5" lg="6">
          <img
            src="/images/landingpage/banner-img.png"
            alt="banner" class="img-fluid"
          />
        </v-col>
      </v-row>

      <!-- -----------------------------------------------
            End Banner
        ----------------------------------------------- -->
    </v-container>
  </div>
</template>

