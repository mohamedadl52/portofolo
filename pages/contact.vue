<template>
  <div class="bgground">
      <div class="z-50"><navbar-3></navbar-3></div>

      <div class="absolute w-full  mx-auto top-48 z-50">
        <ul
          class="text-white flex w-56 mx-auto xl:hidden  justify-around items-center"
        >
          <li>
            <a href="https://www.facebook.com/profile.php?id=100011322487924">
              <font-awesome-icon
                class="text-4xl hover:text-blue-400"
                :icon="['fab', 'facebook']"
            /></a>
          </li>
          <li>
            <a href="00249907452551">
              <font-awesome-icon
                class="text-4xl hover:text-blue-400"
                :icon="['fab', 'whatsapp']"
            /></a>
          </li>
          <li>
            <a href="http://t.me/mhmdadl">
              <font-awesome-icon
                class="text-4xl hover:text-blue-400"
                :icon="['fab', 'telegram']"
            /></a>
          </li>
        </ul>

      </div>
      <div class="z-20 bgground">
        <div class="flex absolute w-full xl:w-10/12 xl:ml-20 bgground top-48 md:top-40 xl:top-0 justify-center items-center">
          <div class="con w-11/12 mx-auto -ml-1">
             <h1> contact us </h1>
        <div class="row100">
          <div class="col">
            <div class="inputbox">
               <input type="text" name="" required id="">
               <span class="text">first name </span>
               <span class="line"> </span>
            </div>
          </div>
          <div class="col">
            <div class="inputbox">
               <input type="text" name="" required id="">
               <span class="text">last name </span>
               <span class="line"> </span>
            </div>
          </div>
        </div>
        <div class="row100">
          <div class="col">
            <div class="inputbox">
               <input type="text" name="" required id="">
               <span class="text">Email </span>
               <span class="line"> </span>
            </div>
          </div>
          <div class="col">
            <div class="inputbox">
               <input type="text" name="" required id="">
               <span class="text">Moblie </span>
               <span class="line"> </span>
            </div>
          </div>
        </div>
        <div class="row100">
          <div class="col">
            <div class="inputbox textarea">
               <textarea type="text" placeholder="type your supject here" name="" > </textarea>
               <span class="linee"> </span>
            </div>
          </div>
        
        </div>
        <div class="row100">
          <div class="col w-full text-center ">
             <input style="background-color; :#3b82f6" class="mt-16 w-24 mx-auto font-bold cursor-pointer text-white bg-blue-500 p-2"  type="submit" value="Send">
          </div>
        
        </div>
          </div>
    </div>

      </div>
  </div>
</template>

<script>
import navbar3 from '../components/navbar3.vue'
export default {
  components: { navbar3 },
}
</script>
<style lang="scss" scoped>
.bgground {
  background-color: #797171;
}
.con {
  h1 {
    @apply text-2xl ml-1 mt-20 md:ml-0 mb-5 text-white uppercase font-bold  w-full text-center
  }
  .row100 {
    @apply relative w-full  flex-col md:flex-row  flex ;
        grid-template-columns: repeat(autofit, minmax(300px, 1fr));
   .col {
     @apply relative px-3 transition-all  m-3 w-full duration-500  ;
     transition: all .5s
   } 
   .inputbox {
     @apply relative w-full h-10 text-gray-800 ;
       input , .textarea textarea {
         @apply w-full absolute h-full bg-transparent border-0   border-b-2 border-black outline-none text-xl px-4 z-10 text-white ;
           &:focus ~ .line ,  &:valid ~ .line {
              height: 100%;
           }
         &:focus + .text ,  &:valid + .text   {
           @apply -left-3 -top-8
         }
       }
       .text {
         @apply absolute left-0 top-0 leading-10 text-lg block px-5 transition-all duration-500 pointer-events-none  
       }
     .line {
       @apply absolute bottom-0 transition-all duration-500 pointer-events-none rounded-md bg-gray-500 block h-1 w-full
     }


   }
  }

}

     .textarea {
   @apply relative w-full h-64 py-3 ;
   textarea {
     @apply bg-transparent text-white border-0 border-black border-b-2;
     width: 100%;
      height: 100px;
      resize: none;
      &::placeholder{
        color: black;
      }
   }
     }
</style>
