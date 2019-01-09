# Dropbox Clone com Firebase
Projeto de apresentação tecnica demonstrando habilidades e manuseio com tecnologia javascript.

## Tecnologias
Javascript Vanilla / Firebase Database / Firebase Storage

## Requisitos
Para funcionamento completo do projeto é necessario ter o node com os gerenciadores de pacote bower e npm instalados na maquina.

## Configuração do projeto
1. Com o node e demais gerenciadores de pacotes instalados dê um bower install na raiz deste projeto e aguarde as dependencias serem adicionadas.

**OBS:** Recomenda-se o uso de um pacote global como o browser-sync para gerir um servidor web basico caso não exista um na maquina.

## Configuração do firebase
1. Para funcionamento completo do sistema é necessario ter uma conta no firebase.
2. Com a conta e um projeto criado busque no item de configurações do projeto o item "Adicionar o firebase a seu aplicativo da web"

Será exibido um script que deve ser configurado dentro deste projeto.
```
<script src="https://www.gstatic.com/firebasejs/5.7.2/firebase.js"></script>

<script>
  // Initialize Firebase
  var config = {
    apiKey: "***************************************",
    authDomain: "app.firebaseapp.com",
    databaseURL: "https://app.firebaseio.com",
    projectId: "dropbox-clone",
    storageBucket: "dropbox-clone.appspot.com",
    messagingSenderId: "309997021757"
  };
  firebase.initializeApp(config);
</script>
```
3. Dentro do caminho: 'src/controllers/DropboxController.js' busque pela função 'connectFirebase()' e altere a função com o bloco que o firebase lhe forneceu:

```
connectFirebase() {
  var config = {
    apiKey: "***************************************",
    authDomain: "app.firebaseapp.com",
    databaseURL: "https://app.firebaseio.com",
    projectId: "dropbox-clone",
    storageBucket: "dropbox-clone.appspot.com",
    messagingSenderId: "309997021757"
  };
  
  firebase.initializeApp(config);
}
```

**OSB:** Para fucionamento correto você deve editar o metodo acima com os dados fornecidos pelo firebase no local dito no passo 2.

4. Com tudo configurado rode um servidor web e terá o clone funcional.

## Considerações finais.
1. Este projeto tem o unico intuito de apresentar habilidades de uso com tecnologia javascript
e compor o portifolio do autor em questão.
2. Todo corpo HTML foi extraido de um template já pré definido.
