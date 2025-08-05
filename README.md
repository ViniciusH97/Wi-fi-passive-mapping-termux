# WI-FI Passive Mapping Termux

## Objetivo

Realizar o mapeamento de APs(Access Points) com o uso de ferramenta mobile sem a necessidade de root. 

Antes de iniciar o mapeamento e utilizar as ferramentas, é necessário ter conhecimento prévio do terminal shell, para que possamos manipular arquivos e navegar nas pastas onde serão armazenados os scripts e resultados.

## Emulador de Terminal para Android

O aplicativo essencial para esse mapeamennto será o Termux.

<img width="100" height="100" alt="4dca8e0edabe9ede" src="https://github.com/user-attachments/assets/7422dde9-5a28-4ac0-b6f3-288f5eeb0f97" />

## O que é o Termux?
O Termux é um aplicativo que simula o terminal shell no smartphone Android, ele pode ser baixado tanto na PlayStore quanto via F-Droid. Porém, como vamos utilizar o Termux para realizar um mapeamento de rede utilizando a interface WI-FI e GPS, será necessário realizar o download do Termux:API. O Termux:API é um add-on, ele permite que scripts ou comandos executados no Termux interajam com as funcionalidades do Android, como por exemplo: GPS, câmera, chamadas, SMS, brilho da tela, entre outros. 

### Como instalar o Termux?

Para instalar a última versão do Termux no seu smartphone, é recomendado instalar pela plataforma de aplicativos chamada de F-Droid. A versão disponível na loja da Google (Google Play Store) geralmente são disponibilizadas versões antigas que não possuem o suporte adequado para o Termux:API. Nesse caso, vamos baixar o F-Droid em seu site oficial clicando [aqui](https://f-droid.org/).

1. Instale o apk do aplicativo F-Droid, e abra-o. Você verá um ícone de uma lupa verde, clique nela e abrirá a tela de pesquisa de apps. Digite Termux, selecione e pressione instalar.

![IMG_20250804_210157](https://github.com/user-attachments/assets/88db82f6-07f2-4d6e-b668-b82109826e48)

2. Após instalar o Termux, é recomendado que inicie pela primeira vez, para que seja aceito as permissões mínimas.

3. Em seguida, abra o F-Droid novamente, clique na lupa verde, e pesquise: Termux API, e instale também.

![IMG_20250804_211503](https://github.com/user-attachments/assets/88f312b5-7f90-4f5d-aece-645057b49a9f)

Desabilite as opções recomendadas e feche.

4. Abra o Termux e instale o pacote Termux:API, digite o comando abaixo:

```bash
pkg install termux-api
```

5. Nesse momento, inicie o Termux e atualize as listas de pacotes com `pkg update`, e atualize os pacotes com `pkg upgrade`.

Agora seu Termux está atualizado e pronto para utilizar as ferramentas necessárias para o mapeamento utilizando as funcionalidade do Android com o Termux:API. Para testar se realmente o Termux:API está instalado e funcionando corretamente, habilite o wifi e a localização do seu smartphone e rode o comando no terminal:

```bash
termux-location
```

> OBS: Não esqueça de habilitar o GPS e o wi-fi do smartphone para realziar os testes

A saída será algo parecido com isso:

![Termux2](https://github.com/user-attachments/assets/1c99be24-4ec6-4d16-94e1-daadc960f2d2)

Se aparecer as coordenadas como na imagem acima, significa que o Termux:API funcionou corretamente.E agora poderá testar o comando para escaneamento de APs:

```bash
termux-wifi-scaninfo
```

A saída será algo como:

![Termux1](https://github.com/user-attachments/assets/77fe28df-2caf-425e-8561-ebc571c166d2)

