<template>
  <nav
    style="background-color: white"
    class="
      border-solid
      fixed
      bg-red
      w-full
      z-20
      px-6
      py-4
      md:flex md:justify-between md:items-center
    "
  >
    <div class="flex items-center justify-between mt-3">
      <span style="color: blueviolet">IDYLLIC</span>

      <!-- Mobile menu button -->
      <div @click="showMenu = !showMenu" class="flex md:hidden">
        <button
          type="button"
          class="
            text-gray-800
            hover:text-gray-400
            focus:outline-none focus:text-gray-400
          "
        >
          <svg viewBox="0 0 24 24" class="w-6 h-6 fill-current">
            <path
              fill-rule="evenodd"
              d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"
            ></path>
          </svg>
        </button>
      </div>
    </div>

    <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
    <ul
      :class="showMenu ? 'flex' : 'hidden'"
      class="
        flex-col
        mt-8
        space-y-4
        md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0
      "
    >
      <li
        class="text-sm font-bold text-black-800 hover:text-blue-400"
        v-for="(item, $index) in items"
        :key="$index"
      >
        <a
          @click="setUrlSection(item.section)"
          :href="item.link"
          :class="{ active: urlSection === item.link }"
          >{{ item.name }}</a
        >
      </li>
      <!-- <li class="text-sm font-bold text-black-800 hover:text-blue-400">
        <a  href="#Home">Home</a>
      </li>
      <li class="text-sm font-bold text-black-800 hover:text-blue-400">
        <a href="#About">About</a>
      </li>
      <li class="text-sm font-bold text-black-800 hover:text-blue-400">
        <a href="#Gallery">Gallery</a>
      </li>
      <li class="text-sm font-bold text-black-800 hover:text-blue-400">
        <a href="#Contacts">Contacts</a>
      </li> -->
    </ul>
  </nav>
</template>
<script>
export default {
  data() {
    return {
      showMenu: false,
      items: [
        {
          name: "Home",
          link: "#Home",
          section: "hash",
        },
        {
          name: "About",
          link: "#About",
          section: "hash",
        },
        {
          name: "Gallery",
          link: "#Gallery",
          section: "hash",
        },
        {
          name: "Contacts",
          link: "#Contacts",
          section: "hash",
        },
      ],
      urlSection: window.location.hash || window.location.pathname,
    };
  },
  methods: {
    setUrlSection(section) {
      setTimeout(() => (this.urlSection = window.location[section]));
    },
  },
};
</script>
<style scoped>
span {
  font-size: 25px;
  font-weight: 700;
  font-family: Josefin Sans;
  gap: 2px;
}
ul li .active {
  text-decoration: underline;
  color: green;
}
</style>