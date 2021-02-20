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
          <img src="../assets/images/5.jpg" />
        </splide-slide>
        <splide-slide>
          <img src="../assets/images/2.jpg" />
        </splide-slide>
        <splide-slide>
          <img src="../assets/images/3.jpg" />
        </splide-slide>
        <splide-slide>
          <img src="../assets/images/4.jpg" />
        </splide-slide>
      </splide>
      <splide ref="primary2" :options="primaryOptions2">
        <splide-slide>
          <div class="flex justify-between">
            <p class="text-xl">this project talk about medicen in 2021</p>
            <span class="text-blue-500 font-bold text-xl">
              <a href="/">visit project</a></span
            >
          </div>
        </splide-slide>
        <splide-slide>
          <div class="flex justify-between">
            <p class="text-xl">this project talk about medicen in 2021</p>
            <span class="text-blue-500 font-bold text-xl">
              <a href="/">visit project</a></span
            >
          </div>
        </splide-slide>
        <splide-slide>
          <div class="flex justify-between">
            <p class="text-xl">this project talk about medicen in 2021</p>
            <span class="text-blue-500 font-bold text-xl">
              <a href="/">visit project</a></span
            >
          </div>
        </splide-slide>
        <splide-slide>
          <div class="flex justify-between">
            <p class="text-xl">this project talk about medicen in 2021</p>
            <span class="text-blue-500 font-bold text-xl">
              <a href="/">visit project</a></span
            >
          </div>
        </splide-slide>
      </splide>

      <splide ref="secondary" :options="secondaryOptions">
        <splide-slide>
          <img src="../assets/images/5.jpg" />
        </splide-slide>
        <splide-slide>
          <img src="../assets/images/2.jpg" />
        </splide-slide>
        <splide-slide>
          <img src="../assets/images/3.jpg" />
        </splide-slide>
        <splide-slide>
          <img src="../assets/images/4.jpg" />
        </splide-slide>
      </splide>
    </div>

    <div
      style="background-color: #5a4b4b"
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
          src="../assets/images/1.jpg"
          class=""
          style="max-width: 100%"
          alt=""
        />
        <p class="text-center">this project for med</p>
        <p class="text-center text-blue-400 text-xl font-bold">
          <a href="#">visit project </a>
        </p>
      </div>
      <div class="my-6 mx-4">
        <img
          src="../assets/images/1.jpg"
          class=""
          style="max-width: 100%"
          alt=""
        />
        <p class="text-center">this project for med</p>
        <p class="text-center text-blue-400 text-xl font-bold">
          <a href="#">visit project </a>
        </p>
      </div>
      <div class="my-6 mx-4">
        <img
          src="../assets/images/1.jpg"
          class=""
          style="max-width: 100%"
          alt=""
        />
        <p class="text-center">this project for med</p>
        <p class="text-center text-blue-400 text-xl font-bold">
          <a href="#">visit project </a>
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
        height: 299,
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
        height: 30,
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
    this.$refs.primary.sync(this.$refs.secondary.splide)
    // this.$refs.primary2.sync( this.$refs.secondary.splide );
    this.$refs.primary.sync(this.$refs.primary2.splide)
    this.$refs.secondary.sync(this.$refs.primary2.splide)
    this.$refs.secondary.sync(this.$refs.primary.splide)
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
  background-color: #000;
}
</style>
