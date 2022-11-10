<template>

  <div class="explore w-full h-full -center">
    <div class="fixed-explore h-ful flex justify-evenly items-center flex-wrap w-[60rem] max-md:w-[38.5rem] max-sm:w-[20rem]">

        <div class="one-on-one h-72 w-72 bg-yellow-700 -center" style="background-image: url('https://aniyuki.com/wp-content/uploads/2022/03/aniyuki-cute-anime-avatar-profile-picture-1.jpg')">
            <div class="one-on-one-icons flex justify-center items-center">
                <div class="left-ooo-icon p-6 text-white">
                    <i class="fa-solid fa-heart text-xl"> <span class="font-medium font-sans tex-ms"> 300 </span> </i>
                </div>
                <div class="right-ooo-icon p-6 text-white">
                    <i class="fa-solid fa-comment text-xl"> <span class="font-medium font-sans tex-ms"> 17 </span> </i>
                </div>
            </div>
        </div>

        <div class="one-on-one h-72 w-72 bg-yellow-700 -center" style="background-image: url('https://i.pinimg.com/originals/a8/3e/9e/a83e9eb2bb4b46580ccef7423bad389b.jpg')">
            <div class="black-box">

            </div>
            <div class="one-on-one-icons flex justify-center items-center">
                <div class="left-ooo-icon p-6 text-white">
                    <i class="fa-solid fa-heart text-xl"> <span class="font-medium font-sans tex-ms"> 147 </span> </i>
                </div>
                <div class="right-ooo-icon p-6 text-white">
                    <i class="fa-solid fa-comment text-xl"> <span class="font-medium font-sans tex-ms"> 10 </span> </i>
                </div>
            </div>
        </div>

        <div class="one-on-one h-72 w-72 bg-yellow-700 -center" style="background-image: url('https://i.pinimg.com/736x/ac/18/7c/ac187ca639b0b85468531204dcbe13f7.jpg');">
            <div class="black-box">

            </div>
            <div class="one-on-one-icons flex justify-center items-center">
                <div class="left-ooo-icon p-6 text-white">
                    <i class="fa-solid fa-heart text-xl"> <span class="font-medium font-sans tex-ms"> 222 </span> </i>
                </div>
                <div class="right-ooo-icon p-6 text-white">
                    <i class="fa-solid fa-comment text-xl"> <span class="font-medium font-sans tex-ms"> 104 </span> </i>
                </div>
            </div>
        </div>

        <div class="tall-video bg-red-600  w-72  flex justify-center items-center relative" style="height: 511.68px;">
            <div class="fixed-play-btn absolute top-0 right-0 mt-1 h-10 w-10 -center">
                <i class="fa-solid fa-clapperboard text-[22px] mr-2 text-white"></i>
            </div>
            <video width="300" height="600" controls autoplay loop muted style="pointer-events: none;">
            <source src="../assets/t1-aphelios.mp4" type="video/mp4">
            Your browser does not support the video tag.
            </video>
            <div class="black-box">

            </div>
            <div class="one-on-one-icons flex justify-center items-center">
                <div class="left-ooo-icon p-6 text-white">
                    <i class="fa-solid fa-play text-[18px]"> <span class="font-medium font-sans tex-ms ml-1"> 10,5K </span> </i>
                </div>
                <div class="right-ooo-icon p-6 text-white">
                    <i class="fa-solid fa-comment text-[18px]"> <span class="font-medium font-sans tex-ms ml-1"> 2K </span> </i>
                </div>
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

    .one-on-one, .tall-video {
        background-size: 100%;
        position: relative;
        margin-top : 28px
    }

    .one-on-one-icons {
        position: absolute;
        z-index: 4;
        backface-visibility: hidden;
        visibility: hidden;
    }

    .one-on-one::after, .tall-video::after {
    content: '\A';
    position: absolute;
    width: 100%; height: 100%;
    top:0; left:0;
    background:rgba(0,0,0,0.3);
    opacity: 0;
    z-index: 1;
    }

    .one-on-one:hover:after {
    opacity: 1;
    }   

    .tall-video:hover:after {
    opacity: 1;
    }   

    .one-on-one:hover .one-on-one-icons {
        visibility: visible;
    }

    .tall-video:hover .one-on-one-icons {
        visibility: visible;
    }

</style>