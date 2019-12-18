<template>
  <div class="header-conatiner">
    <div class="mobile-menu" :class="{'active':menuOpen}" @click="openMenu">
      <label></label>
      <label></label>
      <label></label>
    </div>
    <div class="logo-container">
      <p>
        Company
        <span>Logo</span>
      </p>
    </div>
    <div class="menu-container" :class="{'active':menuOpen}">
      <ul>
        <li class="active">About</li>
        <li>Services</li>
        <li>Solutions</li>
        <li>Blog</li>
        <li>
          <button>Get In Touch</button>          
        </li>
      </ul>      
    </div>
    <div class="touch-icon">
            <img src="../assets/touch-icon.png" alt="touch">
          </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      menuOpen: false
    };
  },
  methods: {
    openMenu() {
      this.menuOpen = !this.menuOpen;
    }
  }
};
</script>


