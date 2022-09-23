<template>
    <div>
      <div class="container">
          <div class="row">
              <div class="col s12"></div>
              <div class="col s12">
                  <div class=" white darken-4">
                      <div class="card-content">
                        <h6 class="center black-text" style="font-weight:500;">
                            Hi, Welcome
                        </h6>
                        <p class="center" style="font-weight:500;">
                            Kindly fill out your information to get you started.
                        </p>
                        <h6 class="left black-text" style="font-weight:500; margin-bottom: 20px;">
                            Personal, Information
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
                                    <input type="text" class="black-text" placeholder="" id="firstname" ref="firstname">
                                    <label for="firstname">First Name</label>
                                </div>
                            </div>
                            <div class="row">
                                <div class="input-field col s12">
                                    <input type="text" class="black-text" placeholder="" id="lastname" ref="lastname">
                                    <label for="lastname">Last Name</label>
                                </div>
                            </div>
                            <div class="row">
                                <div class="input-field col s12">
                                    <input type="text" class="black-text" placeholder="" id="phonenumber" ref="phonenumber">
                                    <label for="phonenumber">Phone Number</label>
                                </div>
                            </div>
                            <div class="row">
                                <div class="input-field col s12">
                                    <input type="password" class="black-text" placeholder="" id="password">
                                    <label for="password">Password</label>
                                </div>
                            </div>
                            <div class="row">
                                <div class="input-field col s12">
                                    <input type="password" class="black-text" placeholder="" id="confirmpassword">
                                    <label for="confirmpassword">Confirm Password</label>
                                </div>
                            </div>
                            <div class="row">
                                <div class="input-field col s12">
                                    <button class="customButtonColor btn btn-large right">
                                        Create Account
                                    </button>
                                </div>
                                <div class="col s12 right-align">
                                    Have an account? <nuxt-link class="orange-text" to="./login" style="font-size:17px">Login</nuxt-link>
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