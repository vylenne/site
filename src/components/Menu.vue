<template>
  <div class="menu">
    <router-link class="menu__logo" to="/">Vilena Vorobyeva</router-link>
    <div class="menu__links">
      <router-link to="/experience">Experience</router-link>
      <router-link to="/services">Services</router-link>
      <router-link to="/works">Works</router-link>
      <router-link to="/contacts">Contact</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Menu',
};
</script>

<style scoped>
.menu {
  width: 200px;
  padding: 40px 0 40px 24px;
  box-sizing: border-box;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.menu__logo {
  text-decoration: none;
  font-family: 'Syne', sans-serif;
  font-size: 2.5rem;
  display: block;
}

.menu__links a {
  color: #1D1D1D;
  text-decoration: none;
  font-family: 'Spartan', sans-serif;
  font-weight: bold;
  display: block;
  margin: 24px 0;
  font-size: 1rem;
}

.menu__links a:after,
.menu__logo:after {
  background: none repeat scroll 0 0 transparent;
  top: 0;
  content: "";
  display: block;
  height: 4px;
  left: 50%;
  position: absolute;
  background: rgba(44, 111, 243, 0.8);
  transition: width 0.3s ease 0s, left 0.3s ease 0s;
  width: 0;
}
.menu__links a:hover:after, .menu__logo:hover:after {
  width: 100%;
  left: 0;
}

@media screen and (max-width: 500px) {
  .menu {
    width: 40px;
    padding: 8px 0;
    align-items: center;
  }

  .menu__logo {
    font-size: 2rem;
    writing-mode: vertical-rl;
    transform:rotate(-180deg);
  }

  .menu__links a {
    writing-mode: vertical-rl;
    transform:rotate(-180deg);
  }
  .menu__links a:after,
  .menu__logo:after {
    display: none;
  }
}
</style>
