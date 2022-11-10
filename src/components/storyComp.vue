<template>
  <div class="story-div h-32 border border-slate-200 rounded-md flex justify-start items-center">
    <div class="fixed-story-div h-24 w-16">
        <div class="flexable-stories  h-24 w-16 flex justify-center items-center flex-col  ml-5">
            <div class="story-img-active  w-16 flex justify-center items-center border-2 rounded-full h-16">
                <img src="https://i.pinimg.com/originals/dc/04/5f/dc045f68cbb786ec97c1f7281dc83643.jpg" alt="single-story-img" class="w-14 h-14 rounded-full">
            </div>
            <div class="username-story w-16 flex justify-center items-center">
                <p class="text-xs mt-2 h-3 stories-names"> MasterOfAlune </p>
            </div>
        </div>
    </div>

    <div class="fixed-story-div h-24 w-16 ml-5">
        <div class="flexable-stories  h-24 w-16 flex justify-center items-center flex-col  ml-5">
            <div class="story-img border-slate-200   w-16 flex justify-center items-center border-2 rounded-full h-16">
                <img src="https://i.pinimg.com/originals/cd/d1/96/cdd196f17b42b38564b307b0a4a09134.jpg" alt="single-story-img" class="w-14 h-14 rounded-full">
            </div>
            <div class="username-story w-16 flex justify-center items-center">
                <p class="text-xs mt-2 h-3 stories-names"> Jacku-chan </p>
            </div>
        </div>
    </div>

  </div>
</template>

<script>
export default {

}
</script>

<style>

    .story-div {
        width: 470px;
    }

    .story-img-active {
        background: linear-gradient(white, white) padding-box,
                    linear-gradient(to right, #fcb045, #fd1d1d, #833ab4) border-box;
        border-radius: 50em;
        border: 4px solid transparent;
    }

    .stories-names {
        color: #8e8e8e;
    }

</style>