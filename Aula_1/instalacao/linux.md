
# Instalação do Linux Mint e Visual Studio Code

Neste artigo, vamos abordar a instalação do Linux Mint, uma distribuição baseada no Ubuntu, e o Visual Studio Code, um editor de código amplamente utilizado por desenvolvedores. A instalação do Linux Mint é o primeiro passo para configurar um ambiente de desenvolvimento no Linux, e o Visual Studio Code é uma ferramenta poderosa para escrever e depurar código.

# Requisitos Iniciais
Antes de começarmos, certifique-se de que você possui o seguinte:

- Um computador com hardware compatível.
- Um pendrive ou DVD em branco com pelo menos 4 GB de espaço para criar um disco de instalação do Linux Mint.
- Acesso à internet para baixar o Linux Mint.


# Instalação do Linux Mint
A instalação do Linux Mint é relativamente simples. Siga os passos abaixo:

- **Baixe o Linux Mint:** Acesse o site oficial do Linux Mint (https://linuxmint.com/) e escolha a versão adequada para o seu hardware. Geralmente, você deve escolher a versão de 64 bits.

- **Crie uma mídia de instalação:** Grave a imagem ISO que você baixou em um pendrive ou DVD usando um programa de gravação de disco.

- **Inicie a partir da mídia de instalação:** Insira a mídia de instalação no seu computador e inicie-o a partir dela. Isso geralmente requer a configuração da ordem de inicialização na BIOS ou UEFI do seu sistema.

- **Instale o Linux Mint:** Siga as instruções na tela para instalar o Linux Mint no seu computador. Você terá a opção de escolher a configuração de particionamento, criar senhas e configurar sua conta de usuário.

- **Atualize o sistema:** Após a instalação, é uma boa prática atualizar o sistema para garantir que você tenha as últimas atualizações de segurança e software. Abra um terminal e execute os seguintes comandos:

~~~ Terminal
sudo apt update
sudo apt upgrade
~~~

Agora, você tem o Linux Mint instalado no seu sistema e está pronto para configurar seu ambiente de desenvolvimento.


# Instalação do Visual Studio Code
O Visual Studio Code é um dos editores de código mais populares entre desenvolvedores. Para instalá-lo no Linux Mint, siga os passos abaixo:

- **Baixe o Visual Studio Code:** Abra um terminal e execute o seguinte comando para baixar o Visual Studio Code:

~~~
wget - O code.deb https://go.microsoft.com/fwlink/?LinkID=760868
~~~

- **Instale o Visual Studio Code:** Após o download, instale o pacote .deb usando o seguinte comando:
~~~
sudo dpkg - i code.deb
~~~

- **Resolva dependências:** Se você encontrar erros de dependências, execute o seguinte comando para corrigi-los:
~~~
sudo apt install - f
~~~

Agora você tem o Visual Studio Code instalado no seu sistema. Você pode iniciá-lo a partir do menu de aplicativos ou executando o comando code no terminal.

# Configuração Inicial
Após a instalação do Visual Studio Code, você pode personalizá-lo de acordo com suas preferências. Configure as extensões, temas e atalhos de teclado que melhor se adequam ao seu estilo de desenvolvimento.

Além disso, você pode configurar as extensões necessárias para suas linguagens de programação favoritas e ambientes de desenvolvimento.

# Conclusão
Neste artigo, exploramos o processo de instalação do Linux Mint, uma distribuição Linux amigável e baseada no Ubuntu, e do Visual Studio Code, um editor de código altamente funcional. Com essas ferramentas em mãos, você está pronto para iniciar seu desenvolvimento no ambiente Linux.

Lembre-se de que a personalização do ambiente de desenvolvimento é uma etapa importante para melhorar sua produtividade. Experimente diferentes configurações e extensões para encontrar o ambiente ideal para suas necessidades. Bons estudos e feliz programação!

# Link para aula:

[![youtube](../../img/capa_y.jpg)](https://youtu.be/X-B64ffRTW8)