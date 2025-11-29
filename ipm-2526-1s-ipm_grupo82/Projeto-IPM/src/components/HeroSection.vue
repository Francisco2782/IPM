<template>
  <div class="hero">
    <div class="overlay"></div>
    <div class="hero-content">
      <h1>Dados e defesa sobre o impacto do Airbnb nas comunidades residenciais</h1>
      <p>Exploramos dados transparentes sobre listagens Airbnb e o seu impacto nas cidades em todo o mundo</p>
    </div>
  </div>
</template>

<style>
.hero {
  position: relative;
  height: 350px;
  background-image: url('/src/assets/herosection1.png'); 
  background-size: cover;
  background-position: center;
  display: flex;
  justify-content: center;
  align-items: center;
}

.overlay {
  position: absolute;
  inset: 0;
  background: linear-gradient(to bottom, rgba(0,0,0,0.3), rgba(255,255,255,1));
}

.hero-content {
  position: relative;
  text-align: center;
  color: white;
  max-width: 700px;
  padding: 20px;
}
</style>
