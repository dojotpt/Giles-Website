<template>
  <div id=background>
  <header id="app-header">
    <div class="logo">
    <img id="logo-img" src="@/images/headerImage.jpg" alt="picture of wedding rings">
    </div>

    <div class="nav">
      <router-link class="nav-a" v-bind:to="{ name: 'home' }">Home</router-link>
      <router-link class="nav-a" v-bind:to="{ name: 'about' }">About</router-link>
      <router-link class="nav-a" v-bind:to="{ name: 'booking' }">Booking</router-link>
      <router-link class="nav-a" v-bind:to="{ name: 'highlights' }">Highlights</router-link>
      <router-link class="nav-a" v-bind:to="{ name: 'reviews' }">Reviews</router-link>
      <router-link class="nav-a" v-bind:to="{ name: 'contact' }">Contact</router-link>
      <router-link class="nav-a" v-bind:to="{ name: 'faq' }">FAQ</router-link>
    </div>
    <div class="s-media">
      <img src="@/images/instagram.png" class="social-icon" alt="instagram" />
      <img src="@/images/linkedin.png" class="social-icon" alt="linkedin" />
      <img src="@/images/facebook.png" class="social-icon" alt="facebook" />
      <img src="@/images/x.png" class="social-icon" alt="link to x"/>      
    </div>
  </header>
  <router-view />
</div>
</template>

<style>
#app-header {
}

header {
  
  display: grid;
  grid-template-columns: auto 1fr auto;
  grid-template-areas:
    "logo nav s-media";
  align-items: center;
  background-color: #36454F;
  padding: 0.25%;
  border-bottom: 2px solid #D4AF37;
}

.logo {
  grid-area: logo;
  display: flex;
  justify-content: flex-start;
  align-items: center;
  padding-left: 2.5%;
}

#logo-img {
  height: 100%;
  width: 15%;
  border-radius: 50%;
}

.nav {
  grid-area: nav;
  color: #F5F5DC;
  display: flex;
  justify-content:center;
  align-items: center;
  text-align: center;
  font-size: 150%;
}

.nav-a {
  color: inherit;
  text-decoration: none; 
  padding: 5%;
}

#nav a:hover {
  color: #D4AF37;
}

.s-media {
  grid-area: s-media;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  gap: 10px;
  padding-right: 5%;
}
.social-icon {
width: 5%;
}
#background {
  background-color: #F5F5DC;
  height: 100vh;
}
</style>