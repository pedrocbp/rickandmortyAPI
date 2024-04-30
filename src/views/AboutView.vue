<template>
  <center>
    <div class="template">
      <div class="card" style="width: 100%; height: 100vh;">
        <img class="card-img-top" src="/src/assets/images/devicon.png" alt="Card image cap">
        <div class="card-body">
          <div class="name">Pedro Miguel Bonini de Cerqueira</div>
          <div class="course">Análise e Desenvolvimento de Sistemas</div>
          <p class="card-text">19 anos, técnico em eletroeletrônica e estudante de Análise e Desenvolvimento de Sistemas na Unimar</p>
          <a href="mailto:pedromiguelboce@gmail.com">pedromiguelboce@gmail.com</a><br>
          <a href="https://github.com/pedrocbp"><i class="bi bi-github"></i></a>
          <a href="https://www.linkedin.com/in/pedro-bonini-0b0446229/"><i class="bi bi-linkedin"></i></a>
        </div>
      </div>
    </div>
  </center>
  
</template>

<style scoped>

  .bi {
    margin: 5px;
  }

  .card{
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #212529;
    color: #c9c6c6;
    font-size: 20px;
  }

  .card-img-top {
    padding-top:  10px;
    width: 30%;
    height: auto
  }
  .name {
    font-size: 25px;
    color: #fff;
  }

  .course {
    font-size: 20px;
    color: #666;
  }
</style>
