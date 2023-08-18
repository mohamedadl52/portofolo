<template>
  <div class="bgground">
    <navbar-3></navbar-3>

      <div style="background-color :#797171" class="flex bgground absolute w-full mb-20 top-48 xl:top-10 left-0 justify-center items-center ">

        <div class="flex bgground flex-wrap xl:mx-32 flex-col mb-20 md:flex-row justify-around">
          <div class="card">
             <div class="box">
               <div>
                 <div class="percent">
                    <svg>
                       <circle cx="70" cy="70" r="70" ></circle>
                       <circle cx="70" cy="70" r="70" ></circle>
                    </svg>
                    <div class="number">
                       <h2><span>90</span> <span  class="ppr">%</span></h2>
                    </div>
                 </div>
               </div>
             </div>
             <div class="text">
                 html
             </div>

          </div>
          <div class="card">
             <div class="box">
               <div>
                 <div class="percent">
                    <svg>
                       <circle cx="70" cy="70" r="70" ></circle>
                       <circle cx="70" cy="70" r="70" ></circle>
                    </svg>
                    <div class="number">
                       <h2><span>70</span> <span  class="ppr">%</span></h2>
                    </div>
                 </div>
               </div>
             </div>
             <div class="text">
                 css
             </div>

          </div>
          <div class="card">
             <div class="box">
               <div>
                 <div class="percent">
                    <svg>
                       <circle cx="70" cy="70" r="70" ></circle>
                       <circle cx="70" cy="70" r="70" ></circle>
                    </svg>
                    <div class="number">
                       <h2><span>60</span> <span  class="ppr">%</span></h2>
                    </div>
                 </div>
               </div>
             </div>
             <div class="text">
                 js
             </div>

          </div> 
          <div class="card">
             <div class="box">
               <div>
                 <div class="percent">
                    <svg>
                       <circle cx="70" cy="70" r="70" ></circle>
                       <circle cx="70" cy="70" r="70" ></circle>
                    </svg>
                    <div class="number">
                       <h2><span>80</span> <span  class="ppr">%</span></h2>
                    </div>
                 </div>
               </div>
             </div>
             <div class="text">
                 tailwindcss
             </div>

          </div>
          <div class="card">
             <div class="box">
               <div>
                 <div class="percent">
                    <svg>
                       <circle cx="70" cy="70" r="70" ></circle>
                       <circle cx="70" cy="70" r="70" ></circle>
                    </svg>
                    <div class="number">
                       <h2><span>66</span> <span class="ppr">%</span></h2>
                    </div>
                 </div>
               </div>
             </div>
             <div class="text">
                 vuejs
             </div>

          </div>
          <div class="card">
             <div class="box">
               <div>
                 <div class="percent">
                    <svg>
                       <circle cx="70" cy="70" r="70" ></circle>
                       <circle cx="70" cy="70" r="70" ></circle>
                    </svg>
                    <div class="number">
                       <h2><span>50</span> <span class="ppr">%</span></h2>
                    </div>
                 </div>
               </div>
             </div>
             <div class="text">
                 nuxtjs
             </div>

          </div>
        </div>

      </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      colors: [
        'gray',
        'yellow',
        'orange',
        'red',
        'green',
        'teal',
        'blue',
        'indigo',
        'purple',
        'pink',
      ],
    }
  },
}
</script>

<style lang="scss" scoped>
.bgground {
  background: #797171;
}
.card{
  @apply text-center relative my-5  w-64 h-56 mx-6  ;
  .box {
    @apply absolute w-full z-20 rounded-xl  h-full flex justify-center items-center left-0 top-0 text-center ;
    background-color : rgba(25,25,54,.5)
 
 }
  .percent {
    @apply absolute w-56 left-20 h-36 rounded-full flex justify-center items-center ;
    .number {
      @apply absolute -top-5 text-3xl text-white left-7 flex justify-center items-center ;
   .ppr {
     @apply text-xl
   }
   }
svg {
  @apply relative  bottom-1/2 right-16 ;
  width :150px;
  height : 150px ;
  circle {
    height: 100%;
    width:100% ;
    fill : none ;
    stroke-linecap: round; 
    padding: 20px;
    stroke:  rgba(25,25,54,.5) ;
    stroke-width: 10 ;
    transform: translateX(3%) translateY(3%);
&:nth-child(2){
  stroke: white ;
  stroke-dasharray: 440px ;
  stroke-dashoffset: 40px
}
  }
}
  }
.text {
  @apply absolute   text-center z-10 uppercase rounded-md shadow-xl bg-blue-500 text-white font-bold text-xl p-2 ;
  transition :bottom .5s , z-index 0s , transform .5s , padding .5s ;
    transition-delay: 0.5s , .5s , 0s ,0s;
  transform : translateX(-50%) ;
  left: 50%;
  z-index: 999;
 padding: 5px 10px 10px;
bottom: -40px;
transform: translateX(-50%) translateY(-50%);
}
&:hover .text {
  transition-delay: 0s , .5s , .5s ,0s;
z-index: 999;
 padding: 10px 20px 10px;
bottom: -50px;
transform: translateX(-50%) translateY(-50%);
}
}

.card:nth-child(1) svg circle:nth-child(2){
  stroke-dashoffset: calc(440 - (440 *90)/100)
} 
.card:nth-child(2) svg circle:nth-child(2){
  stroke-dashoffset: calc(440 - (440 *70)/100)
} 
.card:nth-child(3) svg circle:nth-child(2){
   stroke-dashoffset: calc(440 - (440 *60)/100)
} 
.card:nth-child(4) svg circle:nth-child(2){
   stroke-dashoffset: calc(440 - (440 *80)/100)
} 
.card:nth-child(5) svg circle:nth-child(2){
   stroke-dashoffset: calc(440 - (440 *66)/100)
} 
.card:nth-child(6) svg circle:nth-child(2){
   stroke-dashoffset: calc(440 - (440 *50)/100)
} 
</style>
