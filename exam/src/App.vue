<template>
  <div id="app">
    <main>
        <router-view/>
    </main>
    <div id="footer">
      <router-link to="/" tag='span'>Home</router-link> |
      <router-link to="/my" tag='span'>My</router-link>
    </div>
  </div>
</template>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
}
html,body,#app {
  width: 100%;
  height: 100%;
}
#app{
  display: flex;
  flex-direction: column;
}
main{
  flex: 1
}
#footer{
  height: 44px;
  line-height: 44px;
  display: flex;
  span{
    text-align: center;
    flex: 1
  }
}
</style>
