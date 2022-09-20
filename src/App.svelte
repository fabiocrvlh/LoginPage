<script>
  let emailCerto = "fabio@fabio.com";
  let senhaCerta = "fabio123";
  let email = "";
  let senha = "";
  let validar = "";

  const validarAceito = () => {
    if (emailCerto === email && senhaCerta === senha) {
      validar = true;
      window.location.href = "https://marketbuy.vercel.app/";
    } else {
      validar = false;
      window.location.href = "https://error-login.vercel.app/";
    }
  };
</script>

<div
  class="h-screen  "
  style="background-image: url(https://www.pdvg.it/wp-content/uploads/2019/07/dying-light-2.jpg);"
>
  <div>
    <svg 
     xmlns="http://www.w3.org/2000/svg"
     
     fill="none" 
     viewBox="0 0 24 24" 
     stroke-width="1.5" 
     stroke="currentColor"
     class=" flex w-48 h-48 m-auto">
      <path stroke-linecap="round" stroke-linejoin="round" d="M17.982 18.725A7.488 7.488 0 0012 15.75a7.488 7.488 0 00-5.982 2.975m11.963 0a9 9 0 10-11.963 0m11.963 0A8.966 8.966 0 0112 21a8.966 8.966 0 01-5.982-2.275M15 9.75a3 3 0 11-6 0 3 3 0 016 0z" />
    </svg>
    
  </div>
  <div class="py-18 ">
    <div class=" bg-black bg-opacity-90 py-4  ">
      <div class=" flex flex-col items-center space-y-4 text-xl   ">
        <input
          bind:value={email}
          class="bg-blue-100  w-5/6  rounded-bl-xl rounded-tr-xl pl-3 outline-none hover:outline-red-500 lg:w-1/3 py-4 "
          type="text "
          placeholder="E-mail"
        />
        <input
          bind:value={senha}
          class="w-5/6 md:bg-blue-100  rounded-bl-xl rounded-tr-xl pl-3 outline-none hover:outline-red-500 lg:w-1/3 py-4"
          type="password"
          placeholder="Senha"
        />
      </div>
      <div class=" flex py-4 ">
        <button
          on:click={validarAceito}
          class="  ml-auto mr-2 bg-gray-500  py-4 px-10 text-white hover:bg-red-500 rounded-bl-xl rounded-tr-xl "
        >
          LOGAR
        </button>
        <button
          class="   mr-auto ml-2 bg-gray-500  py-4 px-3 text-white hover:bg-red-500 rounded-bl-xl rounded-tr-xl"
        >
          INSCREVER-SE
        </button>
      </div>
    </div>
  </div>

  <div class=" flex mt-36">
    <p class="text-white ml-2 mr-2  mt-48 ">
      DL.Connect é um serviço de distribuição digital, gerenciamento de direitos
      digitais, multijogador e comunicações desenvolvido pela DL.studious para
      fornecer uma experiência semelhante às conquistas / troféus oferecidos por
      várias outras empresas de jogos. O serviço é fornecido em várias
      plataformas.
    </p>
  </div>
</div>
