<h1 align="center">  </h1>
<p align="center">Trabalho para a disciplina de DESENVOLVIMENTO DE APLICAÇÕES PARA DISPOSITIVOS MÓVEIS - 4º Informática do IFSP-Jacareí</p>
<br>
<p align="center">
<img loading="lazy" src="http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=blue&style=for-the-badge"/>

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

<img src="" width=1000> 
<br>
- Observação:

<h2>Matriz de Requisitos Funcionais</h2>



<h1>📱Mockup do APP </h1>

Pré-Mockup da Interface: <img src="" width=1000> 

<h1>📊 Modelagem do Banco de Dados</h1>
<img src="![Diagrama banco de dados ](https://github.com/user-attachments/assets/a019b6d0-5477-4ac9-b8a7-d6b6aa153eb6)
" width=1000>


<h1>📖 Dicionário de dados </h1> 

<h2>Tabela: categorias</h2>  
<table border="1">  
<tr>  
    <th>Nome do Campo</th>  
    <th>Tipo de Dado</th>  
    <th>Tamanho</th>  
    <th>Permite Nulo?</th>  
    <th>Descrição</th>  
</tr>  
<tr>  
    <td>id_categoria</td>  
    <td>INT</td>  
    <td>-</td>  
    <td>NÃO</td>  
    <td>Identificador único da categoria (chave primária, autoincremento).</td>  
</tr>  
<tr>  
    <td>nome_categoria</td>  
    <td>VARCHAR</td>  
    <td>100</td>  
    <td>NÃO</td>  
    <td>Nome da categoria (exemplo: "Bolos").</td>  
</tr>  
</table>  

<h2>Tabela: receitas</h2>  
<table border="1">  
<tr>  
    <th>Nome do Campo</th>  
    <th>Tipo de Dado</th>  
    <th>Tamanho</th>  
    <th>Permite Nulo?</th>  
    <th>Descrição</th>  
</tr>  
<tr>  
    <td>id_receita</td>  
    <td>INT</td>  
    <td>-</td>  
    <td>NÃO</td>  
    <td>Identificador único da receita (chave primária, autoincremento).</td>  
</tr>  
<tr>  
    <td>nome_receita</td>  
    <td>VARCHAR</td>  
    <td>150</td>  
    <td>NÃO</td>  
    <td>Nome da receita (exemplo: "Bolo de cenoura").</td>  
</tr>  
<tr>  
    <td>ingredientes</td>  
    <td>TEXT</td>  
    <td>-</td>  
    <td>NÃO</td>  
    <td>Lista dos ingredientes necessários.</td>  
</tr>  
<tr>  
    <td>modo_preparo</td>  
    <td>TEXT</td>  
    <td>-</td>  
    <td>NÃO</td>  
    <td>Passo a passo para preparar a receita.</td>  
</tr>  
<tr>  
    <td>tempo_preparo</td>  
    <td>INT</td>  
    <td>-</td>  
    <td>NÃO</td>  
    <td>Tempo estimado de preparo (em minutos).</td>  
</tr>  
<tr>  
    <td>rendimento</td>  
    <td>VARCHAR</td>  
    <td>50</td>  
    <td>NÃO</td>  
    <td>Quantidade de porções que a receita rende.</td>  
</tr>  
<tr>  
    <td>id_categoria</td>  
    <td>INT</td>  
    <td>-</td>  
    <td>NÃO</td>  
    <td>Categoria da receita (chave estrangeira de `categorias`).</td>  
</tr>  
<tr>  
    <td>video_link</td>  
    <td>VARCHAR</td>  
    <td>255</td>  
    <td>SIM</td>  
    <td>Link de um vídeo tutorial da receita.</td>  
</tr>  
</table>  

<h2>Tabela: imagens_receitas</h2>  
<table border="1">  
<tr>  
    <th>Nome do Campo</th>  
    <th>Tipo de Dado</th>  
    <th>Tamanho</th>  
    <th>Permite Nulo?</th>  
    <th>Descrição</th>  
</tr>  
<tr>  
    <td>id_imagem</td>  
    <td>INT</td>  
    <td>-</td>  
    <td>NÃO</td>  
    <td>Identificador único da imagem (chave primária, autoincremento).</td>  
</tr>  
<tr>  
    <td>id_receita</td>  
    <td>INT</td>  
    <td>-</td>  
    <td>NÃO</td>  
    <td>Receita relacionada (chave estrangeira de `receitas`).</td>  
</tr>  
<tr>  
    <td>url_imagem</td>  
    <td>VARCHAR</td>  
    <td>255</td>  
    <td>NÃO</td>  
    <td>URL ou caminho da imagem armazenada.</td>  
</tr>  
</table>

<h2>users</h2>

<br><br>

- 

<h2></h2>

<br><br>



<h2>Item</h2>

<br><br>




<h1>🧍Diagramas UML</h1>
<h2>Tela de Login e Cadastro</h2>
<img src="" width=1000>
<h2>Tela principal, criação de coleção e criação de item</h2>
<img src="" width=1000>


<h1>🧰 Tecnologias Utilizadas</h1> 

Front-end e back-end:
<br><br>
<img src="">

Banco de Dados:
<br><br>
<img src="">

Diagramas e Mockups:
<br><br>
<img src="">
<img src="">
<img src="">


<h1>🏗️ Arquitetura da Aplicação</h1> 

<h1>💻 Desenvolvedores</h1>

| [<img src=">]() <br> ** | [<img src = >]() <br> ** |
| :---: | :---: |
