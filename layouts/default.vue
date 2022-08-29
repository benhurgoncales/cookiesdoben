<template>
  <div class="container is-fluid" >

    <b-navbar shadow="true" >
        <template #brand>
            <b-navbar-item tag="router-link" :to="{ path: '/' }">
                <img
                    src="https://github.com/benhurgoncales/cookiesdoben/blob/master/assets/Cookies.png?raw=true"
                    alt="Lightweight UI components for Vue.js based on Bulma"
                >
            </b-navbar-item>
        </template>
        <template #start>
          
            <b-navbar-item tag="router-link" :to="{ path: '/' }">
                Home
            </b-navbar-item>

          
            <b-navbar-item tag="router-link" :to="{ path: '/sabores' }">
                Sabores
            </b-navbar-item>

          
          <b-navbar-item tag="router-link" :to="{ path: '/lista' }">
                lista
            </b-navbar-item>

          
          <b-navbar-item tag="router-link" :to="{ path: '/endereços' }">
                endereços
            </b-navbar-item>

          <b-navbar-item tag="router-link" :to="{ path: '/pedido' }">
               Faça seu pedido
            </b-navbar-item>
        </template>

        <template #end>
            <b-navbar-item tag="div">
                <div class="buttons">
                    <a class="button is-primary">
                        <strong>Cadastre-se</strong>
                    </a>
                    <a class="button is-light">
                        Login
                    </a>
                </div>
            </b-navbar-item>
        </template>
    </b-navbar>

    <Nuxt/>

    <footer class="footer">
      <div class="content has-text-centered">
        <p>
          <strong>Cookies do Ben</strong> by Ben-Hur. 
          <a target="_blank" href="https://fae.edu">FAE Centro Universitário</a>
        </p>
      </div>
    </footer>      
    
  </div>
</template>

