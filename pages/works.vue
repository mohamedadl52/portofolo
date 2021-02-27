<template>
  <div class="bgground">
    <navbar-3></navbar-3>
    <div
      class="absolute w-64 hidden md:mt-24 xl:mt-0 md:block md:w-10/12 md:left-12 lg:left-32 xl:left-2 top-16 xl:top-0"
    >
      <img
        class="absolute top-2 left-64 w-16"
        src="../assets/images/animal.png"
        alt=""
      />
      <img
        class="absolute top-2 left-32 w-16"
        src="../assets/images/animal.png"
        alt=""
      />
      <img
        class="absolute top-2 left-16 w-16"
        src="../assets/images/animal.png"
        alt=""
      />
      <img
        class="absolute top-2 right-16 w-16"
        src="../assets/images/animal.png"
        alt=""
      />
      <img
        class="absolute top-2 right-32 w-16"
        src="../assets/images/animal.png"
        alt=""
      />
      <img
        class="absolute top-2 right-64 w-16"
        src="../assets/images/animal.png"
        alt=""
      />
      <img
        class="absolute top-2 left-64 w-16"
        src="../assets/images/animal.png"
        alt=""
      />
      <splide
        ref="primary"
        :options="primaryOptions"
        @splide:click="onMounted"
        @splide:arrows:updated="onArrowsMounted"
      >
        <splide-slide>
          <img src="../assets/images/imgprojects/sushii.JPG"/>
        </splide-slide>
        <splide-slide>
            <img src="../assets/images/imgprojects/yogaa.JPG"/>
        </splide-slide>
        <splide-slide>
        <img src="../assets/images/imgprojects/clanasowa.JPG"/>
        </splide-slide>
        <splide-slide>
   <img src="../assets/images/imgprojects/tanatos.jpg"/>
        </splide-slide>
        <splide-slide>
   <img src="../assets/images/imgprojects/timer.JPG"/>
        </splide-slide>
        <splide-slide>
   <img src="../assets/images/imgprojects/flipauth.JPG"/>
        </splide-slide>
        <splide-slide>
   <img src="../assets/images/imgprojects/learnenglish.jpg"/>
        </splide-slide>
        <splide-slide>
   <img src="../assets/images/imgprojects/animations.JPG"/>
        </splide-slide>
      </splide>
      <splide ref="primary2" :options="primaryOptions2">
        <splide-slide>
          <div class="flex justify-between">
            <p class="text-xl p-2 w-10/12 bg-blue-400">
              sushi template
            </p>
            <span
              class="text-blue-400 flex-grow text-center hover:text-gray-500 transition-all duration-700 bg-white font-bold text-xl"
            >
              <a href="https://mohhaammeedd.000webhostapp.com/sushi/">visit project</a></span
            >
          </div>
        </splide-slide>
        <splide-slide>
          <div class="flex justify-between">
            <p class="text-xl p-2 w-10/12 bg-blue-400">
               yoga template 
            </p>
            <span
              class="text-blue-400 flex-grow text-center hover:text-gray-500 transition-all duration-700 bg-white font-bold text-xl"
            >
              <a href="/yoga">visit project</a></span
            >
          </div>
        </splide-slide>
        <splide-slide>
          <div class="flex justify-between">
            <p class="text-xl p-2 w-10/12 bg-blue-400">
               blog kalna sowa 
            </p>
            <span
              class="text-blue-400 flex-grow text-center hover:text-gray-500 transition-all duration-700 bg-white font-bold text-xl"
            >
              <a href="/https://blognewrepo.herokuapp.com/">visit project</a></span
            >
          </div>
        </splide-slide>
        <splide-slide>
          <div class="flex justify-between">
            <p class="text-xl p-2 w-10/12 bg-blue-400">
               tanatos template  (just for pc)
            </p>
            <span
              class="text-blue-400 flex-grow text-center hover:text-gray-500 transition-all duration-700 bg-white font-bold text-xl"
            >
              <a href="http://mohhaammeedd.000webhostapp.com/tanatos">visit project</a></span
            >
          </div>
        </splide-slide>
        <splide-slide>
          <div class="flex justify-between">
            <p class="text-xl p-2 w-10/12 bg-blue-400">
               timer with animation
            </p>
            <span
              class="text-blue-400 flex-grow text-center hover:text-gray-500 transition-all duration-700 bg-white font-bold text-xl"
            >
              <a href="https://mohhaammeedd.000webhostapp.com/test1/">visit project</a></span
            >
          </div>
        </splide-slide>
        
        <splide-slide>
          <div class="flex justify-between">
            <p class="text-xl p-2 w-10/12 bg-blue-400">
              style flip login 
            </p>
            <span
              class="text-blue-400 flex-grow text-center hover:text-gray-500 transition-all duration-700 bg-white font-bold text-xl"
            >
              <a href="https://mohhaammeedd.000webhostapp.com/flipauth/">visit project</a></span
            >
          </div>
        </splide-slide>
        
        <splide-slide>
          <div class="flex justify-between">
            <p class="text-xl p-2 w-10/12 bg-blue-400">
              style lading page 
            </p>
            <span
              class="text-blue-400 flex-grow text-center hover:text-gray-500 transition-all duration-700 bg-white font-bold text-xl"
            >
              <a href="https://mohhaammeedd.000webhostapp.com/learnEngilsh/">visit project</a></span
            >
          </div>
        </splide-slide>
        <splide-slide>
          <div class="flex justify-between">
            <p class="text-xl p-2 w-10/12 bg-blue-400">
              some animations in one page 
            </p>
            <span
              class="text-blue-400 flex-grow text-center hover:text-gray-500 transition-all duration-700 bg-white font-bold text-xl"
            >
              <a href="/animations">visit project</a></span
            >
          </div>
        </splide-slide>
        
      </splide>

      <!-- <splide ref="secondary" :options="secondaryOptions">
       <splide-slide>
          <img src="..\assets\images\imgprojects\sushii.JPG"/>
        </splide-slide>
        <splide-slide>
            <img src="..\assets\images\imgprojects\yogaa.JPG"/>
        </splide-slide>
        <splide-slide>
        <img src="..\assets\images\imgprojects\clanasowa.JPG"/>
        </splide-slide>
        <splide-slide>
   <img src="..\assets\images\imgprojects\tanatos.JPG"/>
        </splide-slide>
        <splide-slide>
   <img src="..\assets\images\imgprojects\timer.JPG"/>
        </splide-slide>
        <splide-slide>
   <img src="..\assets\images\imgprojects\flipauth.JPG"/>
        </splide-slide>
        <splide-slide>
   <img src="..\assets\images\imgprojects\learnenglish.JPG"/>
        </splide-slide>
      </splide> -->
    </div>

    <div
      style="background-color: #797171"
      class="flex flex-col justify-center items-center absolute top-56 md:hidden"
    >
      <img
        class="absolute top-4 left-64 w-16"
        src="../assets/images/animal.png"
        alt=""
      />

      <img
        style="transform: rotateY(180deg)"
        class="absolute top-4 left-4 w-16"
        src="../assets/images/animal.png"
        alt=""
      />

      <p
        style="
          font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto,
            Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        "
        class="text-white text-2xl underline uppercase"
      >
        my works
      </p>
      <div class="my-6 mx-4">
        <img
       src="../assets/images/imgprojects/sushii.JPG"
          class=""
          style="max-width: 100%"
          alt=""
        />
        <p class="text-center">sushi template</p>
        <p class="text-center text-blue-400 text-xl font-bold">
          <a href="https://mohhaammeedd.000webhostapp.com/sushi/">visit project </a>
        </p>
      </div>
      <div class="my-6 mx-4">
        <img
           src="../assets/images/imgprojects/yogaa.JPG"
          class=""
          style="max-width: 100%"
          alt=""
        />
        <p class="text-center">yoga template</p>
        <p class="text-center text-blue-400 text-xl font-bold">
          <a href="/yoga">visit project </a>
        </p>
      </div>
      <div class="my-6 mx-4">
        <img
          src="../assets/images/imgprojects/clanasowa.JPG"
          class=""
          style="max-width: 100%"
          alt=""
        />
        <p class="text-center"> blog kalna sowa</p>
        <p class="text-center text-blue-400 text-xl font-bold">
          <a href="https://blognewrepo.herokuapp.com/"> visit project  </a>
        </p>
      </div>
      <div class="my-6 mx-4">
        <img
         src="../assets/images/imgprojects/tanatos.jpg"
          class=""
          style="max-width: 100%"
          alt=""
        />
        <p class="text-center">tanatos template (only for pc)</p>
        <p class="text-center text-blue-400 text-xl font-bold">
          <a href="http://mohhaammeedd.000webhostapp.com/tanatos">  visit project  </a>
        </p>
      </div>
      <div class="my-6 mx-4">
        <img
        src="../assets/images/imgprojects/timer.JPG"
          class=""
          style="max-width: 100%"
          alt=""
        />
        <p class="text-center">timer with animation </p>
        <p class="text-center text-blue-400 text-xl font-bold">
          <a href="https://mohhaammeedd.000webhostapp.com/test1/"> visit project </a>
        </p>
      </div>
      <div class="my-6 mx-4">
        <img
         src="../assets/images/imgprojects/flipauth.JPG"
          class=""
          style="max-width: 100%"
          alt=""
        />
        <p class="text-center">style flip login</p>
        <p class="text-center text-blue-400 text-xl font-bold">
          <a href="https://mohhaammeedd.000webhostapp.com/flipauth/"> visit project  </a>
        </p>
      </div>
      <div class="my-6 mx-4">
        <img
         src="../assets/images/imgprojects/learnenglish.jpg"
          class=""
          style="max-width: 100%"
          alt=""
        />
        <p class="text-center">lading page learnenglish</p>
        <p class="text-center text-blue-400 text-xl font-bold">
          <a href="https://mohhaammeedd.000webhostapp.com/learnEngilsh/">  visit project  </a>
        </p>
      </div>
      <div class="my-6 mx-4">
        <img
         src="../assets/images/imgprojects/animations.JPG"
          class=""
          style="max-width: 100%"
          alt=""
        />
        <p class="text-center">some animations in one page</p>
        <p class="text-center text-blue-400 text-xl font-bold">
          <a href="https://mohhaammeedd.000webhostapp.com/learnEngilsh/">  visit project  </a>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
import '@splidejs/splide/dist/css/themes/splide-default.min.css'
// or
import '@splidejs/splide/dist/css/themes/splide-sea-green.min.css'
// or
// import '@splidejs/splide/dist/css/themes/splide-skyblue.min.css';

export default {
  data() {
    return {
      primaryOptions: {
        type: 'loop',
        perPage: 1,
        width: 1200,
        height: 425,
        perMove: 1,
        focus: true,
        // autoplay: true,
        speed: 1000,
        gap: '1rem',
        pagination: true,
      },
      primaryOptions2: {
        type: 'loop',
        perPage: 1,
        width: 1200,
        height: 40,
        perMove: 1,
        focus: true,
        // autoplay: true,
        arrows: false,
        speed: 1000,
        gap: '1rem',
        pagination: false,
      },
      secondaryOptions: {
        type: 'slide',
        rewind: true,
        height: 40,
        gap: '1rem',
        pagination: false,
        fixedWidth: 110,
        arrows: false,
        fixedHeight: 70,
        cover: true,
        focus: 'center',
        isNavigation: true,
        updateOnMove: true,
      },
      tages: ['hello1', 'hello2', 'hello3'],
      count: 0,
    }
  },

  mounted() {
    // Set the sync target.
    // this.$refs.primary.sync(this.$refs.secondary.splide)
    // this.$refs.primary2.sync( this.$refs.secondary.splide );
    this.$refs.primary.sync(this.$refs.primary2.splide)
    // this.$refs.secondary.sync(this.$refs.primary2.splide)
    // this.$refs.secondary.sync(this.$refs.primary.splide)
    // this.$refs.primary2.sync( this.$refs.primary.splide );
  },
  methods: {
    onMounted(splide) {},

    onArrowsMounted(splide, prev, next) {},
  },
}
</script>

<style lang="scss" scoped>
.bgground {
  background-color: #797171;
}
</style>
