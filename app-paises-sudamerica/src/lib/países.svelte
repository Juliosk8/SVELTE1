<script>
  export let pais;
  let p;
  /*0=nombre_pais [1]=capital [2]=poblacion [3]=moneda [4]=area [5]=bandera*/
  const paises = {
    colombia: [
      "Colombia",
      "Bogota",
      "51,52 millones",
      "Peso colombiano",
      "1,142 millones km²",
      "colombia.jpeg",
    ],
    venezuela: [
      "Venezuela",
      "Caracas",
      "28,8 millones",
      "Bolivar",
      "916.445 km²",
      "venezuela.jpeg",
    ],
    ecuador: [
      "Ecuador",
      "Quito",
      "17,8 millones",
      "Dólar estadounidense",
      "256.370 km²",
      "ecuador.jpeg",
    ],
    peru: [
      "Peru",
      "Lima",
      "33,2 millones",
      "Sol peruano",
      "1.285.215 km²",
      "peru.jpeg",
    ],
    brasil: [
      "Brasil",
      "Brasilia",
      "214,3 millones",
      "Real brasileño",
      "8,51 millones km²",
      "brasil.jpeg",
    ],
    argentina: [
      "argentina",
      "Brasilia",
      "214,3 millones",
      "Real brasileño",
      "8,51 millones km²",
      "argentina.jpeg",
    ],
    chile: [
      "chile",
      "santiago de chile",
      "19.6 millones",
      "peso chileno",
      "756,626 km²",
      "chile.jpeg",
    ],
    paraguay: [
      "paraguay",
      "asuncion",
      "6.1 millones",
      "guaranies",
      "406,752 km²",
      "paraguay.jpeg",
    ],
    uruguay: [
      "uruguay",
      "montevideo",
      "3.423 millones",
      "peso uruguayo",
      "176,215 km²",
      "uruguay.jpeg",
    ],
    bolivia: [
      "bolivia",
      "sucre",
      "12.22 millones",
      "boliviano",
      "1.099 millones km²",
      "bolivia.jpeg",
    ],
  };
  p = paises[pais];
</script>

<div class="main">
  <div class="col1">
    <img
      src="/src/assets/{p[5]}"
      alt="Bandera_Colombia"
      width="300"
      height="200"
    />
  </div>
  <div class="col2">
    <div class="linea"><strong>Pais:</strong> {p[0]}</div>
    <div class="linea"><strong>Capital:</strong> {p[1]}</div>
    <div class="linea"><strong>Población:</strong> {p[2]}</div>
    <div class="linea"><strong>Moneda:</strong> {p[3]}</div>
    <div class="linea"><strong>Extensión:</strong> {p[4]}</div>
  </div>
</div>

<style>
  .main {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-gap: 5px;
    grid-auto-rows: minmax(100px, auto);
    border-radius: 10px;
    border-style: solid;
    border-color: rgb(186, 190, 182);
    border-width: 2px;
    margin-left: 600px;
    width: 700px;
    box-shadow: 0.5px 0.5px 0.5px black;
    margin-right: 5px;
    margin-bottom: 10px;
  }

  .col1 {
    grid-column: 1;
    grid-row: 1;
    margin: 5px;
    padding: 5px;
  }

  .col2 {
    grid-column: 2;
    grid-row: 1;
    margin: 5px;
    padding: 5px;
    border-color: black;
    width: max-content;
  }

  strong {
    color: blue;
    font-weight: bolder;
  }

  .linea {
    font-size: 20px;
    margin-bottom: 18px;
  }
</style>
