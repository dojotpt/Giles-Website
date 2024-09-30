<template>
      <div class="page-container">
    
      <div id="card1" class="card"> 
        <h1 id="about1">Jordan Giles</h1>
        <h2 id="about2">Wedding Officiant</h2>
        <img id="card1-image" src="@\images\headshot.jpeg" alt="wedding image">
      </div>
    </div>
  
  <div class="home">

  </div>
</template>

<script>
export default {
};
</script>

<style scoped>
#page-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  margin: 0;
  padding: 0;
}

#card1 {

}
.card {
  display:grid;
  grid-template-columns: 1fr 1fr;
  grid-template-areas:
  "about1 card1-image"
  "about2 card1-image";
  background-color:rgba(245, 245, 220, 0.6);
  height: 40vh;
  width: 100%;
  margin-top: 20px;
  border-radius:  2%;
}
img {
  grid-area: card1-image;
  height: 35vh;
  width: auto;
  opacity: 0.85;
  border-radius:  10%;
}
#about1 {
  grid-area: about1;
}
#about2 {
  grid-area: about2;
}
</style>
