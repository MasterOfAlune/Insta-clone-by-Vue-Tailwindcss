<template>

  <div class="full-w-switch" v-if="toggleSwitch" ref="w_switch">
    <div class="middle-screen-fixed-switch h-64 w-96 rounded-xl -center-col overflow-hidden bg-white">
        <div class="title-and-close w-96 h-10 flex justify-end items-center text-base font-semibold font-sans border-b border-gray-300">
          <div class="content-inside w-80 -center">
            <p> Switch accounts </p>
          </div>
          <div class="cross-fixed -center h-10 w-10" @click="close_switch">
            <p class="text-2xl"> <i class="fa-solid fa-xmark"></i> </p>
          </div>
        </div>
        <div class="all-accounts-div w-full h-[166px] -flex items-center flex-col justify-start">
          <div class="single-acc-div-fixed h-[72px] w-full flex justify-between items-center" style="padding: 8px 16px;">
            <div class="fixed-in-fixed -center h-14">
              <img src="https://i.pinimg.com/originals/dc/04/5f/dc045f68cbb786ec97c1f7281dc83643.jpg" alt="account-img" class="h-14 w-14  rounded-full">
              <p class="ml-3"> masterofalune </p>
            </div>
            <div class="icon-fif">
              <i class="fa-solid fa-circle-check text-2xl"></i>
            </div>
          </div>
        </div>
        <div class="login-into-ex w-full h-[50px] -center border-t border-gray-300">
          <p class="text-[#0095f6]"> Log into an Existing Account </p>
        </div>
        <div class="bg-black-overlay">
        </div>
    </div>
  </div>

  <div class="full-w-unfollow" v-if="toggle_w_unfollow" ref="w_unfollow">
    <div class="unfollow-div h-[310px] w-[400px] border bg-white rounded-xl">
      <div class="fixed-unfo h-[214px] w-full flex flex-col justify-around items-center">
        <div class="img-unfollow mt-4">
          <img src="https://i.pinimg.com/736x/4f/4d/3f/4f4d3f63a4ea015a8f63daec3f9da691.jpg" alt="unfollow-img" class="w-24 h-24">
        </div>
        <div class="p-unfollow h-11 w-full text-xs font-sans font-light -center mb-2">
          <p class="w-[300px]"> If you change your mind, you'll have to request to follow @clueless again. </p>
        </div>
      </div>
      <div class="btm-btn-unfollow h-24 w-full -center-col">
        <button class="h-12 w-full border-t border-[219, 219, 219] -center" @click="unfollow_pos_abs"> <p class="text-red-500 font-sans font-semibold"> Unfollow </p> </button>
        <button class="h-12 w-full border-t border-[219, 219, 219] -center" @click="close_unfollow"> <p class="font-sans font-light"> Cancel </p> </button>
      </div>
    </div>
  </div>

  <div class="sugg-for-you w-80 h-96 ml-8 mt-4">
    <div class="personal-account w-80 h-14 flex justify-center items-center">
        <div class="personal-account-img h-14 w-14">
            <img src="https://i.pinimg.com/originals/dc/04/5f/dc045f68cbb786ec97c1f7281dc83643.jpg" alt="personal-account-img" class="rounded-full w-14 h-14">
        </div>
        <div class="personal-account-info w-52 flex text-left justify-center flex-col h-14 text-sm ml-5">
            <p> MasterOfAlune </p>
            <p style="color : #8e8e8e"> DeathGuns#525</p>
        </div>
        <div class="personal-account-switch h-14 w-14 flex justify-center items-center text-xs">
            <p style="color : #0095f6" class="font-sans font-medium" @click="toggle_w_switch"> Switch </p>
        </div>
    </div>
    <div class="sugg-all flex justify-between items-center mt-3.5">
        <p class="font-sans font-medium" style="font-size : 14px; color : #8e8e8e;"> Suggestions For You </p>
        <div class="sugg-see-all  w-14 flex justify-center items-center text-xs font-medium font-sans">
            <p> See All </p>
        </div>
    </div>

    <div class="fixed-random-ppl-sugg pt-2">

    <div class="random-ppl-sugg h-12 w-80 flex justify-between items-center">
        <div class="fixed-random-ppl flex justify-center items-center">
            <div class="random-ppl-img  h-10 w-10 flex justify-center items-center">
                <img src="https://i.pinimg.com/736x/4f/4d/3f/4f4d3f63a4ea015a8f63daec3f9da691.jpg" alt="random-ppl-img" class="h-8 w-8 rounded-full">
            </div>
            <div class="random-ppl-username text-left ml-2">
                <p class="font-medium text-sm font-sans"> Clueless </p>
                <p class="font-light text-xs font-sans"> Followed by Jacku-chan + 1 more</p>
            </div>
        </div>
        <div class="random-ppl-follow h-10 w-10 flex justify-center items-center mr-1.5">
            <p class="font-sans text-xs font-medium" id="tsu" style="color : #0095f6" @click=toggleSliderUnfollow> Follow </p>
        </div>
    </div>

    <div class="random-ppl-sugg h-12 w-80 flex justify-between items-center">
    <div class="fixed-random-ppl flex justify-center items-center">
        <div class="random-ppl-img  h-10 w-10 flex justify-center items-center">
            <img src="https://i.pinimg.com/originals/67/ca/cd/67cacd4f7c659de114c48a3b180be48c.jpg" alt="random-ppl-img" class="h-8 w-8 rounded-full">
        </div>
        <div class="random-ppl-username text-left ml-2">
            <p class="font-medium text-sm font-sans"> Ruthelio </p>
            <p class="font-light text-xs font-sans"> Followed by Jacku-chan + 1 more</p>
        </div>
    </div>
    <div class="random-ppl-follow h-10 w-10 flex justify-center items-center mr-1.5">
        <p class="font-sans text-xs font-medium" style="color : #0095f6"> Follow </p>
    </div>

    </div>

    <div class="random-ppl-sugg h-12 w-80 flex justify-between items-center">
        <div class="fixed-random-ppl flex justify-center items-center">
            <div class="random-ppl-img  h-10 w-10 flex justify-center items-center">
                <img src="https://i.pinimg.com/originals/fc/9a/61/fc9a616dd64463906f226b8d809b4277.jpg" alt="random-ppl-img" class="h-8 w-8 rounded-full">
            </div>
            <div class="random-ppl-username text-left ml-2">
                <p class="font-medium text-sm font-sans"> Shotar </p>
                <p class="font-light text-xs font-sans"> Followed by Jacku-chan + 1 more</p>
            </div>
        </div>
        <div class="random-ppl-follow h-10 w-10 flex justify-center items-center mr-1.5">
            <p class="font-sans text-xs font-medium" style="color : #0095f6"> Follow </p>
        </div>
    </div>

    <div class="random-ppl-sugg h-12 w-80 flex justify-between items-center">
        <div class="fixed-random-ppl flex justify-center items-center">
            <div class="random-ppl-img  h-10 w-10 flex justify-center items-center">
                <img src="https://i.pinimg.com/originals/d2/7e/83/d27e839ee16c7842bba7393a4cc953bd.jpg" alt="random-ppl-img" class="h-8 w-8 rounded-full">
            </div>
            <div class="random-ppl-username text-left ml-2">
                <p class="font-medium text-sm font-sans"> Mikaku </p>
                <p class="font-light text-xs font-sans"> Followed by Jacku-chan + 1 more</p>
            </div>
        </div>
        <div class="random-ppl-follow h-10 w-10 flex justify-center items-center mr-1.5">
            <p class="font-sans text-xs font-medium" style="color : #0095f6"> Follow </p>
    </div>
    </div>

    <div class="random-ppl-sugg h-12 w-80 flex justify-between items-center">
        <div class="fixed-random-ppl flex justify-center items-center">
            <div class="random-ppl-img  h-10 w-10 flex justify-center items-center">
                <img src="https://i.pinimg.com/736x/18/2a/f1/182af19ded8a897887184a097e2930c0.jpg" alt="random-ppl-img" class="h-8 w-8 rounded-full">
            </div>
            <div class="random-ppl-username text-left ml-2">
                <p class="font-medium text-sm font-sans"> Mei </p>
                <p class="font-light text-xs font-sans"> Followed by Jacku-chan + 1 more</p>
            </div>
        </div>
        <div class="random-ppl-follow h-10 w-10 flex justify-center items-center mr-1.5">
            <p class="font-sans text-xs font-medium" style="color : #0095f6"> Follow </p>
    </div>
    </div>
        <div class="sugg-footer text-xs font-light font-sans text-left" style="color: #8e8e8e">
            <p class="mt-6"> About · Help · Press · API · Jobs · PrivacyTerms · Locations · Language
            </p>
            <p class="mt-5"> © 2022 INSTAGRAM FROM META </p>
        </div>
    </div>

  </div>

</template>

<script>
export default {
  data() {
    return {
      toggleSwitch : false,
      toggle_w_unfollow : false,
    }
  },
  methods: {

    toggle_w_switch() {
        this.toggleSwitch = !this.toggleSwitch
    },

    toggleSliderUnfollow() {
      let TSUchecker = document.getElementById("tsu").innerHTML
      if(TSUchecker == " Follow ") {
        document.getElementById("tsu").innerText = " Following "
        document.getElementById("tsu").style.color = "black"
      }
      if (TSUchecker == " Following ") {
        this.toggle_w_unfollow = !this.toggle_w_unfollow
      }
    },

    close_switch() {
        this.toggleSwitch = false
    },

    unfollow_pos_abs() {
        document.getElementById("tsu").innerHTML = " Follow "
        document.getElementById("tsu").style.color = "#0095f6"
        this.toggle_w_unfollow = !this.toggle_w_unfollow
    },

    close_unfollow() {
        this.toggle_w_unfollow = false
    },

    documentClick(e){
      let el = this.$refs.w_unfollow
      let el2 = this.$refs.w_switch
      let target = e.target
      if ( el == target) {
        this.toggle_w_unfollow=false
      }
      if ( el2 == target) {
        this.toggleSwitch=false
      }
    }
  },
    created () {
      document.addEventListener('click', this.documentClick)
    },
    destroyed () {
    // important to clean up!!
    document.removeEventListener('click', this.documentClick)
  }
}
</script>

<style>

</style>