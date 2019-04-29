<template>
  <div>
    <nav class="navbar">
      <router-link
        class="spacing"
        v-for="routes in links"
        v-bind:key="routes.id"
        :to="`${routes.page}`"
      >{{routes.text}}</router-link>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Navigation",
  data() {
    return {
      links: [
        {
          id: 0,
          text: "Home",
          page: "/Home"
        },
        {
          id: 1,
          text: "About",
          page: "/About"
        },
        {
          id: 2,
          text: "Contact",
          page: "/Contact"
        }
      ]
    };
  }
};
</script>

<style>
.spacing {
  margin-right: 10px;
  border: solid 1px;
  border-color: #ebe7e2;
  padding: 10px;
  color: #512b2b;
}
.navbar {
  font-family: HeadlineBlack, Arial, sans-serif;
  font-weight: bold;
  background-color: #fefefe;
  padding: 20px;
  margin-bottom: 100px;
  border-top: solid 10px;
  border-top-color: #fa8324;
  position: absolute;
  text-align: left;
  min-width: 100%;
}
body {
  background-color: #fbf2ea;
}
</style>