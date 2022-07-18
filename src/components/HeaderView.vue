<template>

    <b-navbar class="p-3" style="display: flex; justify-content:space-between; width:100%; " toggleable="lg" type="dark" variant="info">
     
        <b-navbar-brand href="#" >Cursos <font color="black">de</font> Programação</b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" class="menuLateral" is-nav>
          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <!-- <b-nav-item to="/">Home</b-nav-item> -->
            <b-nav-item to="/about">About</b-nav-item>
          </b-navbar-nav>
        </b-collapse>
      
    </b-navbar>
 
</template>

<style>
.menuLateral{
  display: flex;
  justify-content: flex-end !important;
}

@media screen and (max-width: 992px) {
  .menuLateral{
    justify-content: flex-end !important;
  }
}


</style>