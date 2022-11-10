<template>

    <div class='mobile-photos mr-8 bg-[url("https://i.ibb.co/ZHcVs5p/It-Tndl-ZM2n2.png")] w-[23.75rem] h-[36.25rem] max-md:hidden' style="background-size: 468.32px 634.15px; background-position: -46px 0;">
    <div class="all-photos h-12 w-full relative">
        <img src="https://i.ibb.co/0nhMM68/screenshot1.png" alt="all-photos" id="im1" class="hidden absolute top-0 right-0 mt-6 mr-4">
        <img src="https://i.ibb.co/NmWmSPr/screenshot2.png" alt="all-photos" id="im2" class="hidden absolute top-0 right-0 mt-6 mr-4">
        <img src="https://i.ibb.co/pj90VJJ/screenshot4.png" alt="all-photos" id="im3" class="hidden absolute top-0 right-0 mt-6 mr-4">
        <img src="https://i.ibb.co/GFGWV6T/screenshot3.png" alt="all-photos" id="im-def" class="absolute top-0 right-0 mt-6 mr-4">
    </div>
    </div>

    <div class="login-div h-[36.25rem] w-[21.875rem] -center-col max-md:scale-1.10">
        
        <div class="login-form h-[25rem] w-full flex items-center flex-col justify-end border border-gray-300 mt-3">

            <div class="logo-fixed-pos h-[6.25rem] mb-5 flex justify-center items-center">
                <div class="logo-insta-login -center">
                    <i data-visualcompletion="css-img" aria-label="Instagram" class="" role="img" style="background-image: url(&quot;https://static.cdninstagram.com/rsrc.php/v3/yw/r/kUy2G4UGM26.png&quot;); background-position: 0px -504px; background-size: 348px 612px; width: 174px; height: 50px; background-repeat: no-repeat; display: inline-block;"></i>
                </div>
            </div>

            <div class="elements-fixed-pos -center-col  h-[15.625rem]">
                <div class="forms-login">
                    <div class="input-fixed w-full h-[2.375rem] flex justify-start items-center font-sans">
                        <input type="text" class="bg-[#FAFAFA] rounded text-[12px] w-64 h-9 outline-none border border-gray-300" style="padding: 9px 0 7px 8px;" placeholder="Phone number, username, or email">
                    </div>
                    <div class="input-fixed w-full h-[2.375rem] flex justify-start items-center mt-1 font-sans">
                        <input type="text" class="bg-[#FAFAFA] rounded text-[12px] w-64 h-9 outline-none border border-gray-300" style="padding: 9px 0 7px 8px;" placeholder="Password">
                    </div>
                    <button class="w-64 h-[1.875rem] rounded text-[14px] font-sans font-medium text-white mt-3 -center" style="background-color: rgba(0, 149, 246, 0.3);"> Log in </button>
                </div>
                <div class="hrs-fixed w-full h-12 flex justify-center items-center">
                    <hr class="w-[6.5625rem] mr-4">
                    or
                    <hr class="w-[6.5625rem] ml-4">
                </div>
                <div class="btm-fixed-pos h-20 flex justify-end items-center flex-col">
                    <div class="fb-login">
                        <button class="h-6 w-full text-lg font-semibold font-sans -center mb-4" style="color: #385185;">
                            <i class="fa fa-brands fa-square-facebook mr-2.5"></i> 
                            <p class="text-sm -center"> Log in with Facebook </p> 
                        </button>
                    </div>
                    <div class="forget-password text-xs font-thin font-sans pb-4">
                        <p> Forget pasword? </p>
                    </div>
                </div>
            </div>
        </div>
        
        <div class="new-account h-16 w-full -center-col border border-gray-300 mt-3 text-sm">
            <p> Don't have an account? <span style="color: #0095f6"> Sign up </span> </p>
        </div>
        
        <div class="get-app h-[6.25rem] w-full flex justify-evenly items-center flex-col">
            <div class="get-app-p -center h-5 w-full">
            <p class="text-sm text-center" style="color: #262626;"> Get the app</p>
            </div>
            <div class="store-btns h-11 w-full flex justify-center items-center">
                <div class="btn-windows h-10 w-[8.5rem]">
                <img src="https://i.ibb.co/6vfywH0/c5-Rp7-Ym-Klz.png" alt="btn-img" class="h-10 w-[8.5rem]">
                </div>
                <div class="btn-mobile h-10 w-[6.875rem] ml-2">
                <img src="https://i.ibb.co/FnXjG4r/EHY6-Qn-ZYd-NX.png" alt="btn-img" class="h-10 w-[6.5rem] ">
                </div>
            </div>
        </div>
    </div>

</template>

<script>
export default {
    data() {
        return {
            img : ""
        }
    },
    mounted() {
        setInterval(function() {
            document.getElementById("im-def").setAttribute("style", "display: none;")
            if (this.img) {
                img.setAttribute("style", "display: none;")
            }
            let randomNum = Math.floor(Math.random() * 4)
            if (randomNum == 0) {
                randomNum = 1
            }
            this.img = document.getElementById("im" + randomNum)
            this.img.setAttribute("style", "display: block;")
        }, 10000)
    },
    updated() {
        console.log("updated")
    },
}
</script>

<style>

</style>