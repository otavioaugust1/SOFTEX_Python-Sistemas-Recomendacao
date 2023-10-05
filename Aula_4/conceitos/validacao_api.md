
# Utilizando o Postman para Explorar e Validar APIs

## Introdução ao Postman
O Postman é uma plataforma essencial para desenvolvedores que oferece uma variedade de ferramentas e recursos para atender às necessidades de desenvolvedores. Neste artigo, vamos explorar como usar o Postman para interagir com APIs públicas e utilizar métodos HTTP para acessar e validar essas APIs.

## Acessando o Postman
Para começar, acesse o site oficial do Postman em postman.com(https://www.postman.com). Você pode baixar a versão desktop ou utilizar a versão online. Para utilizar a versão online, é necessário fazer um cadastro gratuito.

## Criando um Novo Workspace
Após fazer o login, você será redirecionado para o seu workspace. Aqui, você pode criar coleções para organizar suas requisições. Vamos criar uma coleção chamada \"Curso Postman\" para este exemplo.

## Explorando Métodos HTTP
O Postman nos permite utilizar os métodos HTTP, como GET, POST, PUT e DELETE, para fazer requisições a APIs. Vamos começar com um exemplo simples usando o método GET.

## Exemplo com Via CEP
Suponha que você queira obter informações de um CEP específico. Utilizaremos a API Via CEP para isso. O endpoint da API é `https://viacep.com.br/ws/{CEP}/json/`.

1. Crie uma nova requisição no Postman e selecione o método GET.
2. Insira o endpoint da API, substituindo `{CEP}` pelo CEP desejado, por exemplo, `https://viacep.com.br/ws/77001090/json/`.
3. Envie a requisição e observe a resposta contendo informações relacionadas ao CEP, como logradouro, bairro e cidade.

## Utilizando Variáveis
Uma funcionalidade útil do Postman é a capacidade de usar variáveis. Isso permite que você torne suas requisições mais dinâmicas. Por exemplo, você pode criar uma variável chamada `CEP` e definir seu valor como o CEP desejado. Em seguida, utilize essa variável no endpoint da API. Dessa forma, você pode reutilizar a mesma requisição com diferentes CEPs.

## Explorando a API do Pokémon
Vamos explorar outra API divertida, a API do Pokémon. Você pode obter informações sobre Pokémon específicos, como suas habilidades e características.

1. Crie uma nova requisição no Postman, selecione o método GET e utilize o endpoint da API do Pokémon, por exemplo, `https://pokeapi.co/api/v2/pokemon/pikachu/`.
2. Envie a requisição e observe a resposta contendo informações sobre o Pokémon Pikachu.

## Previsão do Tempo com o INPE
A API do Instituto Nacional de Pesquisas Espaciais (INPE) oferece informações sobre a previsão do tempo. Vamos utilizar essa API para obter a previsão do tempo para diferentes cidades.

1. Crie uma nova requisição no Postman, selecione o método GET e utilize o endpoint da API do INPE para listar cidades: `http://servicos.cptec.inpe.br/XML/listaCidades`.
2. Envie a requisição e observe a lista de cidades retornadas.
3. Escolha uma cidade, por exemplo, Palmas, e crie uma nova requisição utilizando o endpoint da previsão do tempo: `http://servicos.cptec.inpe.br/XML/cidade/236/previsao.xml`. Substitua o código da cidade pelo código da cidade desejada.
4. Envie a requisição e obtenha a previsão do tempo para a cidade selecionada.

## Documentação da API
É importante observar que a maioria das APIs possui documentação detalhada que descreve os endpoints disponíveis, os parâmetros necessários e exemplos de uso. Sempre consulte a documentação da API que você está utilizando para obter informações precisas sobre como fazer as requisições.

## Conclusão
O Postman é uma ferramenta poderosa para explorar, validar e testar APIs de forma eficiente. Neste artigo, demonstramos como realizar requisições GET e como utilizar variáveis para tornar suas requisições dinâmicas. Além disso, exploramos exemplos de APIs, como a Via CEP, a API do Pokémon e a API do INPE. A partir desses exemplos, você pode expandir suas habilidades e criar integrações mais avançadas em suas aplicações.

Lembre-se sempre de consultar a documentação da API que você está utilizando para obter informações detalhadas sobre como fazer as requisições e aproveitar ao máximo os recursos disponíveis.