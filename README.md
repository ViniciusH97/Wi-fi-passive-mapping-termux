# WI-FI Passive Mapping Termux

## Objetivo

Realizar o mapeamento de APs utilizando ferramentas sem root. Para comerçarmos o mapeameno e ir direto para a ferramentas, precisamos ter o conhecimento prévio do terminal shell, para que possamos manipular arquivos e navegar nas pastas que vamos armazenar o script e os resultados dos mapeamentos.

## Ferramentas

O aplicativo essencial para esse mapeamennto será o Termux. 

### O que é o Termux?
O Termux é um aplicativo que simula o terminal shell no seu smartphone, ele pode ser baixado tanto na PlayStore quanto na AppleStore. Porém como vamos utilizar o Termux para realizar um mapeamento de rede utilizando a interface WI-FI e GPS, será necessário realizar o download do Termux:API. O Termux:API é um add-on, ele permite que scripts ou comandos executados no Termux interajam com as funcionalidades do Android, como por exemplo: GPS, câmera, chamadas, SMS, brilho da tela, entre outros. 

### Como instalar o Termux?

Para instalar a última versão do Termux no seu smartphone, é recomendado instalar pela plataforma de aplicativos chamada de F-Droid. A versão disponível na loja da Google (Google Play Store) geralmente sçao versão antigas que não possuem o suporte adequado para o Termux:API. Nesse caso, vamos baixar o F-Droid em seu site oficial clicando [aqui](https://f-droid.org/).

1. Instale o apk do aplicativo F-Droid, e abra-o. Você verá um ícone de uma lupa verde, clique nela e abrirá a tela de pesquisa de apps. Digite Termux, selecione e pressione instalar.

[print da tela do f-droid]

2. Após instalar o Termux, é recomendado que inicie pela primeira vez, para que seja aceito as permissões mínimas.

[print da tela do termux iniciado pela primeira vez]

4. Em seguida, abra o F-Droid novamente, clique na lupa verde, e pesquise: Termux API, e instale também.

[print da tela do termux api]

Desabilite as opções recomendadas e feche.

5. Nesse momento, inicie o Termux e atualize as listas de pacotes com `pkg update`, e atualize os pacotes com `pkg upgrade`.

Agora seu Termux está atualiza e pronto para utilizar as ferramentas necessárias para o mapeamento utilizando as funcionalidade do Android com o Termux:API. Para testar se realmente o Termux:API está instalado e funcionando corretamente, habilite o wifi e a localização do seu smartphone e rode o comando no terminal:

```bash
termus-location
```

A saída será algo parecido com isso:

[print da tela com a saída do termux-location]
