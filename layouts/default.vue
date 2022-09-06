<template>
  <div class="container is-fluid" >

    <b-navbar shadow="true" style="height:90px">
        <template #brand>
            <b-navbar-item tag="router-link" :to="{ path: '/' }">
                <img style="max-height:90px"
                    src="https://github.com/benhurgoncales/cookiesdoben/blob/master/assets/Cookies.png?raw=true"
                    alt="Lightweight UI components for Vue.js based on Bulma"
                >
            </b-navbar-item>
        </template>
        <template #start>
          
            <b-navbar-item tag="router-link" :to="{ path: '/' }">
                Home
            </b-navbar-item>

          
            <b-navbar-item tag="router-link" :to="{ path: '/produto' }">
                Produto
            </b-navbar-item>

          
          <b-navbar-item tag="router-link" :to="{ path: '/lista' }">
                lista
            </b-navbar-item>

          <b-navbar-item tag="router-link" :to="{ path: '/pedido' }">
               Faça seu pedido
            </b-navbar-item>

            <b-navbar-item tag="router-link" :to="{ path: '/carrinho' }">
               Carrinho
            </b-navbar-item>

        </template>

        <template #end>
            <b-navbar-item tag="div">
                <div class="buttons">
                    <a class="button is-dark" href="/cadastro">
                        <strong>Cadastre-se</strong>
                    </a>
                    <a class="button is-light" href="/login">
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

