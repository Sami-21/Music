<template>
  <nav
    class="w-screen h-32 z-10 flex justify-between items-center px-16 fixed text-white top-0 left-0"
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
      class="md:flex md:h-full md:relative md:top-0 md:left-0 flex-col md:flex-row justify-between items-center lg:text-3xl text-xl absolute top-32 -left-full text-center md:opacity-100 opacity-0 h-60 py-4 z-10 md:border-t-0 border-t-2"
    >
      <li>HOME</li>
      <li>PRODUCT</li>
      <li>PROMO</li>
      <li>ABOUT</li>
      <li>CONTACT</li>
    </ul>

    <div class="pl-28 text-center">
      <v-icon @click="toggleSearchBar()" dark size="52px">mdi-magnify</v-icon>
    </div>
    <div @click="toggleMenu()" id="NavBarIcon" class="cursor-pointer md:hidden">
      <div class="bar1 h-1 w-9 bg-white my-2 duration-300"></div>
      <div class="bar2 h-1 w-9 bg-white my-2 duration-300"></div>
      <div class="bar3 h-1 w-9 bg-white my-2 duration-300"></div>
    </div>
    <div
      id="searchContainer"
      class="flex justify-center items-center w-full h-0 border-t-2 absolute top-32 left-0"
    >
      <input
        type="text"
        placeholder="search..."
        class="bg-gray-200 w-full md:mx-32 mx-12 outline-none p-2 rounded text-black"
      />
    </div>
  </nav>
</template>

<script>
export default {
  data: () => ({
    MenuClosed: true,
    SearchbarClosed: true,
  }),
  methods: {
    toggleMenu() {
      document
        .querySelector("#NavItems")
        .classList.toggle("NavItemsTransition");
      document.querySelector("#NavItems").classList.toggle("-left-full");
      document.querySelector("#NavItems").classList.toggle("left-0");
      document.querySelector("#NavItems").classList.toggle("opacity-0");
      document.querySelector("#NavItems").classList.toggle("opacity-100");
      document.querySelector(".bar1").classList.toggle("bar1_translate");
      document.querySelector(".bar2").classList.toggle("opacity-0");
      document.querySelector(".bar3").classList.toggle("bar2_translate");
      this.menuClosed = !this.menuClosed;
    },
    toggleSearchBar() {
      document.querySelector("#searchContainer").classList.toggle("h-0");
      document.querySelector("#searchContainer").classList.toggle("h-1/2");
      this.searchBarClosed = !this.searchBarClosed;
      if (this.searchBarClosed) {
        document.querySelector("#NavItems").classList.add("top-48");
        document.querySelector("#NavItems").classList.remove("top-32");
      } else {
        document.querySelector("#NavItems").classList.remove("top-48");
        document.querySelector("#NavItems").classList.add("top-32");
      }
    },
  },
};
</script>

<style scope>
nav {
  background-color: #2c2c2c;
}
#NavItems {
  width: 750px;
  list-style: none;
  transition-property: top opacity;
  transition-duration: 500ms;
}

#searchContainer {
  background: #2c2c2c;
  overflow: hidden;
  transition: height 500ms;
}
.bar1_translate {
  transform: rotate(-45deg) translate(-9px, 6px);
}
.bar2_translate {
  transform: rotate(45deg) translate(-9px, -9px);
}
@media (max-width: 768px) {
  #NavItems {
    display: flex;
    width: 100%;
    background: #2c2c2c;
  }
}
</style>
