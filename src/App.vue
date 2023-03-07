<template>
  <div class="main">
    <div class="flayer">
      <div class="title">
        <h2>
          SEGUIMIENTO<br />
          ENVIOS
        </h2>
        <div class="content">
          <span class="super-polito">SUPER POLITO!</span>
          <div class="clip-path">
            <span>RÁPIDO Y SEGURO</span>
          </div>
          <div class="ul">
            <ul>
              <li><span class="li">ENVIO DE REGALOS DE CUMPLEAÑOS</span></li>
              <li><span class="li">1 x HIJA FAVORITA</span></li>
              <li><span class="li">1 x YERNO FAVORITO</span></li>
              <li><span class="li">1 x MATIAS</span></li>
            </ul>
          </div>
          <div class="blob">
            SU PRODUCTO SERA ENTREGADO EN MANOS DE SU FAMILIAR DIRECTO FAVORITO
            EL DIA: <br /><br />
            <span class="text-bold">DOMINGO 12-03/2023 EN HS DEL MEDIODIA</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Anton&family=Roboto:wght@400;700;900&display=swap");

html,
body {
  padding: 0;
  margin: 0;
}

* {
  box-sizing: border-box;
  font-family: "Roboto", sans-serif;
  color: #1e3044;
}

.main {
  width: 100%;
  height: 100vh;
  display: grid;
  place-content: center;

  background: url(./assets/img/roadblurred.jpg);
  background-size: cover;
  background-position: 50%;
}

.flayer {
  position: relative;

  width: 90vw;
  height: 90vh;

  padding: 2rem 0;

  background: url("./assets/img/roadandpolito.jpg");
  background-position: 50% 80%;
  background-size: cover;
  background-repeat: no-repeat;
}

.title {
  width: 100%;
  padding: 0 2rem;
  overflow-wrap: break-word;
}

h2 {
  font-size: 3.14rem;
  font-style: italic;
  font-family: Anton;
  margin: 0;
}

.content {
  display: flex;
  flex-direction: column;

  height: 100%;

  padding: 0 0 1rem 0;

  .super-polito {
    font-size: 2rem;
  }

  .clip-path {
    width: fit-content;
    clip-path: polygon(0% 0%, 90% 0%, 100% 50%, 90% 100%, 0% 100%);

    padding: 0.4rem 50px 0.4rem 0.8rem;
    background-color: #1e3044;
    span {
      color: white;
      font-size: 2rem;
      font-family: Anton;
      font-style: italic;
    }
  }

  .ul {
    margin: 1rem 0;
    background-color: #1e304488;
    border-radius: 25px;
    ul {
      list-style: none;
      li::before {
        content: "\2022";
        color: white;
        font-weight: bold;
        display: inline-block;
        width: 1em;
        margin-left: -1em;
      }
      li {
        span {
          color: white;
        }
      }
    }
  }

  .blob {
    position: absolute;
    bottom: 10px;
    right: 10px;
    text-align: center;
    width: 70%;
    height: 20%;
    padding: 2.2rem 3rem 5rem;
    background-color: rgb(255, 255, 255);
    border: 2px solid #1e3044;
    border-radius: 70% 30% 30% 70% / 60% 40% 60% 40%;
    box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.03),
      0px 0px 2px rgba(0, 0, 0, 0.06), 0px 2px 6px rgba(0, 0, 0, 0.12);
  }
}

.text-bold {
  font-weight: bold;
}

@media only screen and (min-width: 750px) {
  .flayer {
    width: 500px;
  }
}
</style>
