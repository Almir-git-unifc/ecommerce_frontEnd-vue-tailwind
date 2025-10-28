<template>
  <header class="sticky top-0 z-50 transition-all duration-300">
    <section
      :class="[
        'w-full', isScrolled  ? 'bg-gray-100/95 backdrop-blur shadow-md py-2' : 'bg-gray-100 py-4',
      ]"
    >
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div
          class="flex flex-col md:flex-row items-center justify-between gap-3 md:gap-6"
        >
          <!-- Logo + Mobile Menu Toggle -->
          <div class="flex justify-between items-center w-full md:w-auto">
            <a href="/" class="text-2xl font-bold text-pink-600">ShopEase</a>
            <button
              class="md:hidden text-gray-700 hover:text-indigo-600"
              aria-label="Toggle mobile menu"
              @click="isMobileMenuOpen = !isMobileMenuOpen"
            >
              <Icon icon="mdi:menu" class="w-6 h-6" />
            </button>
          </div>

          <!-- Search bar   - - - - - - - - - - - -    -->
          <form
            class="w-full md:flex-1 max-w-sm"   role="search"  aria-label="Site search"
          >
            <label class="relative w-full">
              <input  type="text"  placeholder="Search ..."
                class="w-full px-3 py-2 text-xs border border-gray-300 rounded-full focus:outline-none focus:ring-2 focus:ring-indigo-500"
              />
              <button
                type="submit"
                class="absolute right-2 top-1/2 -translate-y-1/2 text-gray-500 hover:text-indigo-600"
                aria-label="Search button"
              >
                <Icon icon="mdi:magnify" class="w-4 h-4" />
              </button>
            </label>
          </form>

          <!-- Icons  - - - - - - - -  -->
          <aside
            class="flex items-center justify-end space-x-4 w-full md:w-auto"
          >
            <button
              class="relative p-2 text-gray-700 hover:text-pink-600"
              aria-label="Wishlist"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"  width="24" height="24"  viewBox="0 0 24 24"
              >
                <path
                  fill="currentColor"
                  d="m12.1 18.55l-.1.1l-.11-.1C7.14 14.24 4 11.39 4 8.5C4 6.5 5.5 5 7.5 5c1.54 0 3.04 1 3.57 2.36h1.86C13.46 6 14.96 5 16.5 5c2 0 3.5 1.5 3.5 3.5c0 2.89-3.14 5.74-7.9 10.05M16.5 3c-1.74 0-3.41.81-4.5 2.08C10.91 3.81 9.24 3 7.5 3C4.42 3 2 5.41 2 8.5c0 3.77 3.4 6.86 8.55 11.53L12 21.35l1.45-1.32C18.6 15.36 22 12.27 22 8.5C22 5.41 19.58 3 16.5 3"
                />
              </svg>
              <span
                class="absolute -top-1 -right-1 bg-pink-500 text-white text-xs rounded-full h-5 w-5 flex items-center justify-center"
              >
                3
              </span>
            </button>

            <button
              class="relative p-2 text-gray-700 hover:text-pink-600"
              aria-label="Wishlist"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"   width="24"  height="24"   viewBox="0 0 24 24"
              >
                <path
                  fill="currentColor"
                  d="M17 18a2 2 0 0 1 2 2a2 2 0 0 1-2 2a2 2 0 0 1-2-2c0-1.11.89-2 2-2M1 2h3.27l.94 2H20a1 1 0 0 1 1 1c0 .17-.05.34-.12.5l-3.58 6.47c-.34.61-1 1.03-1.75 1.03H8.1l-.9 1.63l-.03.12a.25.25 0 0 0 .25.25H19v2H7a2 2 0 0 1-2-2c0-.35.09-.68.24-.96l1.36-2.45L3 4H1zm6 16a2 2 0 0 1 2 2a2 2 0 0 1-2 2a2 2 0 0 1-2-2c0-1.11.89-2 2-2m9-7l2.78-5H6.14l2.36 5z"
                />
              </svg>
              <span
                class="absolute -top-1 -right-1 bg-pink-500 text-white text-xs rounded-full h-5 w-5 flex items-center justify-center"
              >
                5
              </span>
            </button>

            <button
              class="relative p-2 text-gray-700 hover:text-pink-600"
              aria-label="Wishlist"
            >
              <Icon icon="mdi:account-outline" class="w-5 h-5">
                <svg
                  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"
                >
                  <path
                    fill="currentColor"
                    d="M12 4a4 4 0 0 1 4 4a4 4 0 0 1-4 4a4 4 0 0 1-4-4a4 4 0 0 1 4-4m0 10c4.42 0 8 1.79 8 4v2H4v-2c0-2.21 3.58-4 8-4"
                  />
                </svg>
                Icon-User
              </Icon>
            </button>
          </aside>
        </div>
      </div>

      <!-- Navbar links Aos 13:04 min.  - - - - - -    -->
      <nav class="bg-pink-950" aria-label="Main navigation">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <ul
            class="hidden md:flex justify-center py-3 flex-wrap gap-x-6 text-sm font-medium text-white"
          >
            <li v-for="item in navItems" :key="item.id">
              <a
                :href="item.link"
                class="hover:text-pink-300 transition-colors"
              >
                {{ item.name }}
              </a>
            </li>
          </ul>
          <section
            v-if="isMobileMenuOpen"
            class="md:hidden mt-2 bg-white rounded-lg shadow-md p-4 space-y-3 text-[#5D4037] text-center"
            aria-label="Mobile Navigation"
          >
            <a
              v-for="item in navItems"  :href="item.link" :key="item.id"
              class="block hover:text-amber-600 text-sm font-medium"
            >
              {{ item.name }}
            </a>
          </section>
        </div>
      </nav>
    </section>
  </header>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from "vue";
const isScrolled = ref(false);
const isMobileMenuOpen = ref(false);
const navItems = [
  { id: 1, name: "Home", link: "#home" },
  { id: 2, name: "Products", link: "#products" },
  { id: 3, name: "Categories", link: "#categories" },
  { id: 4, name: "Offers", link: "#offers" },
  { id: 5, name: "About", link: "#about" },
  { id: 6, name: "Contact", link: "#contact" },
];

const handleScroll = () => {
  isScrolled.value = window.scrollY > 10;
};

onMounted(() => {
  window.addEventListener("scroll", handleScroll);
});

onUnmounted(() => {
  window.removeEventListener("scroll", handleScroll);
});
</script>
