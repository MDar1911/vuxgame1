<template>
   <div id = "app">
     <section class = "row">
       <div class = "small-6 columns">
         <h1 class="text-center">玩家</h1>
         <div class = "healthbar">
           <div class = "healthbar text-center"
           style="background-color: green; margin: 0; color: white;">
             
           </div>
         </div>
       </div>
       <div class = "small-6 columns">
         <h1 class="text-center">怪兽</h1>
         <div class = "healthbar">
           <div class = "healthbar text-center"
           style="background-color: green; margin: 0; color: white;">
             
           </div>
         </div>
       </div>
     </section>
     <section class = "row controls">
         <div class = "small-12 columns">
             <button id = "start-game">开始游戏</button>
         </div>
     </section>
     <section class = "row controls">
         <div class = "small-12 columns">
             <button id = "attack">暴击</button>
             <button id = "special-attact">放大招</button>
             <button id = "heal">治愈</button>
             <button id = "give-up">投降</button>
         </div>
     </section>
     <section class = "row log">
         <div class = "small-12 columns">
             <ul>
                 <li>
                   
                 </li>
             </ul>
         </div>
     </section>
   </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.text-center {
    text-align: center;
}

.healthbar {
    width: 80%;
    height: 40px;
    background-color: #eee;
    margin: auto;
    transition: width 500ms;
}

.controls, .log {
    margin-top: 30px;
    text-align: center;
    padding: 10px;
    border: 1px solid #ccc;
    box-shadow: 0px 3px 6px #ccc;
}

.turn {
    margin-top: 20px;
    margin-bottom: 20px;
    font-weight: bold;
    font-size: 22px;
    
}

.log ul {
    list-style: none;
    font-weight: bold;
    text-transform: uppercase;
}

.log ul li {
    margin: 5px;
    
}

.log ul .player-turn {
    color: blue;
    background-color: #e4e8ff;
}

.log ul .monster-turn {
    color: red;
    background-color: #ffc0c1;
}

button {
  font-size: 20px;
  background-color: #eee;
  padding: 12px;
  box-shadow: 0 1px 1px black;
  margin: 10px;
}
#start-game {
    background-color: #aaffb0;
}

#start-game:hover {
    background-color: #76ff7e;
}

#attack {
    background-color: #ff7367;
}

#attack:hover {
    background-color: #ff7367;
}
#special-attact {
    background-color: #ffaf4f;
}

#special-attact:hover {
    background-color: #ffaf4f;
}

#heal {
    background-color: #aaffb0;
}

#heal:hover {
    background-color: #aaffb0;
}

#give-up {
    background-color: #ffffff;
}

#give-up:hover {
    background-color: #c7c7c7;
}
</style>
