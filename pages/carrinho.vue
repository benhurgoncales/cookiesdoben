<template>
  <section class="section">
    <h1 class="title">Meu carrinho</h1>
    <h1 class="title">{{quantidade * parseInt(baunilha)}}</h1>

    <div>
      <table class="table is-striped is-hoverable is-fullwidth">
        <thead>
          <tr>
            <th>Produto</th>
            <th>
                Quantidade
            </th>
            <th>Preco Unidade</th>
            <th>Preco Total</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="produto in produtos" :key="produto.nome">
            <td>{{produto.nome}}</td>
            <td>
              <b-field>
                <b-numberinput v-model="produto.quantidade"
                  controls-position="compact"
                  controls-rounded 
                ></b-numberinput>
              </b-field>
            </td>
            <td>R$ {{produto.valor}}</td>
            <td>R$ {{produto.quantidade * produto.valor}}</td>
          </tr>
          
          
        </tbody>
      </table>
      <p class="subtitle is-3">Preco Total: R$17,00</p>
      <div class="buttons">
        <button class="button is-success is-large">Confirmar compra</button>
      </div>
    </div>
  </section>
</template>

<script>
  import { SourceMapSource } from 'webpack-sources';
  
  export default {
      data() {
          return { 
              baunilha: 3.00,
              chocolate: 3.00,
              doceleite: 5.00,
              quantidade1: 0,
              quantidade2: 0,
              produtos:[
                {
                  nome:"baunilha",
                  valor: 3.00,
                  quantidade: 1
                },
                {
                  nome:"chocolate",
                  valor: 3.00,
                  quantidade: 2
                },
                {
                  nome:"doceleite",
                  valor: 5.00,
                  quantidade: 2
                },
                
                {
                  nome:"doceleite",
                  valor: 5.00,
                  quantidade: 2
                }

              ]
              
          }
      },
      methods: {
        
      

      }
  }
  </script>