<template>

    <div class="full-w-threedots" v-if="toggle_w_threedots" ref="w_threedots">
        <div class="threedots-fixed h-[384px] w-[400px] bg-white -center-col rounded-xl">
        <div class="single-choice h-12 w-full -center  border-b border-[219, 219, 219]">
            <p class="font-sans font-semibold text-sm text-red-500"> Report </p>
        </div>
        <div class="single-choice h-12 w-full -center">
            <p class="font-sans font-semibold text-sm text-red-500"> Unfollow </p>
        </div>
        <div class="single-choice h-12 w-full -center border-t border-[219, 219, 219]">
            <p class="font-sans font-light text-s"> Add to favorites </p>
        </div>
        <div class="single-choice h-12 w-full -center border-t border-[219, 219, 219]">
            <p class="font-sans font-light text-sm"> Go to post </p>
        </div>
        <div class="single-choice h-12 w-full -center border-t border-[219, 219, 219]">
            <p class="font-sans font-light text-sm"> Share to... </p>
        </div>
        <div class="single-choice h-12 w-full -center border-t border-[219, 219, 219]">
            <p class="font-sans font-light text-sm"> Copy link </p>
        </div>
        <div class="single-choice h-12 w-full -center border-t border-[219, 219, 219]">
            <p class="font-sans font-semlightibold text-sm"> Embed </p>
        </div>
        <div class="single-choice h-12 w-full -center border-t border-[219, 219, 219]" @click="close_threedots">
            <p class="font-sans font-semlightibold text-sm"> Cancel </p>
        </div>
        </div>
    </div>

    <div class="warp-reel">
        <!-- First reel -->
        <div class="reel h-full border border-slate-200 rounded-md flex -center flex-col mt-5">
                <div class="person-de h-14 flex justify-center items-center">
                    <div class="reel-icons-img h-10 w-10 flex justify-center items-center">
                        <img src="https://i.pinimg.com/originals/dc/04/5f/dc045f68cbb786ec97c1f7281dc83643.jpg" alt="reel-icon-img" class="rounded-full h-8 w-8">
                    </div>
                    <div class="reel-acc-info ml-1 flex justify-center items-center flex-col h-10 pl-1">
                        <div class="reel-account-name w-full h-5 flex justify-start items-center">
                            <p class="font-thin text-sm"> MasterOfAlune </p>
                        </div>
                        <div class="reel-account-username flex justify-start items-center h-5 w-full">
                            <p class="font-thin text-xs"> DeathGuns#525 </p>
                        </div>
                    </div>
                    <div class="more-options w-10 h-10 flex justify-center items-center" @click="toggleThreeDots">
                        <i class="fa-solid fa-ellipsis"></i>
                    </div>
                </div>
                <div class="reel-img">
                    <img src="https://i.pinimg.com/originals/46/ae/f8/46aef8ac37957c677eabf4ed78a5fc67.jpg" alt="reel-img">
                </div>
                <div class="reel-tools h-full">
                    <div class="reel-interactions h-12 flex justify-between items-center">
                        <div class="left-side flex justify-center items-center">
                            <div class="left-side-first flex justify-center items-center h-10 w-10">
                                <i class="fa-regular fa-heart text-xl"></i>
                            </div>
                            <div class="left-side-sec flex justify-center items-center h-10 w-10">
                                <i class="fa-regular fa-comment text-xl"></i>
                            </div>
                            <div class="left-side-third flex justify-center items-center h-10 w-10">
                                <i class="fa-regular fa-paper-plane text-xl"></i>
                            </div>
                        </div>
                        <div class="right-side flex justify-center items-center h-10 w-10">
                            <i class="fa-regular fa-bookmark text-xl"></i>
                        </div>
                    </div>
                    <div class="reel-like h-4 flex justify-start items-center pl-3 mt-1">
                        <p> 20 <span class="text-base"> Likes </span> </p>
                    </div>
                    <div class="reel-bio flex justify-center items-center">
                        <p class="reel-bio-text text-sm text-left w-11/12 mr-5 mt-2 font-light"> <span class="text-ms font-medium font-sans"> Dinkndots </span> : Garfield #Yuumi bc I refuse to take #skintober2022 too seriously this year Lul <span class="-more font-thin text-ms"> <br/> .... more</span> </p>
                    </div>
                    <div class="reel-comments flex justify-center items-center">
                        <p class="reel-comments-text text-ms text-left w-11/12 mr-5 mt-1"> View all 271 comments </p>
                    </div>
                    <div class="reel-date-trans h-full flex justify-start items-center mt-2">
                        <p class="reel-date-text ml-3"> OCTOBER 21 <span class="text-xs font-medium ml-2 text-black font-sans"> See translate </span> </p>
                    </div>
                    <div class="reel-comment-tools h-12 w-full flex justify-center items-center mt-3.5 border-t border-slate-200">
                        <div class="emojis-div w-10 h-10 flex justify-center items-center text-2xl">
                            <i class="fa-regular fa-face-smile"></i>
                        </div>
                        <div class="comment-input h-10 flexl justify-center items-center">
                            <input type="text" placeholder="Add a comment..." class="w-full pl-2 h-10 outline-none" autocomplete="off">
                        </div>
                        <div class="send-div  w-10 h-10 flex justify-center items-center" >
                            <p class="text-blue-200 text-sm mr-0.5"> Post</p>
                        </div>
                    </div>
                </div>
        </div>

        <!-- Sec reel -->
        <div class="reel h-full border border-slate-200 rounded-md flex justify-center items-center flex-col mt-5">
                <div class="person-de h-14 flex justify-center items-center">
                    <div class="reel-icons-img-unactive h-10 w-10 flex justify-center items-center">
                        <img src="https://i.pinimg.com/originals/cd/d1/96/cdd196f17b42b38564b307b0a4a09134.jpg" alt="reel-icon-img" class="rounded-full h-8 w-8">
                    </div>
                    <div class="reel-acc-info ml-1 flex justify-center items-center flex-col h-10 pl-1">
                        <div class="reel-account-name w-full h-5 flex justify-start items-center">
                            <p class="font-thin text-sm"> Jacku-chan </p>
                        </div>
                        <div class="reel-account-username flex justify-start items-center h-5 w-full">
                            <p class="font-thin text-xs"> JackTheTroller </p>
                        </div>
                    </div>
                    <div class="more-options w-10 h-10 flex justify-center items-center">
                        <i class="fa-solid fa-ellipsis"></i>
                    </div>
                </div>
                <div class="reel-img">
                    <img src="https://i.pinimg.com/originals/d5/ee/be/d5eebea57bd966cdc46fd1a31fca3218.jpg" alt="reel-img">
                </div>
                <div class="reel-tools h-full">
                    <div class="reel-interactions h-12 flex justify-between items-center">
                        <div class="left-side flex justify-center items-center">
                            <div class="left-side-first flex justify-center items-center h-10 w-10">
                                <i class="fa-regular fa-heart text-xl"></i>
                            </div>
                            <div class="left-side-sec flex justify-center items-center h-10 w-10">
                                <i class="fa-regular fa-comment text-xl"></i>
                            </div>
                            <div class="left-side-third flex justify-center items-center h-10 w-10">
                                <i class="fa-regular fa-paper-plane text-xl"></i>
                            </div>
                        </div>
                        <div class="right-side flex justify-center items-center h-10 w-10">
                            <i class="fa-regular fa-bookmark text-xl"></i>
                        </div>
                    </div>
                    <div class="reel-like h-4 flex justify-start items-center pl-3 mt-1">
                        <p> 2500 <span class="text-base"> Likes </span> </p>
                    </div>
                    <div class="reel-bio flex justify-center items-center">
                        <p class="reel-bio-text text-sm text-left w-11/12 mr-5 mt-2 font-light"> <span class="text-ms font-medium font-sans"> Jacku-chan </span> : Words of the day(mostly verdbs): 1. Walk: aruku. <br/> 2. Sit: suwaru. <br/> 3. Drink: nomu. <br/> 4. Look: miru. <br/> 5. Stop: tomaru <br/> Ex: Watashi wa aruku(I will walk) <br/> Watashi wa miru(I will look) <span class="-more font-thin text-ms"> <br/> .... more</span> </p>
                    </div>
                    <div class="reel-comments flex justify-center items-center">
                        <p class="reel-comments-text text-ms text-left w-11/12 mr-5 mt-1"> View all 21 comments </p>
                    </div>
                    <div class="reel-date-trans h-full flex justify-start items-center mt-2">
                        <p class="reel-date-text ml-3"> OCTOBER 19 <span class="text-xs font-medium ml-2 text-black font-sans"> See translate </span> </p>
                    </div>
                    <div class="reel-comment-tools h-12 w-full flex justify-center items-center mt-3.5 border-t border-slate-200">
                        <div class="emojis-div w-10 h-10 flex justify-center items-center text-2xl">
                            <i class="fa-regular fa-face-smile"></i>
                        </div>
                        <div class="comment-input h-10 flexl justify-center items-center">
                            <input type="text" placeholder="Add a comment..." class="w-full pl-2 h-10 outline-none" autocomplete="off">
                        </div>
                        <div class="send-div  w-10 h-10 flex justify-center items-center" >
                            <p class="text-blue-200 text-sm mr-0.5"> Post</p>
                        </div>
                    </div>
                </div>
        </div>
    </div>

</template>

<script>
export default {
  data() {
    return {
      toggle_w_threedots : false
    }
  },
  methods: {

    toggleThreeDots() {
      this.toggle_w_threedots = !this.toggle_w_threedots
    },

    close_threedots() {
        this.toggle_w_threedots = false
    },

    documentClick(e){
      let el = this.$refs.w_threedots
      let target = e.target
      if ( el == target) {
        this.toggle_w_threedots=false
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

    .reel {
        width: 470px;
    }

    .reel-icons-img {
        background: linear-gradient(white, white) padding-box,
                    linear-gradient(to right, #fcb045, #fd1d1d, #833ab4) border-box;
        border-radius: 50em;
        border: 2px solid transparent;
    }

    .reel-acc-info {
        width: 360px;
        height: 42px;
    }
    
    .reel-img {
        width: 470px;
    }

    .reel-interactions {
        width: 470px;
    }

    .-more {
        color: #8e8e8e;
    }

    .reel-comments-text {
        color: #8e8e8e;
    }

    .reel-date-trans {
        width: 470px;
    }

    .reel-date-text {
        font-size: 10px;
        color: #8e8e8e;
    }

    .comment-input {
        width: 377px;
    }

</style>