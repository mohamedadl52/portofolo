<template>
  <div class="bgground">
    <navbar-3></navbar-3>
    <div class="absolute top-48 md:right-32 lg:right-64 leading-10 mx-2">
      <form action="" class="mx-auto">
        <input
          id=""
          type="text"
          name=""
          placeholder="name"
          class="w-full md:w-56"
        />
        <input
          id=""
          type="email"
          name=""
          placeholder="email"
          class="w-full md:w-64"
        />
        <br />
        <input
          id=""
          type="text"
          name=""
          placeholder="subject"
          class="w-full p-0"
        />
        <br />
        <textarea class="w-full" rows="6" placeholder="message"></textarea>

        <button
          style="background-color: #5a4b4b"
          class="border-black border-2 w-32 mx-auto block"
        >
          Send
        </button>
      </form>
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
input {
  padding: 2px;
}
.bgground {
  background-color: #797171;
}
</style>
