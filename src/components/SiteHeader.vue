<template>
  <header>
    <div class="container">
      <nav>
        <router-link class="svg-wrapper" to="/">
          <v-icon
            name="home"
            scale="2"
          />
        </router-link>
      </nav>
      <h3 class="title">Catalog</h3>
      <div class="spacer"></div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'SiteHeader',
};
</script>

<style lang="scss" scoped>
header {
  background: $blue;
}

header .container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}

.title {
  margin: 0;
  color: $white;
}

nav {
  a {
    font-weight: bold;

    &.svg-wrapper {
      display: inline-block;

      & svg {
        fill: $white;
        vertical-align: middle;
      }
    }

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
