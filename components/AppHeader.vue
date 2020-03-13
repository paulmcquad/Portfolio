<template>
  <header class="header">
    <img src="~/assets/coderforge.jpg" class="logo img-rounded" height="84" width="84">
    <h1 class="title">Coder Forge</h1>
    <ul>
      <li>
        <nuxt-link to="/">Home</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/jokes">Jokes</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/about">About</nuxt-link>
      </li>
      <li>
        <div>

        <div class="dropdown">
        <nuxt-link to="/about">Drop</nuxt-link>
            <i class="fa fa-caret-down"></i>
          </button>
          <div class="dropdown-content">
            <a href="/bob">Link 1</a>
            <a href="/alice">Link 2</a>
            <a href="/sam">Link 3</a>
          </div>
        </div> 
        </div>
      </li>
    </ul>
   </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader"
};
</script>

<style>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 1rem;
  padding-bottom: 1rem;
  border-bottom: 1px dotted #ccc;
}
.header .title {
  font-size: 3rem;
  color: #ce8e29;

}
.header ul {
  display: flex;
}
.header a {
  display: inline-block;
  background:#ce8e29;
  color: #fff;
  padding: 0.3rem 1rem;
  margin-right: 0.5rem;
}


.dropdown .dropbtn {
  font-size: 16px;  
  border: none;
  outline: none;
  color: white;
  padding: 14px 16px;
  background-color: inherit;
  font-family: inherit;
  margin: 0;
}


.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 80px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
}

.dropdown-content a {
  float: none;
  color: white;
  padding: 12px 20px;
  text-decoration: none;
  display: block;
  text-align: left;
}

.dropdown:hover .dropdown-content {
  display: block;
}

</style>