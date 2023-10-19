<template>
    <div class="w-full h-[100vh] bg-black">
        <div class="w-full h-[100vh] bg_image ">
            <img src="../assets/herosectionbackground.png" class="object-fit w-full h-full max-[1370px]:hidden !bg-white" alt="">
        </div>
        <div class="absolute z-[100] absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2">
            <div class="w-[1340px] max-[1370px]:w-full max-[790px]:text-center">
                <p class="mb-[25px] font-black text-[60px] latofont max-[1370px]:text-white max-[490px]:mb-[5rem]">AP Sopic</p>
                <p class="max-w-[645px] leading-7 text-[18px] mb-[35px] max-[1370px]:text-white max-[490px]:hidden">AP Sopic je u mogućnosti organizirati prijevoz pošiljaka svim vrstama kamiona uključujući i prijevoz specijalnih tereta.</p>
                <a href="#contact"><button class="py-[12px] px-[35px] bg-[#0D4268] rounded text-white hover_button">Contact Us</button> </a>
            </div>
        </div>
    </div>
</template>

<script setup>

</script>

<style>
@media only screen and (max-width: 1370px) {
    .bg_image{
    opacity: 0.3;
    }
    .bg-black{
        background-color: black;
    }
}

.hover_button:hover{
        background-color: black;
        transition: all 0.4s ease-in;
    }
.hover_button{
    transition: all 0.4s ease-out;
}
.bg_image{
    background-image: url('../assets/mobile_hero_img.webp');
    background-size: cover;
    background-position: center center;
    background-repeat: no-repeat;
    background-attachment: fixed;
}

</style>

