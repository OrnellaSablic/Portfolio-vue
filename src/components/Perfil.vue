<template>
    <div>
        <section class="section">
            <div class="container-fliud">
                <img :src="require('@/assets/img/photo.jpg')" alt="foto-de-perfil" class="rounded-circle">
                <div class="name-text">
                    <h1> {{nombre }}</h1>
                    <h2>{{ profesion}}</h2>
                </div>
            </div>
        </section>
    </div>
</template>


<script>
  export default {
    name: 'perfil',
    data() {
      return {
        nombre: 'Ornella Sablic',
        profesion: 'Frontend Developer',
      };
    },
  };
</script>

<style lang="css" scoped>
    .section{
        padding-top: 70px;
        padding-bottom: 25px;
        background-image: url('../assets/img/background.png');
    }
    .name-text{
        margin-top: 25px;
    }
    .rounded-circle{
        max-width:40%;
    }
    
    @media (min-width: 768px) { 
         .rounded-circle{
            max-width:30%;
        }
     }
    @media (min-width: 1200px) {
        .rounded-circle{
            max-width:20%;
        }
    }
</style>