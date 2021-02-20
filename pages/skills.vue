<template>
  <div class="bgground">
    <navbar-3></navbar-3>
    <div
      style="direction: rtl"
      class="absolute top-48 right-6 left-0 mx-2 md:left-64 xl:top-20 text-white xl:right-64"
    >
      <h2 class="text-3xl h2">ما استطيع فعله :</h2>

      <img
        class="absolute left-0 -top-10 md:-left-40 xl:-top-20 xl:-left-64 w-16 xl:w-32"
        src="../assets/images/bird.png"
        alt=""
      />
      <img
        class="absolute xl:-top-20 md:top-4 xl:-left-24 w-7/12 z-20 hidden md:block"
        src="../assets/images/folck.png"
        alt=""
      />
      <ul class="list-disc leading-10 z-30">
        <li>تصميم المواقع بواسطه html و css و js</li>
        <li>تصميم المواقع بواسطه vue و taiwindcss</li>
        <li>تصميم المواقع بواسطه nuxt و taiwindcss</li>
      </ul>

      <ul style="direction: ltr" class="leading-10 mt-10 z-30">
        <li>
          <label for="file" class="rounded-full"> tailwind css 70% </label>
        </li>

        <li>
          <label for=""> bootstrap 50% </label>

          <progress id="file" value="32" max="100"></progress>
        </li>
        <li>
          <label for=""> vue 60% </label>

          <progress id="file" value="32" max="100"></progress>
        </li>
        <li>
          <label for=""> nuxt js 55% </label>

          <progress id="file" value="32" max="100"></progress>
        </li>
      </ul>
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
  @apply bg-black;
  .h2 {
    color: red;
  }
}
</style>
