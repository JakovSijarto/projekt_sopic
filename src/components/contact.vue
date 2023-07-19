<template>
    <div class="flex justify-center flex-col items-center w-full" id="contact">
       <div class="flex justify-between w-[1340px] items-center pt-[100px] max-[1370px]:flex-col max-[1370px]:w-full max-[1370px]:pt-[50px] px-8">
               <div class="w-full mb-[6em]">
                   <form ref="form" @submit="sendEmail">
                   <p class="text-center latofont text-[35px] font-bold mb-[5px]">Drop us message for any query</p>
                   <p class="text-center catamaran mb-[30px] text-[#555]">For more information about our Transport, get in touch with Tranx contacts</p>
                   <div class="flex gap-[2em] w-[full] justify-between mb-[20px] max-[640px]:flex-col">
                       <div class="w-[50%] max-[640px]:w-full">
                           <p class="mb-[5px] text-[#555]">Name</p>
                           <input type="text" required v-model="ime" class="border-0  w-[100%] h-[50px] py-[0.375rem] pl-[20px] pr-[0.75rem] bg-[#f5f5f5] text-[1rem] leading-6">
                       </div>
                       <div class="w-[50%] max-[640px]:w-full">
                           <p class="mb-[5px] text-[#555]">Email</p>
                           <input type="email" required v-model="email" class="border-0  w-[100%] h-[50px] py-[0.375rem] pl-[20px] pr-[0.75rem] bg-[#f5f5f5] text-[1rem] leading-6">
                       </div>
                   </div>
                   <div class="flex gap-[2em] w-[full] justify-between mb-[20px] max-[640px]:flex-col">
                       <div class="w-[50%] max-[640px]:w-full">
                           <p class="mb-[5px] text-[#555]">Telefon</p>
                           <input type="phone" required v-model="telefon" class="border-0  w-[100%] h-[50px] py-[0.375rem] pl-[20px] pr-[0.75rem] bg-[#f5f5f5] text-[1rem] leading-6">
                       </div>
                       <div class="w-[50%] max-[640px]:w-full">
                           <p class="mb-[5px] text-[#555]">Firma</p>
                           <input type="text" v-model="firma" class="border-0  w-[100%] h-[50px] py-[0.375rem] pl-[20px] pr-[0.75rem] bg-[#f5f5f5] text-[1rem] leading-6">
                       </div>
                   </div>
                   <div class="w-full mb-[20px]">
                           <p class="mb-[5px] text-[#555]">Message</p>
                           <textarea v-model="poruka" class="border-0 py-[1.2rem] px-[20px] bg-[#f5f5f5] text-[1rem] leading-6 w-full h-[10em] max-h-[10em]"></textarea>
                   </div>
                   <div class="text-center">
                       <button type="submit" class="py-[12px] px-[35px] bg-[#0D4268] rounded text-white hover_button mt-[30px] max-[640px]:w-[100%]">Send Message</button>
                   </div>
               </form>
               </div>
               <div class="w-[600px] text-center px-[10px] pl-[70px] max-[1370px]:flex max-[1370px]:p-0 max-[1370px]:w-full max-[1370px]:justify-between max-[1370px]:px-8 max-[850px]:flex-col">
                   <div class="">
                       <svg class="m-auto mb-[8px]" width="50px" height="64px" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path d="M16.5562 12.9062L16.1007 13.359C16.1007 13.359 15.0181 14.4355 12.0631 11.4972C9.10812 8.55901 10.1907 7.48257 10.1907 7.48257L10.4775 7.19738C11.1841 6.49484 11.2507 5.36691 10.6342 4.54348L9.37326 2.85908C8.61028 1.83992 7.13596 1.70529 6.26145 2.57483L4.69185 4.13552C4.25823 4.56668 3.96765 5.12559 4.00289 5.74561C4.09304 7.33182 4.81071 10.7447 8.81536 14.7266C13.0621 18.9492 17.0468 19.117 18.6763 18.9651C19.1917 18.9171 19.6399 18.6546 20.0011 18.2954L21.4217 16.883C22.3806 15.9295 22.1102 14.2949 20.8833 13.628L18.9728 12.5894C18.1672 12.1515 17.1858 12.2801 16.5562 12.9062Z" fill="#0D4268"></path> </g></svg>
                       <p class="latofont text-[20px] font-bold mb-[15px]">Call us</p>
                       <p class="mb-[5px] catamaran">Phone:<a href="" class="pl-[5px] text-[#0D4268]">+1 (514) 312-5678</a></p>
                       <p class="mb-[30px] catamaran mb-[30px] pb-[30px] max-[1370px]:!border-b-0 max-[850px]:!border-b-2" style="border-bottom: 1px solid #e5e5e5;">Mobile:<a href="" class="pl-[5px] text-[#0D4268]">+1 (514) 312-5678</a></p>
                   </div>
                   <div class="">
                       <svg class="m-auto mb-[8px]" version="1.0" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="40px" height="40px" viewBox="0 0 64 64" enable-background="new 0 0 64 64" xml:space="preserve" fill="#000000"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path fill="#0D4268" d="M32,0C18.746,0,8,10.746,8,24c0,5.219,1.711,10.008,4.555,13.93c0.051,0.094,0.059,0.199,0.117,0.289l16,24 C29.414,63.332,30.664,64,32,64s2.586-0.668,3.328-1.781l16-24c0.059-0.09,0.066-0.195,0.117-0.289C54.289,34.008,56,29.219,56,24 C56,10.746,45.254,0,32,0z M32,32c-4.418,0-8-3.582-8-8s3.582-8,8-8s8,3.582,8,8S36.418,32,32,32z"></path> </g></svg>
                       <p class="font-bold text-[20px] mb-[15px] latofont text-[#1A1A1A]">Our location</p>
                       <p class="catamaran text-[#555] mb-[30px] pb-[30px] max-[1370px]:!border-b-0 max-[850px]:!border-b-2" style="border-bottom: 1px solid #e5e5e5;">6890 Blvd, The Bronx, NY 1058 New York, USA</p>
                   </div>
                   <div class="max-[850px]:mb-[5rem]">
                       <svg class="m-auto mb-[8px]" width="40px" height="40px" viewBox="0 -3.5 32 32" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:sketch="http://www.bohemiancoding.com/sketch/ns" fill="#000000"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <title>mail</title> <desc>Created with Sketch Beta.</desc> <defs> </defs> <g id="Page-1" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd" sketch:type="MSPage"> <g id="Icon-Set-Filled" sketch:type="MSLayerGroup" transform="translate(-414.000000, -261.000000)" fill="#0D4268"> <path d="M430,275.916 L426.684,273.167 L415.115,285.01 L444.591,285.01 L433.235,273.147 L430,275.916 L430,275.916 Z M434.89,271.89 L445.892,283.329 C445.955,283.107 446,282.877 446,282.634 L446,262.862 L434.89,271.89 L434.89,271.89 Z M414,262.816 L414,282.634 C414,282.877 414.045,283.107 414.108,283.329 L425.147,271.927 L414,262.816 L414,262.816 Z M445,261 L415,261 L430,273.019 L445,261 L445,261 Z" id="mail" sketch:type="MSShapeGroup"> </path> </g> </g> </g></svg>
                       <p class="latofont text-[20px] font-bold mb-[15px]">Email</p>
                       <p class="text-[#555] catamaran">Gmail: <a href="" class="pl-[5px] text-[#0D4268]">tranx@gmail.com</a></p>
                   </div>
               </div>
       </div> 
       <iframe src="https://www.google.com/maps/embed?pb=!1m17!1m12!1m3!1d2781.845880917174!2d15.785049415568533!3d45.79431527910627!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m2!1m1!2zNDXCsDQ3JzM5LjUiTiAxNcKwNDcnMTQuMSJF!5e0!3m2!1shr!2shr!4v1688818911144!5m2!1shr!2shr" class="w-full min-h-[500px]" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>        </div>
</template>

<script>
import emailjs from 'emailjs-com';

export default {
data(){
return{
 ime:"",
 email:"",
 telefon:"",
 firma:"",
 poruka:""
}
},
methods: {
sendEmail() {
 emailjs.sendForm('service_55615g5', 'template_fudpvll', this.$refs.form, 'yEsBpX8Qb6pmeIUeP')
   .then((result) => {
        console.log('SUCCESS!', result.text);
   }, (error) => {
       console.log('FAILED...', error.text);
   });
   
},

},

}
</script>

<style scoped>

</style>