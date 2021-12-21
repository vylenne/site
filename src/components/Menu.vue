<template>
  <div class="menu">
    <router-link class="menu__logo" to="/">Vilena Vorobyeva</router-link>
    <div class="menu__links">
      <router-link to="/experience">Experience</router-link>
      <router-link to="/services">Services</router-link>
      <router-link to="/works">Works</router-link>
      <router-link to="/contacts">Contact</router-link>
    </div>
    <div class="menu__contacts">
      <div class="contacts__cv">
        <a href="https://resume.io/r/qyEHdOgHY" target="_blank">Check CV</a>
      </div>
      <div class="contacts__email">
        <p>Contact me :)</p>
        <a href="mailto:v.vylenne@gmail.com" target="_blank">v.vylenne@gmail.com</a>
      </div>
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
  width: 240px;
  padding: 40px 24px;
  box-sizing: border-box;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  position: sticky;
  top: 0;
  left: 0;
  bottom: 0;
}

.menu__logo {
  text-decoration: none;
  font-family: 'Syne', sans-serif;
  font-size: 1.5rem;
  display: block;
}

.menu__links a {
  color: #1D1D1D;
  text-decoration: none;
  font-family: 'Spartan', sans-serif;
  font-weight: bold;
  display: block;
  margin: 1.5rem 0;
  font-size: .875rem;
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

.contacts__cv {
  margin-bottom: 40px;
}

.contacts__cv a {
  font-family: 'Syne', sans-serif;
  font-size: 1.25rem;
  color: #2C6FF3;
  background: linear-gradient(to bottom, #2C6FF3 0%, #2C6FF3 100%);
  background-position: 0 105%;
  background-repeat: repeat-x;
  background-size: 2px 2px;
  text-decoration: none;
}

.contacts__cv a:hover {
  background-image: url("data:image/svg+xml;charset=utf8,%3Csvg id='squiggle-link' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' xmlns:ev='http://www.w3.org/2001/xml-events' viewBox='0 0 20 4'%3E%3Cstyle type='text/css'%3E.squiggle{animation:shift .3s linear infinite;}@keyframes shift {from {transform:translateX(0);}to {transform:translateX(-20px);}}%3C/style%3E%3Cpath fill='none' stroke='%232C6FF3' stroke-width='2' class='squiggle' d='M0,3.5 c 5,0,5,-3,10,-3 s 5,3,10,3 c 5,0,5,-3,10,-3 s 5,3,10,3'/%3E%3C/svg%3E");
  background-position: 0 100%;
  background-size: auto 3px;
  background-repeat: repeat-x;
  text-decoration: none;
}

.contacts__email {
  font-family: 'Spartan', sans-serif;
  font-size: .875rem;
}

.contacts__email p {
  font-weight: 600;
  margin-bottom: .5rem;
}

.contacts__email a {
  color: #2C6FF3;
  background: linear-gradient(to bottom, #2C6FF3 0%, #2C6FF3 100%);
  background-position: 0 105%;
  background-repeat: repeat-x;
  background-size: 2px 2px;
  text-decoration: none;
}

@media screen and (max-width: 500px) {
  .menu {
    width: 40px;
    padding: 8px;
    align-items: center;
  }

  .menu__logo {
    font-size: 1.25rem;
    writing-mode: vertical-rl;
    transform:rotate(-180deg);
  }

  .menu__links a {
    writing-mode: vertical-rl;
    margin: 1rem 0;
    transform:rotate(-180deg);
  }

  .contacts__cv {
    writing-mode: vertical-rl;
    transform:rotate(-180deg);
    margin-bottom: 0;
  }

  .menu__links a:after,
  .menu__logo:after,
  .contacts__email {
    display: none;
  }
}
</style>
