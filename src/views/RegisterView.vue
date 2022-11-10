<template>

    <div class="login-div h-[51.5remrem] w-[21.875rem] -center-col max-md:scale-1.10">

        <div class="login-form h-[42rem] w-full flex-col flex justify-evenly items-center border border-gray-300">

            <div class="logo-fixed-pos h-[6.25rem] flex justify-center items-center">
                <div class="logo-insta-login -center mt-4">
                    <i data-visualcompletion="css-img" aria-label="Instagram" class="" role="img" style="background-image: url(&quot;https://static.cdninstagram.com/rsrc.php/v3/yw/r/kUy2G4UGM26.png&quot;); background-position: 0px -504px; background-size: 348px 612px; width: 174px; height: 50px; background-repeat: no-repeat; display: inline-block;"></i>
                </div>
            </div>

            <div class="register-msg -center h-14 font-sans font-semibold text-[17px] text-[#8e8e8e]">
                <p class="h-10 w-[16.75rem]"> Sign up to see photos and videos from your friends. </p>
            </div>

            <div class="div-fb-btn-fixed w-full h-10 -center mt-2.5">
                <button class="w-64 h-[1.875rem] rounded text-[14px] font-sans font-medium -center" style="background-color: rgb(0, 149, 246);"> 
                    <div class="fb-login -center h-full w-full">
                            <div class="register-fb-fixed mr-2.5 text-lg  text-white">
                                <i class="fa fa-brands fa-square-facebook"></i> 
                            </div>
                            <p class="text-sm -center text-white"> Log in with Facebook </p> 
                    </div>
                </button>
            </div>

            <div class="hrs-fixed w-full h-12 flex justify-center items-center mt-8">
                <hr class="w-[6.5625rem] mr-4">
                <p> or </p>
                <hr class="w-[6.5625rem] ml-4">
            </div>

            <div class="elements-fixed-pos -center-col  w-full h-96">
                <div class="forms-login w-full">

                    <div class="full-inputs-fixed">
                        <div class="input-fixed w-full h-[2.375rem] flex justify-center items-center font-sans">
                            <input type="text" class="bg-[#FAFAFA] rounded text-[12px] w-64 h-9 outline-none border border-gray-300" style="padding: 9px 0 7px 8px;" placeholder="Mobile Number or Email">
                        </div>
                        <div class="input-fixed w-full h-[2.375rem] flex justify-center items-center mt-1 font-sans">
                            <input type="text" class="bg-[#FAFAFA] rounded text-[12px] w-64 h-9 outline-none border border-gray-300" style="padding: 9px 0 7px 8px;" placeholder="Full Name">
                        </div>
                        <div class="input-fixed w-full h-[2.375rem] flex justify-center items-center mt-1 font-sans">
                            <input type="text" class="bg-[#FAFAFA] rounded text-[12px] w-64 h-9 outline-none border border-gray-300" style="padding: 9px 0 7px 8px;" placeholder="Username">
                        </div>
                        <div class="input-fixed w-full h-[2.375rem] flex justify-center items-center mt-1 font-sans">
                            <input type="text" class="bg-[#FAFAFA] rounded text-[12px] w-64 h-9 outline-none border border-gray-300" style="padding: 9px 0 7px 8px;" placeholder="Password">
                        </div>
                    </div>

                    <div class="form-msg-btn-fixed mt-6">
                        <div class="form-msg text-xs text-[#8e8e8e]">
                            People who use our service may have uploaded your contact information to Instagram. <a href="#" class="font-semibold font-sans text-gray-500"> Learn More </a>
                            <br>
                            <br>
                            By signing up, you agree to our <a href="#" class="font-semibold font-sans text-gray-500"> Terms , Privacy Policy and Cookies Policy . </a>
                        </div>

                        <div class="login-fixed-btn w-full -center mt-1">
                            <button class="w-64 h-[1.875rem] rounded text-[14px] font-sans font-medium text-white mt-3 -center" style="background-color: rgba(0, 149, 246, 0.3);"> Sign up </button>
                        </div>                      
                    </div>

                </div>
            </div>
        </div>

        <div class="new-account h-16 w-full -center-col border border-gray-300 mt-3 text-sm">
            <p> Have an account? <span style="color: #0095f6"> Log in </span> </p>
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
        // setInterval(function() {
        //     document.getElementById("im-def").setAttribute("style", "display: none;")
        //     if (this.img) {
        //         img.setAttribute("style", "display: none;")
        //     }
        //     let randomNum = Math.floor(Math.random() * 4)
        //     if (randomNum == 0) {
        //         randomNum = 1
        //     }
        //     this.img = document.getElementById("im" + randomNum)
        //     this.img.setAttribute("style", "display: block;")
        // }, 10000)
    },
    updated() {
        console.log("updated")
    },
}
</script>

<style>

</style>