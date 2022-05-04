<template>
  <nav
    class="w-screen h-32 z-30 flex justify-between items-center px-16 fixed text-white top-0 left-0"
  >
    <div class="w-48 text-center mr-8">
      <div class="w-full flex justify-center align-center">
        <svg
          version="1.0"
          xmlns="http://www.w3.org/2000/svg"
          width="48"
          height="48"
          viewBox="0 0 512 512"
        >
          <path
            d="M2472 5099 c-47 -24 -83 -66 -101 -118 -8 -25 -11 -506 -11 -1798 0
-971 -3 -1763 -7 -1761 -5 2 -30 15 -58 29 -148 79 -335 121 -529 121 -623 -1
-1082 -454 -957 -944 73 -286 345 -519 700 -599 123 -28 312 -35 436 -16 435
67 754 342 805 693 6 43 10 509 10 1222 0 633 2 1152 5 1152 22 0 217 -103
299 -157 292 -194 497 -485 586 -833 l21 -82 -50 -68 c-59 -81 -66 -95 -75
-139 -21 -111 75 -221 193 -221 97 0 139 34 253 204 254 378 385 900 323 1284
-29 180 -107 378 -211 534 -61 91 -203 239 -313 327 -47 38 -174 128 -281 202
-345 235 -443 318 -559 473 -131 174 -172 249 -201 364 -21 82 -109 151 -195
152 -22 0 -59 -10 -83 -21z"
            transform="translate(0.000000,512) scale(0.100000,-0.100000)"
            fill="#fff"
            stroke="none"
          />
        </svg>
      </div>
      <h1 class="text-3xl tracking-wide">Musicology</h1>
    </div>

    <ul
      id="NavItems"
      class="md:flex md:h-full md:relative md:top-0 md:left-0 flex-col md:flex-row justify-between items-center lg:text-3xl text-xl absolute top-32 left-0 text-center h-60 py-4"
    >
      <li>HOME</li>
      <li>PRODUCT</li>
      <li>PROMO</li>
      <li>ABOUT</li>
      <li>CONTACT</li>
    </ul>

    <div class="pl-20 text-center">
      <v-icon dark size="52px">mdi-magnify</v-icon>
    </div>
    <div id="icon" class="cursor-pointer md:hidden">
      <div class="h-1 w-8 bg-white my-2"></div>
      <div class="h-1 w-8 bg-white my-2"></div>
      <div class="h-1 w-8 bg-white my-2"></div>
    </div>
  </nav>
</template>

<script>
export default {
  data: () => ({
    NavBarItems: ["test1", "test2", "test3", "test4", "test5"],
  }),
};
</script>

<style scope>
nav {
  background-color: #2c2c2c;
}
#NavItems {
  width: 750px;
  list-style: none;
}
@media (max-width: 768px) {
  #NavItems {
    display: flex;
    width: 100%;
    background: #2c2c2c;
  }
}
</style>
