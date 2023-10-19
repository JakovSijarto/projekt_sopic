<template>
    <div class="h-[100px] w-[1340px] flex justify-between items-center max-[1370px]:w-full max-[1370px]:mx-8">

        <img src="../assets/logo_navbar.webp" alt="" class="h-[70%] max-[490px]:h-[50%]">
        <div class="font-medium max-[790px]:hidden">
            <a href="#about_us" class="mr-[15px] hover_effect" >O nama</a>
            <a href="#contact" class="ml-[15px] hover_effect">Kontakt</a>
        </div>
        <div class="flex items-center max-[790px]:hidden">
            <div class="mr-4">
                <svg width="40px" height="40px" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path d="M3 6.5C3 14.5081 9.49187 21 17.5 21C18.166 21 18.8216 20.9551 19.4637 20.8682C20.3747 20.7448 21 19.9292 21 19.01V16.4415C21 15.5807 20.4491 14.8164 19.6325 14.5442L16.4841 13.4947C15.6836 13.2279 14.8252 13.699 14.6206 14.5177C14.3475 15.6102 12.987 15.987 12.1907 15.1907L8.80926 11.8093C8.01301 11.013 8.38984 9.65254 9.48229 9.37943C10.301 9.17476 10.7721 8.31644 10.5053 7.51586L9.45585 4.36754C9.18362 3.55086 8.41934 3 7.55848 3H4.99004C4.0708 3 3.25518 3.62533 3.13185 4.53627C3.0449 5.17845 3 5.83398 3 6.5Z" stroke="#0D4268" stroke-width="2" stroke-linejoin="round"></path> <path d="M21 3L15.5 8.5" stroke="#0D4268" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path> <path d="M15 5V8.5V8.5C15 8.77614 15.2239 9 15.5 9V9H19" stroke="#0D4268" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path> </g></svg>            </div>
            <a href="tel:989552092">
                <p class="text-[#0D4268] font-semibold">Nazovi Nas</p>
                <p>(+385) 98 9552092</p>
            </a>
        </div>
        
        <div class="hamb_menu min-[790px]:hidden">
            <input id="checkbox" type="checkbox" @click="showMobile()">
            <label class="toggle" for="checkbox" >
            <div id="bar1" class="bars"></div>
            <div id="bar2" class="bars"></div>
            <div id="bar3" class="bars"></div>
        </label>
        </div>
        <div class="hamb_menu min-[790px]:hidden  absolute top-[-20rem] left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-white w-full h-[50vh] z-[-1] max-[490px]:w-full" :class="{ active: isActive }" style="transition: all 0.4s ease-in-out;">
            <div class="absolute top-[40%] left-1/2 transform -translate-x-1/2 -translate-y-1/2"><a href="#about_us">O nama</a></div>
            <div class="absolute top-[55%] left-1/2 transform -translate-x-1/2 -translate-y-1/2"><a href="#contact">Kontakt</a></div>
            <div class="absolute top-[75%] left-1/2 transform -translate-x-1/2 -translate-y-1/2">
              <a href="#contact"><button class="py-[12px] px-[35px] bg-[#0D4268] rounded text-white hover_button ">Contact Us</button> </a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  data() {
    return {
      isActive: false,
    };
  },
  methods: {
    showMobile() {
      this.isActive = !this.isActive;
    },
  },
};
</script>

<style scoped>
.active{
  top:10rem;
  transition: all 0.4s ease-in-out;
}
@media only screen and (max-width: 790px) {
  .hamb_menu{
    display:block;
  }
}
    .hover_effect:hover{
        color:#0D4268;
    }
    #checkbox {
  display: none;
}

.toggle {
  position: relative;
  width: 40px;
  height: 40px;
  cursor: pointer;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: center;
  gap: 10px;
  transition-duration: .5s;
}

.bars {
  width: 100%;
  height: 4px;
  background-color: #0D4268;
  border-radius: 4px;
}

#bar2 {
  transition-duration: .8s;
}

#bar1 {
  width: 50%;
}

#bar2 {
  width: 75%;
}

#checkbox:checked + .toggle .bars {
  position: absolute;
  transition-duration: .5s;
}

#checkbox:checked + .toggle #bar2 {
  transform: scaleX(0);
  transition-duration: .1s;
}

#checkbox:checked + .toggle #bar1 {
  width: 100%;
  transform: rotate(45deg);
  transition-duration: .5s;
}

#checkbox:checked + .toggle #bar3 {
  width: 100%;
  transform: rotate(-45deg);
  transition-duration: .5s;
}

#checkbox:checked + .toggle {
  transition-duration: .5s;
  transform: rotate(180deg);
}
</style>