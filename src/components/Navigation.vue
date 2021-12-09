<template>
   <div>
  <b-navbar class="text-center" toggleable="sm" type="light" variant="light">
    <b-navbar-toggle target="nav-text-collapse"></b-navbar-toggle>

    <b-navbar-brand></b-navbar-brand>

    <b-collapse id="nav-text-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item href="#about">Sobre mí</b-nav-item>
        <b-nav-item href="#projects">Proyectos</b-nav-item>
        <b-nav-item href="#skills">Skills</b-nav-item>
        <b-nav-item href="#contact">Contacto</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</div>

</template>

<style lang="css" scoped>
    *{
       padding:0;
       margin:0;
       box-sizing: border-box; 
    }
    
    .bg-light{
        background-image: linear-gradient(147deg, #FFE53B 0%, #ee7e33 74%)!important;
        
    }
    .navbar-expand-lg .navbar-nav{
      margin:0 auto;
    }

    .navbar-light .navbar-nav .nav-link{
       color:#000;
      font-size:19px;
    }

    @media (min-width: 768px) {
          li.nav-item{
            margin-left:5rem;
          }
          .navbar-light .navbar-nav .nav-link{
            color:#000;
            font-size:15px;
        }
     }
    @media (min-width: 1200px) {
    
      li.nav-item{
        margin-left:12rem;
      }
      .navbar-light .navbar-nav .nav-link{
            color:#000;
            font-size:17px;
        }
    }

</style>

