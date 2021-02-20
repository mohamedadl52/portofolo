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
        Front end devolover
      </p>
      <button
        style="font-family: 'Monoton', cursive"
        class="w-48 text-blue-400 z-20 md:left-64 lg:ml-32 xl:ml-64 text-2xl p-2 bg-white absolute top-64 mt-32 left-20 rounded-xl"
      >
        Contact me
      </button>
    </div>
    <div class="absolute top-0 left-0">
      <neon-effect
        class="overflow-hidden w-screen"
        :options="options"
      ></neon-effect>
    </div>
    <div class="absolute top-0 hidden lg:block -left-10 z-30">
      <fabric-canvas
        class="z-30 absolute left-20 top-0.5"
        :height="400"
        :width="400"
      >
        <fabric-line
          :id="'headToBody'"
          :x1="headPosLeft"
          :y1="headPosTop"
          :x2="bodyPosLeft"
          :y2="bodyPosTop"
          :fill="'#302c2c'"
          :stroke="'#302c2c'"
          :stroke-width="5"
          :selectable="false"
          :evented="false"
          :origin-x="'center'"
          :origin-y="'center'"
        ></fabric-line>
        <fabric-line
          :id="'bodyToWaist'"
          :x1="bodyPosLeft"
          :y1="bodyPosTop"
          :x2="waistPosLeft"
          :y2="waistPosTop"
          :fill="'#302c2c'"
          :stroke="'#302c2c'"
          :stroke-width="5"
          :selectable="false"
          :evented="false"
          :origin-x="'center'"
          :origin-y="'center'"
        ></fabric-line>
        <fabric-line
          :id="'bodyToLeftArm'"
          :x1="bodyPosLeft"
          :y1="bodyPosTop"
          :x2="leftHandPosLeft"
          :y2="leftHandPosTop"
          :fill="'#302c2c'"
          :stroke="'#302c2c'"
          :stroke-width="5"
          :selectable="false"
          :evented="false"
          :origin-x="'center'"
          :origin-y="'center'"
        ></fabric-line>
        <fabric-line
          :id="'bodyToRightArm'"
          :x1="bodyPosLeft"
          :y1="bodyPosTop"
          :x2="rightHandPosLeft"
          :y2="rightHandPosTop"
          :fill="'#302c2c'"
          :stroke="'#302c2c'"
          :stroke-width="5"
          :selectable="false"
          :evented="false"
          :origin-x="'center'"
          :origin-y="'center'"
        ></fabric-line>
        <fabric-line
          :id="'waistToLeftFoot'"
          :x1="leftFootPosLeft"
          :y1="leftFootPosTop"
          :x2="waistPosLeft"
          :y2="waistPosTop"
          :fill="'#302c2c'"
          :stroke="'#302c2c'"
          :stroke-width="5"
          :selectable="false"
          :evented="false"
          :origin-x="'center'"
          :origin-y="'center'"
        ></fabric-line>
        <fabric-line
          :id="'waistToRightFoot'"
          :x1="rightFootPosLeft"
          :y1="rightFootPosTop"
          :x2="waistPosLeft"
          :y2="waistPosTop"
          :fill="'#302c2c'"
          :stroke="'#302c2c'"
          :stroke-width="5"
          :selectable="false"
          :evented="false"
          :origin-x="'center'"
          :origin-y="'center'"
        ></fabric-line>
        <fabric-circle
          :id="'head'"
          :left.sync="headPosLeft"
          :top.sync="headPosTop"
          :stroke-width="5"
          :radius="12"
          :fill="'#fff'"
          :stroke="'#666'"
          :origin-x="'center'"
          :origin-y="'center'"
        ></fabric-circle>
        <fabric-circle
          :id="'body'"
          :left.sync="bodyPosLeft"
          :top.sync="bodyPosTop"
          :stroke-width="5"
          :radius="12"
          :fill="'#fff'"
          :stroke="'#666'"
          :origin-x="'center'"
          :origin-y="'center'"
        ></fabric-circle>
        <fabric-circle
          :id="'waist'"
          :left.sync="waistPosLeft"
          :top.sync="waistPosTop"
          :stroke-width="5"
          :radius="12"
          :fill="'#fff'"
          :stroke="'#666'"
          :origin-x="'center'"
          :origin-y="'center'"
        ></fabric-circle>
        <fabric-circle
          :id="'leftHand'"
          :left.sync="leftHandPosLeft"
          :top.sync="leftHandPosTop"
          :stroke-width="5"
          :radius="12"
          :fill="'#fff'"
          :stroke="'#666'"
          :origin-x="'center'"
          :origin-y="'center'"
        ></fabric-circle>
        <fabric-circle
          :id="'rightHand'"
          :left.sync="rightHandPosLeft"
          :top.sync="rightHandPosTop"
          :stroke-width="5"
          :radius="12"
          :fill="'#fff'"
          :stroke="'#666'"
          :origin-x="'center'"
          :origin-y="'center'"
        ></fabric-circle>
        <fabric-circle
          :id="'leftFoot'"
          :left.sync="leftFootPosLeft"
          :top.sync="leftFootPosTop"
          :stroke-width="5"
          :radius="12"
          :fill="'#fff'"
          :stroke="'#666'"
          :origin-x="'center'"
          :origin-y="'center'"
        ></fabric-circle>
        <fabric-circle
          :id="'rightFoot'"
          :left.sync="rightFootPosLeft"
          :top.sync="rightFootPosTop"
          :stroke-width="5"
          :radius="12"
          :fill="'#fff'"
          :stroke="'#666'"
          :origin-x="'center'"
          :origin-y="'center'"
        ></fabric-circle
        >``
      </fabric-canvas>
    </div>
    <div class="absolute bottom-10 left-20 z-30">
      <typical
        class="vt-title text-blue-400 xl:text-2xl"
        :steps="['Hello', 1000, 'Hello world!', 500]"
        :wrapper="'h2'"
      ></typical>
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
      headPosLeft: 250,
      headPosTop: 125,
      bodyPosLeft: 250,
      bodyPosTop: 175,
      waistPosLeft: 250,
      waistPosTop: 250,
      leftHandPosLeft: 175,
      leftHandPosTop: 225,
      rightHandPosLeft: 325,
      rightHandPosTop: 225,
      leftFootPosLeft: 200,
      leftFootPosTop: 350,
      rightFootPosLeft: 300,
      rightFootPosTop: 350,

      options: {
        len: 200, // The unilateral length of the pentagon
        count: 50, // How many lines overlap
        rate: 20, // rate the smaller fast
        dieChance: 0.5, // The chance to #302c2craw a single painting failure.
        sparkChance: 0.05, // [0,1] The larger the figure, the larger the pentagon.
        sparkDist: 100, // Flash point distance.
        sparkSize: 1, // Flash point size.
        contentLight: 60, // [0,100] Brightness of color block
        shadowToTimePropMult: 6, // The shadow size of the inner ring of the pentagon.
        bgColorArr: [0, 0, 0], // Background color array
      },
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
  background-color: black;
}
</style>
