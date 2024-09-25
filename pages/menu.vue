// pages/menu.vue
<template>
  <div class='grid-container'>
      <div class='grid'>
        <div class='grid-item'>
          <div class='text-container'>
            <div class='grid-header'>Bao Bun</div>
            <div class='grid-subheader'>Yummy chicken</div>
            <div class='price'>£12</div>
          </div>
          <img class='food-pic' src='https://images.unsplash.com/photo-1620108092667-dd0d0d61df2c?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwxNDU4OXwwfDF8cmFuZG9tfHx8fHx8fHx8MTYyMDI4NjYyMQ&ixlib=rb-1.2.1&q=80&w=400'/>
        </div>
        <div class='grid-item'>
          <div class='text-container'>
            <div class='grid-header'>Bao Bun</div>
            <div class='grid-subheader'>Yummy chicken</div>
            <div class='price'>£12</div>
          </div>
          <img class='food-pic' src='https://images.unsplash.com/photo-1620108092667-dd0d0d61df2c?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwxNDU4OXwwfDF8cmFuZG9tfHx8fHx8fHx8MTYyMDI4NjYyMQ&ixlib=rb-1.2.1&q=80&w=400'/>
        </div>
        <div class='grid-item'>
          <div class='text-container'>
            <div class='grid-header'>Bao Bun</div>
            <div class='grid-subheader'>Yummy chicken</div>
            <div class='price'>£12</div>
          </div>
          <img class='food-pic' src='https://images.unsplash.com/photo-1620108092667-dd0d0d61df2c?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwxNDU4OXwwfDF8cmFuZG9tfHx8fHx8fHx8MTYyMDI4NjYyMQ&ixlib=rb-1.2.1&q=80&w=400'/>
        </div>
        <div class='grid-item'>
          <div class='text-container'>
            <div class='grid-header'>Bao Bun</div>
            <div class='grid-subheader'>Yummy chicken</div>
            <div class='price'>£12</div>
          </div>
          <img class='food-pic' src='https://images.unsplash.com/photo-1620108092667-dd0d0d61df2c?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwxNDU4OXwwfDF8cmFuZG9tfHx8fHx8fHx8MTYyMDI4NjYyMQ&ixlib=rb-1.2.1&q=80&w=400'/>
        </div>
        <div class='grid-item'>
          <div class='text-container'>
            <div class='grid-header'>Bao Bun</div>
            <div class='grid-subheader'>Yummy chicken</div>
            <div class='price'>£12</div>
          </div>
          <img class='food-pic' src='https://images.unsplash.com/photo-1620108092667-dd0d0d61df2c?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwxNDU4OXwwfDF8cmFuZG9tfHx8fHx8fHx8MTYyMDI4NjYyMQ&ixlib=rb-1.2.1&q=80&w=400'/>
        </div>
        <div class='grid-item'>
          <div class='text-container'>
            <div class='grid-header'>Bao Bun</div>
            <div class='grid-subheader'>Yummy chicken</div>
            <div class='price'>£12</div>
          </div>
          <img class='food-pic' src='https://images.unsplash.com/photo-1620108092667-dd0d0d61df2c?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwxNDU4OXwwfDF8cmFuZG9tfHx8fHx8fHx8MTYyMDI4NjYyMQ&ixlib=rb-1.2.1&q=80&w=400'/>
        </div>
        </div>
      </div>
</template>
<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}


#content {
    height: 100vh;
    width: 100vw;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
  
    font-size: 18px;
    font-family: sans-serif;
    color: red;
  
    background: url(https://images.unsplash.com/photo-1619367436851-715cdc4f1e09?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxNDU4OXwwfDF8cmFuZG9tfHx8fHx8fHx8MTYyMDIwODk3Nw&ixlib=rb-1.2.1&q=85) no-repeat center center fixed; 
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;
}

.nav-bar {
  position: absolute;
  top: 0;
  height: 50px;
  display: flex;
  justify-content: center;
  padding: 15px;
  background-color: black;
  opacity: 80%;
  width: 100%;
  z-index: 23;
}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

ul > li {
  display: inline;
  margin-right: 50px;
}

a:link {
  color: white;
  text-decoration: none;
}
a:hover {
  text-decoration: underline;
}

.header {
  display: flex;
  background-color: black;
  padding: 20px;
  opacity: 80%;
  font-size: 40px;
  border-radius: 10px;
}

.subheader {
  display: flex;
  background-color: black;
  padding: 20px;
  opacity: 80%;
  font-size: 20px;
  border-radius: 10px;
  margin-top: 30px;
}

.grid-container {
    display: flex;
    justify-content: center;
    font-family: 'Yusei Magic', sans-serif;
}
  
.grid {
    width: 100%;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.grid-item {
    /*height: 180px;*/
    padding: 30px 30px;
    text-align: left;
    border: 2px solid black;
    border-radius: 5px;
    margin: 30px 30px;
    line-height: 1.5;
    background-color:lemonchiffon;
    /*opacity: 80%;*/
    display: flex;
    flex-direction: row;
}

.text-container {
  display: flex;
  flex-direction: column;
  margin-right: 20px;
  align-items: space-between;
  justify-content: space-around;
}

.grid-header {
    display: flex;
    font-size: 20px;
    
}

.grid-subheader {
    display: flex;
    font-size: 15px;
}

.price {
  display: flex;
  font-size: 20px;
}

.food-pic {
  display: flex;
  width: 250px;
}
</style>