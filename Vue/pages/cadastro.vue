<template>

   <main>
         <Menu />

      <div id="modal" class="animar">

                <h1>Cadastro</h1><br><br>
                <input id="field1" type="text" placeholder="Nome"> <br> <br>

                <input id="field2" type="text" placeholder="Sobrenome"> <br> <br>

                <input id="field3" type="email" placeholder="E-mail"><br> <br>

                <input id="field4" type="email" placeholder="E-mail"><br> <br>

                <input id="field5" type="password" placeholder="password"><br> <br>

                <input id="field6" type="password" placeholder="password"><br> <br>

                <input id="field7" type="number" placeholder="Celular"><br> <br>

                <input id="field8" type="rg" placeholder="RG"><br> <br>

                <input id="field9" type="cpf" placeholder="CPF"><br> <br>

                <input id="field10" type="date" placeholder="Data de Nascimento"><br> <br>

                <input id="field11" type="endereco" placeholder="Endereço"><br> <br>

                <input id="field12" type="complemento" placeholder="Complemento"><br> <br>

                <input id="field13" type="Logadouro" placeholder="Logadouro"><br> <br>

                <button>Cadastrar</button>

            </div>

         <Footer />
            </main>
</template>



<style scoped>
body{
  background: #f7f7f7;
  margin:20px;
}

#ativar{
  display:block;
  margin:20px auto;
}

#load{
  width:20px;
  height:20px;
  border:10px solid;
  border-radius: 50%;
  border-top-color: transparent;
  margin: 0 auto;
  color:rgb(236, 195, 10);
  animation: load .6s linear infinite;
}

@keyframes load {
  to {
    transform: rotate(360deg);
  }
}

#modal h1{
  font-family: sans-serif;
  margin: 0px 0 0px 20px;
}

#modal label{
  display: block;
  font-family: sans-serif;
  margin-bottom: 5px;
  margin-top: 10px;
}

#modal input{
  width:100%;
  border:1px solid #ddd;
  border-radius: 4px;
  padding: .5rem;
  font-size: 1rem;
  background: #f7f7f7;


}

#modal button{
  margin-top: 20px;
  display:block;
  font-family: sans-serif;
  font-size: 1rem;
  padding: .6rem 2rem;
  border: none;
  background: rgb(236, 195, 10);
  color:black;
}

#modal.animar{
  /*animation-name:slide;
  animation-duration: .3s;
  animation-fill-mode: forwards;
  animation-timing-function: ease;
  animation-delay: 0s;
  animation-iteration-count: 1;
  animation-direction:normal ;
  animation-fill-mode:forwards ;
  animation-play-state:running ;*/
  animation: slide .3s  forwards;



}

@keyframes slide{
  from{
    opacity: 0;
  }
  to{
    transform: translatex(0);
    opacity: 1;
  }
}
#modal{
  padding:30px;
  background:white;
  border-radius: 4px;
  box-shadow: 0 1px 1px rgba(0,0,0.1);
  max-width: 400px;
  margin:20px auto;
  opacity:0;
  transform:translatex(-20px);
}


</style>
