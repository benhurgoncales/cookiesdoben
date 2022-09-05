<template>
  <section class="section">
    <h1 class="title">Meu carrinho</h1>
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
          <tr>
            <td>Cookie de Baunilha</td>
            <td>
              <b-field>
                <b-numberinput
                  controls-position="compact"
                  controls-rounded
                ></b-numberinput>
              </b-field>
            </td>
            <td>R$3,00</td>
            <td>R$6,00</td>
          </tr>
          <tr>
            <td>Cookie de Chocolate</td>
            <td>
                <b-field>
                <b-numberinput
                  controls-position="compact"
                  controls-rounded
                ></b-numberinput>
              </b-field>
            </td>
            <td>R$3,00</td>
            <td>R$6,00</td>
          </tr>
          <tr>
            <td>Cookie de Doce de Leite</td>
            <td>
                <b-field>
                <b-numberinput
                  controls-position="compact"
                  controls-rounded
                ></b-numberinput>
              </b-field>

            </td>
            <td>R$5,00</td>
            <td>R$5,00</td>
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

    