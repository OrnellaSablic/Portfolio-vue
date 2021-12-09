<template>
    <div>
        <section class="section-about">
            <div class="row p-5 justify-content-evenly text-start">
                <div class="col col-md-8 col-lg-4">
                    <h5 id="about" class="text-uppercase"><strong>Sobre mí</strong></h5>
                    <b-card-text>
                        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Fuga reprehenderit aliquam facilis placeat quos cum nihil voluptas eveniet aperiam blanditiis? Neque ratione temporibus, minus debitis esse animi omnis voluptatum sapiente.
                    </b-card-text>
                </div>
                <div class="col-md-4 col-lg-4 datos">
                    <h5 id="about" class="text-uppercase"><strong>Datos personales</strong></h5>
                    <b-card-text>
                        <p><strong>Email:</strong> {{ about.email }}</p>
                        <p><strong>Teléfono:</strong> {{ about.teléfono }}</p>
                        <p><strong>Ciudad:</strong> {{ about.ciudad }}</p>
                    </b-card-text>
                </div>
            </div>
        </section>
    </div>
    
</template>


<script>
const defaultAbout = {
  email: 'correo@gmail.com',
  teléfono: '+33 6 51 99 80 78',
  ciudad: 'Rosario, Santa Fe'
};

export default {
  name: 'about',
  props: {
    about: {
      type: Object,
      default() {
        return defaultAbout;
      },
    },
  },
};
</script>

<style>
 
@media (min-width: 480px) {
    .datos{
        margin-top:2rem;
    }         
}


</style>