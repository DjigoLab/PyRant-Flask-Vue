<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/api">API Sample</router-link>
    </div>
    <div id="logos">
      <p>
        <img src="./assets/vue-logo.png">
        <span id="plus">+</span>
        <img src="./assets/flask-logo.png">
      </p>
    </div>
    <nav id="menu">
      <ul>
        <a href=""><li>HOME</li></a>
        <a href="">LOGIN</a>
        <a href=""><li>SETTINGS</li></a>
      </ul>
    </nav>
    <router-view/>
  <footer id="tag-navigator"> 
    <ul>
        <a href=""><li>PYTHON</li></a>
        <a href="">JS</a>
        <a href=""><li>CSS</li></a>
    </ul>
  </footer>

  </div>
</template>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 20000px;;
  
}
#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
#plus {
  padding: 0 20px 0 20px;
  display: inline-block;
  font-size: 50px;
  vertical-align: top;
  line-height: 100px;
}


//What Antonio is using 
#menu, #tag-navigator {
  border: 1px solid black;
  ul {
    display: flex;
    justify-content: center;
    padding: 0;
    li {
      list-style-type: none;
      padding: 0px 15px;
    }
  }
}

#tag-navigator{
  position: fixed;
  height: 60px;
  width: 80%;
  top:calc(100% - 60px);
  left: 50%;
  transform: translate(-50%, 0);
  border-top-left-radius: 10px;
  border-top-right-radius: 10px;

  
  
}
</style>
