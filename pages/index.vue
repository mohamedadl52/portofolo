<template>
  <div class="bgground">
    <navbar-3></navbar-3>
    <div>
      <h1
        class="absolute xl:top-24 top-48 xl:right-64 right-24 text-2xl md:text-4xl xl:text-5xl underline text-white z-20"
      >
        مرحبا انا
        <span style="font-family: 'Aref Ruqaa', serif">محمد عادل </span>
      </h1>

      <h2
        class="xl:top-56 md:right-24 md:text-4xl top-64 text-2xl xl:right-64 z-20 right-12 xl:text-4xl text-white absolute"
        style="font-famaily: "
      >
        مــــصمم مــواقع الــكترونية
      </h2>
      <p
        style="color: #ffb225"
        class="absolute top-64 w-64 z-20 left-10 xl:left-40 ml-4 md:right-64 md:ml-32 lg:text-center lg:w-1/3 lg:ml-64 shadow-xl font-semibold text-2xl md:text-3xl md:w-8/12 text-center mt-16"
      >
        full stack devolover
      </p>
      <button
        style="font-family: 'Monoton', cursive"
        class="w-48 text-blue-400 z-20  left-1/4 md:left-1/3 md:ml-10 xl:ml-20  text-2xl p-2 bg-white absolute top-64 mt-32   rounded-xl"
      >
        Contact me
      </button>
    </div>
  
    
    <div class="absolute bottom-10 left-20 z-30">
      <typical
        class="vt-title text-blue-400 xl:text-2xl"
        :steps="['Hello', 1000, 'Hello world!', 500]"
        :wrapper="'h2'"
      ></typical>
      <br>
      <typical
        class="vt-subTitle text-white font-bold xl:text-3xl"
        :steps="[' Awesome website!', 500, ' Awesome! Aha :-) 👋', 1000]"
        :loop="545"
        :wrapper="'h1'"
      ></typical>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      
    }
  },
}
</script>

<style lang="scss" scoped>
h2 {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen,
    Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}
.bgground {
  background-color: #797171;
}

</style>
