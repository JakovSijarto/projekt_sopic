<template>
    <div class="w-full h-[100vh]">
        <div class="bg-black w-full h-[100vh]">
            <img src="../assets/herosectionbackground.png" class="object-fit w-full h-full max-[1370px]:hidden !bg-white" alt="">
            <img src="../assets/herosectionbackground.jpg" alt="" class="object-fit w-full h-[100vh] min-[1371px]:hidden opacity-[0.5] !bg-white">
        </div>
        <div class="absolute z-[100] absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2">
            <div class="w-[1340px] max-[1370px]:w-full max-[790px]:text-center">
                <p class="mb-[25px] font-black text-[60px] latofont max-[1370px]:text-white">AP Sopic</p>
                <p class="max-w-[645px] leading-7 text-[18px] mb-[35px] max-[1370px]:text-white max-[490px]:hidden">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua quis ipsum suspendisse.</p>
                <a href="#contact"><button class="py-[12px] px-[35px] bg-[#0D4268] rounded text-white hover_button ">Contact Us</button> </a>
            </div>
        </div>
    </div>
</template>

<script setup>

</script>

<style>
.hover_button:hover{
        background-color: black;
        transition: all 0.4s ease-in;
    }
.hover_button{
    transition: all 0.4s ease-out;
}

</style>

