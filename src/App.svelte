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
  style="background-image: url(https://w7.pngwing.com/pngs/511/894/png-transparent-dying-light-the-following-playstation-4-video-game-xbox-one-minecraft-game-text-graphic.png);"
>
  <div>
    <img
      src="https://dl2.dyinglightgame.com/static/logo-big-798e6541ff2a742cfb7bdd40b7b1ad06.svg"
      alt="logo"
      class="flex ml-auto mr-auto w-90 h-70 mb-10"
    />
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
