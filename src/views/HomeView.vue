<template>

  <div class="flex justify-center items-start mt-8 flex-row-reverse lg:pl-64">
      <div class="sugg-fixed-sm max-md:hidden">
        <suggComp />
      </div>
    <div class="-center-col max-sm:w-full">
      <storyComp />
      <reelComp />
    </div>
  </div>
</template>

<script>
import storyComp from "../components/storyComp.vue"
import reelComp from "../components/reelComp.vue"
import suggComp from "../components/suggComp.vue"

export default {
  name: 'HomeView',
  components: {
    storyComp,
    reelComp,
    suggComp,
  },
}
</script>

<style>

  .full-w-switch {
    width: 100vw;
    height: 100vh;
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    background-color: rgba(0, 0, 0, 0.3);
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .full-w-unfollow {
    width: 100vw;
    height: 100vh;
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    background-color: rgba(0, 0, 0, 0.3);
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .full-w-threedots {
    width: 100vw;
    height: 100vh;
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    background-color: rgba(0, 0, 0, 0.3);
    display: flex;
    justify-content: center;
    align-items: center;
  }

</style>