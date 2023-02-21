<script lang="ts">
    import FullMetalAlch from "./assets/fullmetal.gif"
    
    /* Arreglo para las cards de softskills */

    const skills = [
        {
            foto : "https://assets.stickpng.com/images/58582c01f034562c582205ff.png",
            title : "Trabajar en equipo / Comunicación",
            body : "Es más fácil en compañía y si están en sintonía es más fluido.",
            footer : '<a href="https://www.linkedin.com/in/daniel-michael-lugo-m-86b536256/"> Linked-in </a>'
        },
        {
            foto : "",
            title : "Deporte y actividad física",
            body : "",
            footer : ""
        },
        {
            foto : "",
            title : "Gatos y mascotas",
            body : "",
            footer : ""
        },
        {
            foto : "",
            title : "Redes sociales",
            body : "",
            footer : ""
        },
        {
            foto : "",
            title : "ENFP - T / Extrovertido",
            body : "",
            footer : ""
        },
    ];

</script>
<div class="container text-light ">
    <h3>Lo académico: </h3>
    <h5 class="fw-light"> 
        Egresado de la carrera de Sistemas de Información Administrativa (2022). <br>
        Licenciado de la carrera de Ciencias y Técnicas de la Comunicación (2012). <br>
        Maestro en Desarrollo Organizacional y Humano (2014). <br>
    </h5>
    <h3> Mis gustos: </h3>
    <h5 class="fw-light">
        
    </h5>
    <img src={FullMetalAlch} alt="" width="150">

    <!--Listado para softskills-->

    <div class="card-group">
    {#each skills as skill }
        <div class="card text-dark">
          <img src="{skill.foto}" class="card-img-top" alt="...">
          <div class="card-body">
            <h5 class="card-title">{skill.title}</h5>
            <p class="card-text">{skill.body}</p>
          </div>
          <div class="card-footer">
            <small class="text-muted">{@html skill.footer}</small>
          </div>
        </div>
        
    {/each}
    </div>



</div>