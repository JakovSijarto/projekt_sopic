<script setup>
    import navbar from "./navbar.vue"
    import herosection from "./herosec.vue"
    import aboutus from "./aboutus.vue"
    import contact_page from "./contact.vue"
    import footer_page from "./footer.vue"
</script>

<template>
    <div class="text-[#1A1A1A] ">
        <div class="fixed bg-white z-[999] flex justify-center w-full border-b-[1px] border-[#f5f5f5]">
            <navbar/>
        </div>
        <herosection/>
        <aboutus/>
        <contact_page/>
        <footer_page/>
    </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Lato:wght@900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Catamaran&display=swap');


*{
    scroll-behavior: smooth;
}
.latofont{
     font-family: 'Lato', sans-serif !important;
}
.catamaran{
    font-family: 'Catamaran', sans-serif;
}
</style>
