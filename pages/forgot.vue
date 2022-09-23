<template>
  <div>
    
    <div class="row full-width">
      <div class="col s12 m6" style="margin-top: 130px">
        <Logo/>
        <Forgot/>
      </div>
      
      <div class="col s12 m6 full-width hide-on-small-and-down" :style="{ backgroundImage: `url(${backgroundUrl})` }">

      </div>

    </div>
  </div>
</template>

<script>
  import backgroundUrl from '~/assets/images/angled_background.jpg'
  export default {
    data() {
      return {
        backgroundUrl,
      }
    }
  }
</script>
