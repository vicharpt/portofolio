<template>
  <header :class="'bg-transparent absolute top-0 left-0 w-full flex items-center z-10 ' + navbarFixed ">
    <div class="container">
      <div class="flex items-center justify-between relative">
        <div class="px-4">
          <a :href="navLink[0].link" class="font-bold text-md text-primary block py-6">IndraSaputra</a>
        </div>
        <div class="flex items-center px-4">
          <button :class="'block absolute right-4 md:hidden ' + hamburgerActive" @click="handleToggle">
            <span class="hamburger-line origin-top-left"></span>
            <span class="hamburger-line"></span>
            <span class="hamburger-line origin-bottom-left"></span>
          </button>

          <nav :class="navMenu + ' absolute py-5 bg-white shadow-lg rounded-lg max-w-[250px] w-full right-4 top-full md:block md:static md:bg-transparent md:max-w-full md:shadow-none md:rounded-none'">
            <ul class="block md:flex">
              <li v-for="link in navLink" class="group">
                <a :href="link.link" class="text-sm text-dark py-2 mx-8 md:mx-4 flex group-hover:text-primary">{{ link.menu }}</a>
              </li>
            </ul>
          </nav>
        </div>
      </div>
    </div>
  </header>
</template>


<script>

  export default {
    data() {
      return {
        hamburgerActive: '',
        navbarFixed: '',
        navMenu: 'hidden',
        navLink: [
          {
            menu: 'Beranda',
            link: '#home'
          },
          {
            menu: 'Tentang Saya',
            link: '#about'
          },
          {
            menu: 'Portofolio',
            link: '#portfolio'
          },
          {
            menu: 'Beranda',
            link: '#home'
          }
        ]
      }
    },
    methods: {
      onScroll() {
        this.navbarFixed = window.scrollY > 0 ? 'navbar-fixed' : ''
      },
      handleToggle() {
        this.hamburgerActive = this.hamburgerActive == 'hamburger-active' ? '' : 'hamburger-active'
        this.navMenu = this.navMenu == 'hidden' ? '' : 'hidden'
      }
    },
    mounted() {
      window.addEventListener('scroll', this.onScroll)
    },
    destroyed() {
      window.removeEventListener('scroll', this.onScroll)
    }
  }


</script>