<template>
  <div>
    <header class="">
        <div class="container mx-auto ">
          <br>
            <div class="flex relative justify-between mx-2 xl:mx-0 flex-col md:flex-row">
                 <div class="flex justify-between">
                    <div>
                       <img class="inline-block " width="auto" height="auto" src="../assets/images/project1/1.png" alt=""><span class="text-white text-2xl  mt-20">MotiveZone</span>
          
                    </div>
                    
                          <div class="md:hidden">
                     <font-awesome-icon class="text-white  text-3xlq" @click="togglemenu" :icon="['fas', 'bars']" />
                  </div>
                 </div>
                  

                 <div class="flex justify-between flex-grow flex-col md:flex-row ">
                                 <transition name="bounce">
                   <div   :class="{'hidden': fullwidth}" class="menu transition-all duration-700 ease-linear md:block text-center flex-grow">


                     
                        <ul class="bg-blue-900 underline md:no-underline md:bg-transparent" >
                          <li><a href="">Home</a></li>
                          <li><a href="">Our Works</a></li>
                          <li><a href="">About Us</a></li>
                          <li><a href="">Contact us</a></li>
                  
                        </ul>

                   </div>
                                 </transition>
                  <div class="flex-grow ">
                           
    
                      <button class="btn ">say hi</button>

                   </div>
                 </div>
                 
                
      </div>

      <div class="flex flex-col md:flex-row mx-4 xl:mx-0 ">
   <div>
     <h1 class="text-3xl text-white mt-10 md:mt-32 "> clwe splite every things </h1>
     <p class="tesx-xl text-white ">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Natus ipsum quisquam quaerat architecto vel at repellat eveniet laboriosam fuga atque quis, possimus minus ea necessitatibus voluptatem incidunt nulla beatae praesentium.</p>
   </div>
   <div>
       <img src="../assets/images/2.png" width="auto" class="z-30 mt-10 md:mt-20 relative" height="auto" alt="">
   </div>

      </div>

      <div class=" absolute bottom-0 w-full  left-0">

        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
  <path fill="#fff" fill-opacity="1" d="M0,290L2040,200L1640,420L0,320Z"></path>
</svg>
      </div>
        </div>
    </header>


    <section>
        <div class="mt-20 text-center">
              <h1 class=" text-maincolor text-4xl text-center">Our Service </h1>
              <h1 class=" text-maincolor text-xl text-center ">Lorem ipsum dolor sit amet consectetur adipisicing elit. Dicta maiores, voluptates </h1>
        </div>

        <div class="flex flex-col mt-20  container mx-auto md:flex-row md:justify-around justify-center items-center ">
           <div class="md:w-1/4 text-center mb-10 mx-4 text-maincolor ">
             <img src="../assets/images/project1/3.png" class="mx-auto" alt=""> <br>
          <h1 class="text-2xl">web design</h1>
          <p class="leading-6">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Rem id eos quidem explicabo unde totam suscipit, re</p> 
          <p class="mt-2">learn more ----></p>
           </div>
           <div class="md:w-1/4 text-center mb-10 mx-4 text-maincolor ">
             <img src="../assets/images/project1/4.png" class="mx-auto" alt=""> <br>
          <h1 class="text-2xl">web design</h1>
          <p class="leading-6">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Rem id eos quidem explicabo unde totam suscipit, re</p> 
          <p class="mt-2" >learn more ----></p>
           </div>
           <div class="md:w-1/4 text-center mb-10 mx-4 text-maincolor ">
             <img src="../assets/images/project1/3.png" class="mx-auto" alt=""> <br>
          <h1 class="text-2xl">web design</h1>
          <p class="leading-6">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Rem id eos quidem explicabo unde totam suscipit, re</p> 
          <p class="mt-2">learn more ----></p>
           </div>
          
        </div>
    </section>

    <section class="container xl:mx-auto mt-20 ">
          <div class="flex flex-col md:flex-row mx-2 leading-5">
               <div>
                <h1 class="text-3xl text-maincolor  md:mt-20 font-bold"> what are we doing ?</h1>
             <p class="text-xl text-maincolor leading-7 my-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste, ipsum quo omnis totam harum autem sed obcaecati laudantium adipisci libero vero similique dicta !</p>
             <button class="bg-btn text-maincolor  p-2">read more</button>
               </div>
               <div>
                   <img src="../assets/images/project1/6.png" alt="">
               </div>
          </div>
          <div class="flex flex-col md:flex-row mx-2 leading-5 mt-10 md:mt-20 ">
               <div>
                <h1 class="text-3xl text-maincolor md:mt-20  font-bold"> what are we doing ?</h1>
             <p class="text-xl text-maincolor leading-7 my-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste, ipsum quo omnis totam harum autem sed obcaecati laudantium adipisci libero vero similique dicta !</p>
             <button class="bg-btn text-maincolor  p-2">read more</button>
               </div>
               <div>
                   <img src="../assets/images/project1/7.png" alt="">
               </div>
          </div>
    </section>
      <section class="w-full h-screen sec2">
       <div  class="w-full XL:h-screen  ">
Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero, blanditiis rerum sequi explicabo eligendi itaque in? Placeat optio sunt itaque repellendus, libero, harum dolorem alias iusto deserunt hic eveniet exercitationem!
       </div>
      </section>
  </div>
</template>
<script>
export default {
  data() {
    return {
      fullwidth: true,
    }
  },
  methods: {
    togglemenu() {
      this.fullwidth = !this.fullwidth
    },
  },
}
</script>

<style lang="scss" scoped>
header {
  background: linear-gradient(to left bottom, white 0%, #1b498a 0%);
  @apply relative w-full h-screen;
  .menu ul li {
    @apply text-white md:inline-block ml-5 leading-10 transition-all duration-700  hover:text-gray-900;
  }
  .btn {
    background: #ff9c00;
    @apply text-white  leading-10 w-32 hidden md:block mx-auto;
  }
}

.bounce-enter-active {
  animation: bounce-in 0.5s;
}
.bounce-leave-active {
  animation: bounce-in 0.5s reverse;
}
@keyframes bounce-in {
  0% {
    transform: scale(0);
  }
  50% {
    transform: scale(1.5);
  }
  100% {
    transform: scale(1);
  }
}

.sec2 {
  background: url("../assets/images/project1/8.png") no-repeat;
  background-size: cover;
  div{
    background:#1a4789b8;
  }
}
</style>
