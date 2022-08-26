<template>
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}


</script>



<style>
body{
  margin: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.all{
    display: flex;
    font-size: 1.10rem;
}


/* navbar */


.navbar{
    display: flex;
    justify-content: space-between;
    color: #737373;
    border-bottom: 1px lightgray solid;
   
    height: 40px;
    width: 80vw;
    padding: 5px;
    align-items: center;
}

.navbar>div{
    display: flex;
}

.nav_left{
    margin-left: 15px ;
}

.nav_right{
    margin-right: 15px;
}

.nav_left>div{
    padding: 10px;
}

.nav_right>i{
    padding: 10px;
}

.tirait{
    width: 25px;
}
.tirait>div{
    border-bottom: 1px #737373 solid;
    height: 6px;

}

/* section */

.section{
    display: flex;
    justify-content: space-between;
    border-bottom: 1px lightgray solid;
    height: 40px;
    width: 80vw;
    padding: 5px;
    align-items: center;
}


/* sidebar */

.sidebar{
    padding: 10px;
    background : rgb(59, 75, 100);
    width: 300px;
    color: #bfbfbf;
}

.sidebar>div{
    margin: 15px;
}

.mainpart{
    background : rgb(236, 237, 241);
    width: 100%;
}

.first{
    justify-content: space-around;
}

.first>div{
    border-radius: 3px;
}

.users{
    width: 21%;
    height: 170px;
    background-color: rgb(50, 31, 219);
}

.income{
    width: 21%;
    height: 170px;
    background-color: rgb(53, 152, 254);
}

.rate{
    width: 21%;
    height: 170px;
    background-color: rgb(248, 178, 22);
}

.sessions{
    width: 21%;
    height: 170px;
    background-color: rgb(229, 83, 83);
}

.sec{
    display: flex;
    width: 90%;
    height: 500px;
    background-color: white;
    justify-content: center;
    
}



</style>
