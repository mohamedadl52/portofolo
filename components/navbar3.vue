<template>
  <div class="h-screen overflow-scroll xl:overflow-hidden z-20">
    <nav
      style="direction: rtl"
      class="md:flex xl:flex-col xl:justify-end xl:items-start z-20"
    >
      <div
        style="background-color: #302c2c"
        class="flex z-20 flex-wrap flex-row-reverse lg:flex-col justify-between"
      >
        <div class="xl:w-32 xl:mt-4 z-20">
          <img
            width="70px"
            class="xl:mr-6 md:mr-2 mt-2"
            height="auto"
            src="../assets/images/m.png"
            alt=""
          />
          <p
            style="font-family: 'Aref Ruqaa', serif"
            class="font-bold text-sm text-white xl:text-center ml-3.5 md:mr-2 xl:mr-0 text-xl mt-2"
          >
            محمد عادل
          </p>
        </div>
        <div class="md:hidden z-20">
          <div class="text-white text-4xl mr-6 mt-4 z-20" @click="tooglemenu">
            <font-awesome-icon class="z-20" :icon="['fas', 'bars']" />
          </div>
        </div>
      </div>
      <div
        style="background-color: #302c2c"
        class="flex-grow xl:flex flex-col xl:h-screen justify-between md:pb-6 z-20"
      >
        <transition name="fade" class="z-20">
          <div class="z-20">
            <ul
              :class="{ hidden: fullwidth }"
              class="flex xl:items-center justify-around z-20 md:mt-8 xl:w-32 xl:mt-8 xl:flex flex-grow items-center text-blue-500 transition-all duration-700 delay-75 md:flex ease-linear overflow-hidden xl:flex-col"
            >
              <li class="relative z-20" @mouseenter="noti1">
                <a href="/">
                  <font-awesome-icon
                    class="text-5xl my-4 hover:text-white transition-all duration-700 z-20"
                    :icon="['fas', 'home']"
                /></a>
                <notifications group="foo" position="center top">
                  <template slot="body" slot-scope="props">
                    <div
                      style="font-family: 'Aref Ruqaa', serif"
                      class="text-white z-20"
                      v-text="props.item.text"
                    ></div>
                  </template>
                </notifications>
              </li>
              <li class="z-20" @mouseenter="noti2">
                <a href="/skills">
                  <font-awesome-icon
                    class="text-5xl my-4 hover:text-white transition-all duration-700 z-20"
                    :icon="['fas', 'user-cog']"
                /></a>
              </li>
              <li class="z-20" @mouseenter="noti3">
                <a href="/works">
                  <font-awesome-icon
                    class="text-5xl my-4 hover:text-white transition-all duration-700 z-20"
                    :icon="['fas', 'briefcase']"
                /></a>
              </li>
              <li class="z-20" @mouseenter="noti4">
                <a href="/contact">
                  <font-awesome-icon
                    class="text-5xl my-4 hover:text-white transition-all duration-700 z-20"
                    :icon="['fas', 'envelope']"
                /></a>
              </li>
            </ul>
          </div>
        </transition>
        <ul
          class="text-white hidden xl:flex xl:flex-row xl:items-center justify-around items-center"
        >
          <li>
            <a href="/home">
              <font-awesome-icon
                class="text-2xl hover:text-blue-400"
                :icon="['fab', 'facebook']"
            /></a>
          </li>
          <li>
            <a href="/home">
              <font-awesome-icon
                class="text-2xl hover:text-blue-400"
                :icon="['fab', 'whatsapp']"
            /></a>
          </li>
          <li>
            <a href="/home">
              <font-awesome-icon
                class="text-2xl hover:text-blue-400"
                :icon="['fab', 'telegram']"
            /></a>
          </li>
        </ul>

        <div>
          <ul>
            <li></li>
          </ul>
        </div>
      </div>
    </nav>
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
    tooglemenu() {
      this.fullwidth = !this.fullwidth
    },
    noti1() {
      this.$notify({
        group: 'foo',
        text: 'Home',
      })
    },
    noti2() {
      this.$notify({
        group: 'foo',
        text: 'Skills',
      })
    },
    noti3() {
      this.$notify({
        group: 'foo',
        text: 'Works',
      })
    },
    noti4() {
      this.$notify({
        group: 'foo',
        text: 'Contact me',
      })
    },
  },
}
</script>

<style scoped>
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s;
}
.fade-enter, .fade-leave-to /* .fade-leave-active below version 2.1.8 */ {
  opacity: 0;
}
</style>
