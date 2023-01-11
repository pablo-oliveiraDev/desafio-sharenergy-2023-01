###Instalação###

Recomendamos seguir estas instruções se você for novo no React e apenas estiver interessado em aprender. Se você estiver criando um aplicativo de página única (SPA) com o qual gostaria de usar comandos ou ferramentas Bash e/ou planeja implantar em um servidor Linux, recomendamos que você instale com create-react-app no Windows Subsystem for Linux (WSL).


Pré-requisitos
Instale a versão mais recente do Windows 10 (versão 1903+, build 18362+) ou Windows 11
Instale o Windows Subsystem for Linux (WSL), incluindo uma distribuição Linux (como o Ubuntu) e verifique se ele está sendo executado no modo WSL 2. Você pode verificar isso abrindo o PowerShell e digitando: wsl -l -v
Instale o Node.js no WSL 2: Estas instruções usam o Node Version Manager (nvm) para instalação, você precisará de uma versão recente do NodeJS para executar o create-react-app, bem como uma versão recente do Node Package Manager (npm). Para obter os requisitos exatos da versão, consulte o site Create React App.
Crie seu aplicativo React
Para instalar a cadeia de ferramentas React completa no WSL, recomendamos usar create-react-app:

Abra um terminal (Prompt de Comando do Windows ou PowerShell).

Crie uma nova pasta de projeto: mkdir ReactProjects e insira esse diretório: cd ReactProjects.

Instale o React usando create-react-app, uma ferramenta que instala todas as dependências para criar e executar um aplicativo React.js completo:

PowerShell

cópia de
npx create-react-app meu-aplicativo
  Observação

npx é o executor de pacotes usado pelo npm para executar pacotes no lugar de uma instalação global. Ele basicamente cria uma instalação temporária do React para que, a cada novo projeto, você esteja usando a versão mais recente do React (não qualquer versão atual quando você executou a instalação global acima). Usar o executor de pacotes NPX para executar um pacote também pode ajudar a reduzir a poluição causada pela instalação de muitos pacotes em sua máquina.

Isso primeiro pedirá sua permissão para instalar temporariamente o aplicativo create-react e seus pacotes associados. Depois de concluído, altere os diretórios para seu novo aplicativo ("meu-aplicativo" ou como você quiser chamá-lo): cd meu-aplicativo.

Inicie seu novo aplicativo React:

PowerShell

cópia de
npm start
Este comando iniciará o servidor Node.js e iniciará uma nova janela do navegador exibindo seu aplicativo. Você pode usar Ctrl + c para interromper a execução do aplicativo React em sua linha de comando.

  Observação

Create React App inclui um pipeline de construção de front-end usando Babel e webpack, mas não lida com lógica de back-end ou bancos de dados. Se você deseja criar um site renderizado pelo servidor com o React que usa um back-end Node.js, recomendamos a instalação do Next.js, em vez desta instalação do aplicativo create-react-app, que se destina mais a aplicativos de página única. Você também pode querer considerar a instalação do Gatsby se quiser construir um site estático orientado a conteúdo.

Quando você estiver pronto para implantar seu aplicativo da Web na produção, executar o npm run build criará um build do seu aplicativo na pasta "build". Você pode aprender mais no Guia do usuário do Create React App.

###LINK DO VIDEO####

##<https://youtu.be/TNBa4172sAg/>##