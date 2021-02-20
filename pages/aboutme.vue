<template>
  <div>
    <navbar-2></navbar-2>
    <div
      class="flex flex-col absolute top-20 lg:top-64 lg:left-48 lg:flex-row flex-wrap"
    >
      <div class="flex flex-wrap justify-center mx-auto items-center">
        <div>
          <img
            class="ml-4"
            width="320px"
            height="320px"
            src="../assets/images/1.jpg"
            alt=""
          />
        </div>
      </div>
      <div>
        <ul class="list-none mx-2 mt-10 text-xl lg:mt-0 lg:ml-20 uppercase">
          <li>Name : <span> Mohamed Adel</span></li>
          <li>My jop : <span>Full stack Devolover</span></li>
          <li>country : <span>Sudan</span></li>
          <li>experinse ears : <span>2 ears</span></li>
          <li>numbers of projects : <span>20</span></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style scoped>
ul li {
  @apply text-gray-300 leading-9;
}

ul li span {
  @apply text-white;
}
</style>
