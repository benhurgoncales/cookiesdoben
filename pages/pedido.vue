<template>
  <section class="section">
    

    <div class="columns">
      <div class="column is-4">
  
      </div>
      
      <div class="column is-4">
        <form class="box">
        <h1 class="title"> Faça seu pedido </h1>
        
        <b-field label="Digite seu nome">
          <b-input v-model="name">nome</b-input>
        </b-field>

        <b-field label="Sabores">
          <b-select placeholder="Escolha seu sabor" icon="account">
            <optgroup label="Classicos">
              <option value="baunilha">baunilha</option>
              <option value="chocolate">chocolate</option>
            </optgroup>
            <optgroup label="Especiais">
              <option value="baunilha">Doce de Leite</option>
              <option value="chocolate">Nutella</option>
              <option value="chocolate">Red velvet </option>
            </optgroup>
          </b-select>
        </b-field>
        
        <b-field label="Quantiade de Cookies">
            <b-numberinput controls-rounded ></b-numberinput>
        </b-field>

        <b-field label="Hora para receber">
            <b-clockpicker
                rounded
                placeholder="Click to select..."
                icon="clock"
                :hour-format="format">
            </b-clockpicker>
        </b-field>

        <b-field label="Local que deseja receber">
          <b-input v-model="name">nome</b-input>
        </b-field>

        <div class="buttons">
           <button class="button is-success">Adicionar ao Carrinho</button>
        </div>

      </form>
      </div>

      
       <div class="column is-4">
  
      </div>
      

    </div>

  
    
  </section>
</template>