<template>
  <div id="app">
    <Nav></Nav>
      <div class="marginPrincipal">
        <router-view :key="$route.fullPath"></router-view>
      </div>
  </div>
</template>

<script>

import Nav from './components/_nav/Nav'

export default {
  name: 'App',
  components: {
 
    Nav
  }
}
</script>

<style >
@import url("https://fonts.googleapis.com/css2?family=Lato:ital,wght@1,300&display=swap" );
body{
  background-color: rgba(78, 151, 180, 0.411);
  font-family: 'Lato', sans-serif;
  display: grid;
  justify-items: center;
}
body, html{
  margin: 0px;
  height: 100%;
}
.marginPrincipal{
  width: 50%;
  margin: auto;

}
#app{
  width: 100%;
  
}

.btn_Danger{
  font-size: 0.8em !important;
  background-color: rgb(128, 189, 170);
}

.btn{
  padding: 10px 20px;
  cursor: pointer;
  border: 1px solid rgb(248, 247, 247);
  font-size: 1.2em;
  color: white;
  font-weight: bold;
  border-radius: 5px;
}
.btn:hover{
  
}
table{
  margin: 0px;
  padding: 0px;
  list-style-type: none;
  width: 100%;
}
table tr td {
  padding: 20px;
  font-size: 1.3em;
  background-color: rgba(76, 126, 146, 0.096);
  margin-bottom: 2px;
  color: #3e5252;
}
table thead th{
  background-color: rgba(73, 103, 138, 0.568);
  font-size: 1.2em;
  padding: 10px 10px;
  text-align: center im !important;  
}
.colPequeno{
  width: 5%;
   text-align: right;
  background-color: rgba(94, 161, 187, 0.712);
  font-weight: bold;
}
</style>
