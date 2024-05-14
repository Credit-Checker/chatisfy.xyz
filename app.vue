<template>
  <div>
    <NuxtLayout>
      <NuxtPage/>
    </NuxtLayout>
  </div>
</template>

<script>
export default {
  mounted() {
    this.loadFacebookSDK();
  },
  methods: {
    loadFacebookSDK() {
      // Check if the Facebook SDK script is already loaded
      if (!document.getElementById('facebook-jssdk')) {
        // Load the Facebook SDK script
        const js = document.createElement('script');
        js.id = 'facebook-jssdk';
        js.src = 'https://connect.facebook.net/en_US/sdk.js';
        document.getElementsByTagName('head')[0].appendChild(js);
        
        // Initialize the Facebook SDK
        window.fbAsyncInit = function() {
          FB.init({
            appId: '405263659170044',
            xfbml: true,
            version: 'v19.0'
          });
          FB.AppEvents.logPageView();
        };
      } else {
        // If the Facebook SDK script is already loaded, initialize it immediately
        window.fbAsyncInit();
      }
    }
  }
}
</script>

