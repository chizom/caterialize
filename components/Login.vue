<template>
    <div>
      <div class="container">
          <div class="row">
              <div class="col s12"></div>
              <div class="col s12">
                  <div class=" white darken-4">
                      <div class="card-content">
                        <h6 class="center" style="font-weight:500;">
                            Sign In
                        </h6>
                          <form @submit.prevent>
                              <div class="row">
                                  <div class="input-field col s12">
                                      <input type="text" class="black-text" placeholder="" id="email" ref="email">
                                      <label for="email">Email</label>
                                  </div>
                              </div>
                              <div class="row">
                                  <div class="input-field col s12">
                                      <input type="password" class="black-text" placeholder="" id="password">
                                      <label for="password">Password</label>
                                  </div>
                              </div>
                              <div class="row">
                                  <div class="input-field col s12 right-align">
                                      <nuxt-link class="black-text" to="./forgot">Forgot Password?</nuxt-link>
                                  </div>
                              </div>
                              <div class="row">
                                  <div class="input-field col s12">
                                      <button class="customButtonColor btn btn-large right" style="width: 100px;">
                                          Login
                                      </button>
                                  </div>
                                  <div class="col s12 center">
                                    Don't have an account? <nuxt-link class="orange-text" to="./signup" style="font-size:17px">Sign Up</nuxt-link>
                                  </div>
                              </div>
                          </form>
                      </div>
                  </div>
              </div>
              <!-- <div class="col s12 m3"></div> -->
          </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
      methods: {
          loadFocus() {
              this.$refs.email.focus()
          }
      },
  
      mounted() {
          this.loadFocus();
      }
  }
  </script>
  
  <style>
  
  </style>