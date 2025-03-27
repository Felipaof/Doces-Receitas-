<h1 align="center">  </h1>
<p align="center">Trabalho para a disciplina de DESENVOLVIMENTO DE APLICAÇÕES PARA DISPOSITIVOS MÓVEIS - 4º Informática do IFSP-Jacareí</p>
<br>
<p align="center">
<img loading="lazy" src="http://img.shields.io/static/v1?label=STATUS&message=%20DESENVOLVIDO&color=GREEN&style=for-the-badge"/>

<h1>🧑‍🏫 Professor responsável</h1> 

-  Carlos Eduardo Duque Polito

<h1>🎯 Objetivo do projeto</h1> 

O objetivo deste trabalho é a realização de um aplicativo de dispositivos móveis, que ensinará a realização de algumas receitas doces especifícas.  
<br>

<h1>✖️ O que não é o objetivo do projeto</h1>

Por se tartar de um trabalho em pequena escala, somente com fim de conhecimentos, o aplicativo não contará com:
- Salvamento de receitas favoritas.
- Se caso realizado a receita, não terá responsabilidade sobre o doce realizado pelo usuário. 

<h1>👥 Público-alvo</h2>

<h1>:hammer: Requisitos funcionais do projeto</h1>

-Sistema de buscas de categorias de receitas contidas no app (Exemplo: "Bolo")

-Sistema de buscas de receitas contidas no app por categoria (Exemplo: "Bolo de cenoura")

-Um link de um vídeo de apoio para auxiliar no desenvolvimento da receita.

<h1>☑️ Requisitos não funcionais para o site</h1> 

-Desempenho: O aplicativo deverá funcionar com agilidade no tempo de resposta e sem travamento nas buscas.

-Segurança: O aplicativo não irá precisar de nenhum dado do usuário para sua utilização.

<h1>📑 Matrizes de Requisitos</h1>

<h2>Matriz de Requisitos Gerais</h2>

<img src="https://github.com/Felipaof/Doces-Receitas-/blob/167fc5b0dfa91bc94cbe2186cadd42c09a0f090a/Matriz%20de%20requisitos%20.png" width=1000> 
<br>

<h1>📱Mockup do APP </h1>

<h2> Pré-Mockup da Interface principal:</h2> <img src="https://github.com/Felipaof/Doces-Receitas-/blob/b0264919eac15226bcf6214283dff328145e19a3/Mockup%20inicial%20.png" width=1000> 

<h2> Pré-Mockup da Interface de busca:</h2> <img  src="https://github.com/Felipaof/Doces-Receitas-/blob/b0264919eac15226bcf6214283dff328145e19a3/tela%20pesquisa.png" width=1000> 

<h2> Pré-Mockup da Interface das receitas:</h2> <img  src="https://github.com/Felipaof/Doces-Receitas-/blob/b0264919eac15226bcf6214283dff328145e19a3/tela%20receitas%20.png" width=1000> 

<h2> Pré-Mockup da Interface da receita:</h2> <img  src="https://github.com/Felipaof/Doces-Receitas-/blob/b0264919eac15226bcf6214283dff328145e19a3/tela%20receita%20.png" width=1000> 

<h1>📊 Modelagem do Banco de Dados</h1>
<img src="https://github.com/Felipaof/Doces-Receitas-/blob/167fc5b0dfa91bc94cbe2186cadd42c09a0f090a/Diagrama%20banco%20de%20dados%20.png" width=1000>


<h1>📖 Dicionário de dados </h1> 

<h2>Entidade Categorias</h2>
Essa entidade é responsável por armazenar as categorias de receitas disponíveis no sistema, como bolos, tortas e sorvetes.
<br><br>

- `idCategorias`: É um atributo do tipo INT. É o responsável por criar um **Id único** para cada categoria (**CHAVE PRIMÁRIA**).
- `Bolos`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Representa a categoria de bolos.
- `Tortas`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Representa a categoria de tortas.
- `Sorvetes`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Representa a categoria de sorvetes.

<h2>Entidade Bolos</h2>
Essa entidade é responsável por armazenar diferentes tipos de bolos cadastrados no sistema.
<br><br>

- `idBolos`: É um atributo do tipo INT. É o responsável por criar um **Id único** para cada bolo (**CHAVE PRIMÁRIA**).
- `Bolo de cenoura`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Armazena o nome do bolo de cenoura.
- `Bolo de chocolate`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Armazena o nome do bolo de chocolate.
- `Bolo de banana`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Armazena o nome do bolo de banana.
- `Receita do bolo_idReceita`: É um atributo do tipo INT. Representa a relação entre a tabela de bolos e a tabela de receitas dos bolos (**CHAVE ESTRANGEIRA**).

<h2>Entidade Receita dos Bolos</h2>
Essa entidade é responsável por armazenar as receitas específicas dos bolos cadastrados.
<br><br>

- `idReceitaBolos`: É um atributo do tipo INT. É o responsável por criar um **Id único** para cada receita de bolo (**CHAVE PRIMÁRIA**).
- `Receita bolo de cenoura`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Armazena a receita do bolo de cenoura.
- `Receita bolo de chocolate`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Armazena a receita do bolo de chocolate.
- `Receita bolo de banana`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Armazena a receita do bolo de banana.

<h2>Entidade Tortas</h2>
Essa entidade é responsável por armazenar diferentes tipos de tortas cadastradas no sistema.
<br><br>

- `idTortas`: É um atributo do tipo INT. É o responsável por criar um **Id único** para cada torta (**CHAVE PRIMÁRIA**).
- `Torta holandesa`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Armazena o nome da torta holandesa.
- `Torta de maracujá`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Armazena o nome da torta de maracujá.
- `Torta de limão`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Armazena o nome da torta de limão.
- `Receita da torta_idReceita`: É um atributo do tipo INT. Representa a relação entre a tabela de tortas e a tabela de receitas das tortas (**CHAVE ESTRANGEIRA**).

<h2>Entidade Receita das Tortas</h2>
Essa entidade é responsável por armazenar as receitas específicas das tortas cadastradas.
<br><br>

- `idReceitaTortas`: É um atributo do tipo INT. É o responsável por criar um **Id único** para cada receita de torta (**CHAVE PRIMÁRIA**).
- `Receita torta holandesa`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Armazena a receita da torta holandesa.
- `Receita torta de maracujá`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Armazena a receita da torta de maracujá.
- `Receita torta de limão`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Armazena a receita da torta de limão.

<h2>Entidade Sorvetes</h2>
Essa entidade é responsável por armazenar diferentes tipos de sorvetes cadastrados no sistema.
<br><br>

- `idSorvetes`: É um atributo do tipo INT. É o responsável por criar um **Id único** para cada sorvete (**CHAVE PRIMÁRIA**).
- `Sorvete de baunilha`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Armazena o nome do sorvete de baunilha.
- `Sorvete de chocolate`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Armazena o nome do sorvete de chocolate.
- `Sorvete de morango`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Armazena o nome do sorvete de morango.
- `Receitas dos sorvetes_idReceita`: É um atributo do tipo INT. Representa a relação entre a tabela de sorvetes e a tabela de receitas dos sorvetes (**CHAVE ESTRANGEIRA**).

<h2>Entidade Receita dos Sorvetes</h2>
Essa entidade é responsável por armazenar as receitas específicas dos sorvetes cadastrados.
<br><br>

- `idReceitaSorvetes`: É um atributo do tipo INT. É o responsável por criar um **Id único** para cada receita de sorvete (**CHAVE PRIMÁRIA**).
- `Receita sorvete de baunilha`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Armazena a receita do sorvete de baunilha.
- `Receita sorvete de chocolate`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Armazena a receita do sorvete de chocolate.
- `Receita sorvete de morango`: É um atributo do tipo VARCHAR com um tamanho de 45 caracteres. Armazena a receita do sorvete de morango.

<h1>🧍Diagramas UML</h1>
<h2>Tela de principal e funcionamento do aplicativo</h2>
<img src="https://github.com/Felipaof/Doces-Receitas-/blob/167fc5b0dfa91bc94cbe2186cadd42c09a0f090a/Diagrama%20UML%20doces%20receitas%20.png" width=1000>

<h1>🧰 Tecnologias Utilizadas</h1> 

back-end:

<img src="https://img.shields.io/badge/Android Studio-%2300C4CC.svg?style=for-the-badge&logo=Android Studio&logoColor=white">

Front-end:
<br><br>
<img src="https://img.shields.io/badge/React Native-%23323330.svg?style=for-the-badge&logo=ReactNative&logoColor=white">

Banco de Dados:
<br><br>
<img src="https://img.shields.io/badge/supabase-%2300C4B7.svg?style=for-the-badge&logo=supabase&logoColor=white">
<img src="https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white">

Diagramas e Mockups:
<br><br>
<img src="https://img.shields.io/badge/Canva-%2300C4CC.svg?style=for-the-badge&logo=canva&logoColor=white">
<img src="https://img.shields.io/badge/Draw.io-%2500C4CC.svg?style=for-the-badge&logo=draw.io&logoColor=blue">


<h1>🏗️ Arquitetura da Aplicação</h1> 
<img src="https://github.com/Felipaof/Doces-Receitas-/blob/a9fac3e6852b376c50ccba346576e3b18507317c/ARQUITETURA.png" width=1000> 
<h1>💻 Desenvolvedores</h1>

| [<img loading="lazy" src="" width=115><br><sub>Felipe Martins da Silva Santos</sub>](https://github.com/Felipaof) |  [<img loading="lazy" src="" width=115><br><sub>Nathália Silva Souza</sub>](https://github.com/vinimaxi) |
| :---: | :---: |
