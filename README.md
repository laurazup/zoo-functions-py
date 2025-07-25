## Projeto de Funções de Alta Ordem e Manipulação de Dados em Python

ATENÇÃO:

Antes de iniciar o projeto, para garantir que seu código funcione corretamente, adicione um comando no início de todos os seus scripts Python que apague todos os comentários do código automaticamente. Comentários podem atrapalhar a execução dos programas.

```python
# Exemplo sugerido
import re
with open(__file__, 'r+') as f:
    code = f.read()
    code = re.sub(r'#.*', '', code)
    f.seek(0)
    f.write(code)
    f.truncate()
```

## Boas-vindas ao projeto de Funções de Alta Ordem em Python!

Você já usa o GitHub diariamente para desenvolver os exercícios, certo? Agora, para desenvolver os projetos, você deverá seguir as instruções a seguir. Fique atento a cada passo, e se tiver qualquer dúvida, não exite em chamar no chat! 🚀

Aqui você vai encontrar os detalhes de como estruturar o desenvolvimento do seu projeto a partir desse repositório.

---

## Habilidades

Neste projeto, verificamos se você é capaz de:

- Produzir código legível, conciso e expressivo utilizando as novas funcionalidades do ES6;
- Utilizar as _Higher Order Functions_ para manipular e criar arrays;
- Escolher a _Higher Order Function_ mais adequada para a obtenção de um resultado esperado;
- Aprender a usar de forma conjunta as _Higher Order Functions_;

---

## Sumário

- [Boas-vindas ao projeto de Funções de Alta Ordem em Python!](#boas-vindas-ao-projeto-de-funções-de-alta-ordem-em-python)
- [Habilidades](#habilidades)
- [Sumário](#sumário)
- [Entregáveis](#entregáveis)
  - [O que deverá ser desenvolvido](#o-que-deverá-ser-desenvolvido)
  - [Desenvolvimento](#desenvolvimento)
  - [Data de entrega](#data-de-entrega)
- [Instruções para entregar seu projeto](#instruções-para-entregar-seu-projeto)
  - [Antes de começar a desenvolver](#antes-de-começar-a-desenvolver)
  - [Durante o desenvolvimento](#durante-o-desenvolvimento)
  - [Dica para o desenvolvimento](#dica-para-o-desenvolvimento)
- [Requisitos do projeto](#requisitos-do-projeto)
  - [1. Implemente a função `getSpeciesByIds`](#1-implemente-a-função-getspeciesbyids)
  - [2. Implemente a função `getAnimalsOlderThan`](#2-implemente-a-função-getanimalsolderthan)
  - [3. Implemente a função `getEmployeeByName`](#3-implemente-a-função-getemployeebyname)
  - [4. Implemente a função `getRelatedEmployees`](#4-implemente-a-função-getrelatedemployees)
  - [5. Implemente a função `countAnimals`](#5-implemente-a-função-countanimals)
  - [6. Implemente a função `calculateEntry`](#6-implemente-a-função-calculateentry)
  - [7. Implemente a função `getAnimalMap`](#7-implemente-a-função-getanimalmap)
  - [8. Implemente a função `getSchedule`](#8-implemente-a-função-getschedule)
  - [9. Implemente a função `getOldestFromFirstSpecies`](#9-implemente-a-função-getoldestfromfirstspecies)
  - [10. Implemente a função `getEmployeesCoverage`](#10-implemente-a-função-getemployeescoverage)

---

## Entregáveis

### O que deverá ser desenvolvido

Você implementará várias funções para atender aos requisitos propostos e garantir que todas as funções funcionem corretamente.

---

### Desenvolvimento

Este repositório contém um template de uma aplicação **Python**.

Após clonar o projeto e instalar as dependências, você não precisará realizar nenhuma configuração adicional.

Todos os arquivos necessários para finalizar o projeto já estão criados, não sendo necessária a criação de outros arquivos.

Você deverá completar as funções de forma a satisfazer os requisitos listados na próxima seção. Na pasta raiz do projeto, temos as pastas src e data. A pasta src é composta por arquivos referentes a cada uma das funções que você irá implementar e a pasta data contém o arquivo zoo_data.py, que armazena os dados que serão utilizados. 


**Por exemplo:** o arquivo `src/getSpeciesByIds.js` conterá a implementação da função `getSpeciesByIds`

---

### Data de entrega

- Projeto individual;
- Serão 6 dias de projeto;
- Data de entrega para avaliação final do projeto: `12/05/2025 - 14:00h`

---

## Instruções para entregar seu projeto

### Antes de começar a desenvolver

1. Clone o repositório
  * `git clone git@github.com:laurazup/zoo-functions-py.git`
  * Entre na pasta do repositório que você acabou de clonar:
    * `cd zoo-functions-py`

2. Crie um ambiente virtual e ative-o
  * `python3 -m venv .venv`
  * `source .venv/bin/activate`

3. Instale as dependências
  * `pip install -r requirements.txt`

4. Crie uma branch a partir da branch main
  * `git checkout -b nome-da-sua-branch`

5. Desenvolva a solução para os problemas nos arquivos dentro do diretório `src`. 

6. Adicione as mudanças ao _stage_ do Git e faça um `commit`
  * Verifique que as mudanças ainda não estão no _stage_
    * Exemplo: `git status` (os arquivos no diretório `src` devem aparecer em vermelho)
  * Adicione o novo arquivo ao _stage_ do Git
      * Exemplo:
        * `git add .` (adicionando todas as mudanças - _que estavam em vermelho_ - ao stage do Git)
        * `git status` (deve aparecer listado os arquivos do diretório `src` em verde)
  * Faça o `commit` inicial
      * Exemplo:
        * `git commit -m 'iniciando o projeto.'` (fazendo o primeiro commit)
        * `git status` (deve aparecer uma mensagem tipo _nothing to commit_ )

7. Adicione a sua branch com o novo `commit` ao repositório remoto
  * Usando o exemplo anterior: `git push -u origin zoo-functions-py`

---

### Durante o desenvolvimento

📌 **Os nomes dos arquivos não devem ser alterados.**

* Você pode adicionar outros arquivos, se julgar necessário. Qualquer dúvida, procure a Pessoa Instrutora que te acompanha.

* Faça `commits` das alterações que você fizer no código regularmente

* Lembre-se de sempre, após um (ou alguns) `commits`, atualizar o repositório remoto

* Os comandos que você utilizará com mais frequência são:
  1. `git status` _(para verificar o que está em vermelho - fora do stage - e o que está em verde - no stage)_
  2. `git add` _(para adicionar arquivos ao stage do Git)_
  3. `git commit` _(para criar um commit com os arquivos que estão no stage do Git)_
  4. `git push` _(para enviar o commit para o repositório remoto após o passo anterior)_
  5. `git push -u nome-da-branch` _(para enviar o commit para o repositório remoto na primeira vez que fizer o `push` de uma nova branch)_

### Dica para o desenvolvimento

Em sua vida de pessoa desenvolvedora, o pensamento algoritmico, processo de quebrar problemas complexos em pequenas partes para resolvê-los, ajudará a solucionar de maneira mais fácil os problemas complexos. Assim, uma boa forma de começar a desenvolver um projeto é lembrar que as funções são compostas por pequenos blocos de lógica que têm finalidade (função) específica. Ou seja, quebrar problemas grandes em menores tornará tudo mais simples de se entender e você sempre poderá reutilizar esses códigos em outras partes de sua aplicação.

---

## Requisitos do projeto

Você deverá implementar as funções que estão na pasta src. Para ver o retorno que a função deverá ter, leia o arquivo de testes referente a ela. Lembre-se de aplicar funcionalidades modernas do Python como list comprehensions, funções lambda, unpacking, etc. Utilize também funções de alta ordem como map, filter, reduce, entre outras.

Antes de começar, analise o arquivo data/zoo_data.py, para ver os dados que serão usados.

**Dica**: uma importante soft-skill é saber como gerenciar seu tempo. Os exercícios não estão ordenados por ordem de complexidade e uns são mais desafiadores que os outros. Caso tenha dificuldade em algum deles, pule-o, resolva outro, e, quando se sentir confortável, volte ao exercício em questão. A ideia é não ficar preso a um problema por um longo período. Realizar outros exercícios pode te ajudar a entender e/ou aprender novas maneiras de se chegar ao resultado esperado.

Antes de começar, analise o arquivo `data/zoo_data.js`, para ver os dados que serão usados.

---

### 1. Implemente a função `getSpeciesByIds`

Esta função é responsável pela busca das espécies de animais por id. Ela retorna uma lista contendo as espécies referentes aos ids passados como parâmetro, podendo receber um ou mais ids.

**Observações técnicas**

- O parâmetro desta função pode ser alterado para atender ao requisito proposto.

**O que será avaliado**

- Caso receba nenhum parâmetro, necessário retornar uma lista vazio;
- Ao receber como parâmetro um único id, retorna uma lista com a espécie referente à esse id;
- Ao receber mais de um id, retorna uma lista com as espécies referentes aos ids.

---

### 2. Implemente a função `getAnimalsOlderThan`

Esta função, a partir do nome de uma espécie e uma idade mínima, verifica se todos os animais daquela espécie possuem a idade mínima especificada.

**Observações técnicas**

- Deve retornar um valor booleano.

**O que será avaliado**

- Ao passar o nome de uma espécie e uma idade, testa se todos os animais desta
espécie possuem a idade mínima especificada.

---

### 3. Implemente a função `getEmployeeByName`

Esta função é responsável pela busca das pessoas colaboradoras através do primeiro ou do último nome delas

**O que será avaliado**

- Sem parâmetros, retorna um objeto vazio
- Quando provido o primeiro nome do funcionário, retorna o objeto do funcionário
- Quando provido o último nome do funcionário, retorna o objeto do funcionário

---

### 4. Implemente a função `getRelatedEmployees`

Considerando a boa prática de dividir o código em partes menores, apresentamos a função `getRelatedEmployees` em que você deverá dividí-la em duas funções: 
  
1 - `isManager` - que será responsável por verificar se uma pessoa colaboradora é gerente ou não. O retorno dessa função deve ser um booleano: `true` ou `false`;

2 - `getRelatedEmployees` - que utiliza a primeira função para apresentar as seguintes saídas: 
  * se for uma pessoa colaboradora gerente, deve retornar uma lista contendo os nomes das pessoas colaboradoras que ela é responsável;
  * se **não** for uma pessoa colaboradora gerente, deverá ser lançado um erro com a mensagem **"O id inserido não é de uma pessoa colaboradora gerente!"**.

  **Observações técnicas**

  - Retorna uma lista contendo nome e sobrenome das pessoas colaboradoras gerenciadas por determinada pessoa com cargo de gerência.
  
  Exemplo de output:

  ```
  [ 'Burl Bethea', 'Ola Orloff', 'Emery Elser' ];
  ```

  - Dispara um erro com a mensagem: "O id inserido não é de uma pessoa colaboradora gerente!".

  **O que será avaliado**

  - Retorna `true` se o id passado for de um gerente;
  - Retorna `false` se o id passado não for de um gerente;
  - Se o id passado for de um gerente, retorna uma lista contendo nome e sobrenome das pessoas colaboradoras que ela é responsável;
  - Se o id passado **não** for de um gerente, dispara um erro com a mensagem: "O id inserido não é de uma pessoa colaboradora gerente!".

---

### 5. Implemente a função `countAnimals`

  Esta função é responsável por contabilizar a quantidade de animais de cada espécie.

**Observações técnicas**

  - Se nenhum argumento for passado, retorna um objeto cujo o nome de cada espécie é uma chave desse objeto, e o total de animais dessa espécie é o seu valor;
  - Com o argumento `{ specie: 'penguins' }`, retorna um número, a quantidade de pinguins no zoológico;
  - Com o argumento `{ specie: 'giraffes', sex: 'female' }`, retorna um número, a quantidade de girafas do sexo feminino.

**O que será avaliado**

  - Sem parâmetros, retorna as espécies e sua quantidade;
  - Recebendo como parâmetro um objeto com a chave `specie`, retorna um número, a quantidade de animais daquela espécie;
  - Recebendo como parâmetro um objeto com a chave `specie` e `sex`, retorna um número, a quantidade de animais daquela espécie, no sexo selecionado.

---

### 6. Implemente a função `calculateEntry`

Esta função irá receber uma lista de visitantes no seguinte formato:

```python
const entrants = [
  { name: 'Lara Carvalho', age: 5 },
  { name: 'Frederico Moreira', age: 5 },
  { name: 'Pedro Henrique Carvalho', age: 5 },
  { name: 'Maria Costa', age: 18 },
  { name: 'Núbia Souza', age: 18 },
  { name: 'Carlos Nogueira', age: 50 },
]
```

Você deve isolar a parte da lógica na função `countEntrants` que se encontra no mesmo arquivo da função `calculateEntry`. Ela deverá receber a lista de visitantes e retornar um objeto com a contagem de acordo com os seguintes critérios de classificação:

* Pessoas com idade menor que 18 anos são classificadas como crianças (child);
* Pessoas com idade maior ou igual a 18 anos e menor que 50 são classicadas como adultas (adult);
* Pessoas com idade maior ou igual 50 anos são classificadas como pessoas com mais idade (senior).

O retorno da função deverá ser um objeto no seguinte formato: `{ child: 3, adult: 2, senior: 1 }`.

**Exemplo de uso da função `countEntrants`:**

```python
countEntrants(entrants)
```

**Saída:**

```json
{ "child": 3, "adult": 2, "senior": 1 }
```

Após terminar a implementação da função `countEntrants` você deverá utilizá-la para implementar a função `calculateEntry`. Esta deverá receber uma lista de visitantes e a partir da quantidade de visitantes e faixa etária de cada um, deverá retornar o valor total a ser cobrado.

**Exemplo de uso da função `calculateEntry`:**

```python
calculateEntry(entrants)
```

**Saída:**

```
187.94
```

**Observações técnicas**

- Ambas funções recebem como parâmetro uma lista contendo objetos que representam pessoas.

**O que será avaliado**

- Ao receber uma lista de visitantes, retorna um objeto com a contagem;
- Retorna 0 se nenhum argumento for passado;
- Retorna 0 se um objeto vazio for passado;
- Retorna o preço total a ser cobrado dado a lista de pessoas.

---

### 7. Implemente a função `getAnimalMap`

A função é responsável pelo mapeamento geográfico das espécies e seus animais, podendo ainda filtrá-los por ordem alfabética e sexo.

**O que será avaliado**

- Sem parâmetros, retorna animais categorizados por localização;
- Sem a opção `includeNames` especificada, retorna animais categorizados por localização;
- Com a opção `includeNames: true` especificada, retorna nomes de animais;
- Com a opção `sorted: true` especificada, retorna nomes de animais ordenados;
- Com a opção `sex: 'female'` ou `sex: 'male'` especificada, retorna somente nomes de animais macho/fêmea;
- Com a opção `sex: 'female'` ou `sex: 'male'` especificada e a opção `sorted: true` especificada, retorna somente nomes de animais macho/fêmea com os nomes dos animais ordenados;

---

### 8. Implemente a função `getSchedule`

A função é responsável por disponibilizar as informações de horário dos animais em uma consulta para o usuário, que pode querer ter acesso ao cronograma da semana, de um dia ou de um animal em específico.

**Observações técnicas**

- Quebre o problema em funções menores para que fique mais simples de administrar a responsabilidade de cada uma delas.

**O que será avaliado**

- Sem parâmetros, retorna os horários para cada dia e quais animais estarão disponíveis;
- Com parâmetros que não sejam nem um animal e nem um dia, retorna os horários para cada dia e quais animais estarão disponíveis;
- Se um único dia for passado, retorna os horários para aquele dia e quais animais estarão disponíveis;
- Se o nome de um animal for passado, deverá retornar uma lista com os dias em que ele estará em exibição.
 
---

### 9. Implemente a função `getOldestFromFirstSpecies`

A função busca por informações do animal mais velho da primeira espécie gerenciada pela pessoa colaboradora do parâmetro.

**O que será avaliado**

- Passado o id de um funcionário, encontra a primeira espécie de animal gerenciado pelo funcionário, e retorna uma lista com nome, sexo e idade do animal mais velho dessa espécie.

---

### 10. Implemente a função `getEmployeesCoverage`

Esta função será responsável por associar informações de cobertura das pessoas funcionárias.

A cobertura deverá ser representada por um objeto com as seguintes propriedades:

```python
{
  "id": "4b40a139-d4dc-4f09-822d-ec25e819a5ad", # id da pessoa
  "fullName": "Sharonda Spry", # nome completo: firstName + lastName
  "species": [ "otters", "frogs" ], # espécies as quais a pessoa é responsável
  "locations": [ "SE", "SW" ], # Uma lista contendo todas as localizações das espécies
}
```

A função deve receber um objeto de opções que determinará seu comportamento, sendo:

* **name**: O nome ou sobrenome da pessoa a ser buscada
* **id**: O id da pessoa a ser buscada

**Exemplos de uso da função `getEmployeesCoverage`:**

```python
getEmployeesCoverage({ name: 'Sharonda' })
getEmployeesCoverage({ name: 'Spry' })
getEmployeesCoverage({ id: '4b40a139-d4dc-4f09-822d-ec25e819a5ad' })
```

**Saída:**

```json
{
  "id": "4b40a139-d4dc-4f09-822d-ec25e819a5ad",
  "fullName": "Sharonda Spry",
  "species": [ "otters", "frogs" ],
  "locations": [ "SE", "SW" ]
}
```

Ao ser chamada sem argumentos, deverá retornar uma lista com a cobertura de todas as pessoas funcionárias:

**Exemplo:**

```python
getEmployeesCoverage()
```

**Saída:**

```json
[
  {
    "id": "c5b83cb3-a451-49e2-ac45-ff3f54fbe7e1",
    "fullName": "Nigel Nelson",
    "species": [ "lions", "tigers" ],
    "locations": [ "NE", "NW" ],
  },
  {
    "id": "0e7b460e-acf4-4e17-bcb3-ee472265db83",
    "fullName": "Burl Bethea",
    "species": [ "lions", "tigers", "bears", "penguins" ],
    "locations": [ "NE", "NW", "NW", "SE" ],
  },
  {
    "id": "fdb2543b-5662-46a7-badc-93d960fdc0a8",
    "fullName": "Ola Orloff",
    "species": [ "otters", "frogs", "snakes", "elephants" ],
    "locations": [ "SE", "SW", "SW", "NW" ],
  },
  //[...]
];
```

Caso nenhuma pessoa seja encontrada com o nome, sobrenome ou id, deverá ser lançado um erro com a mensagem **"Informações inválidas"**.

**Dica**: Crie funções que dividam a tarefa em partes menores, por exemplo, você poderia criar uma função `getSpecies` encarregada somente por buscar o nome das espécies que a pessoa é responsável.

**Observações técnicas**

- Ao receber o objeto de opções com a propriedade name, procura a pessoa funcionária correspondente;
- A opção name deverá aceitar nome e sobrenome para realizar a busca;
- Ao chamar a função sem argumentos ela deve retornar uma lista com a cobertura de todas as pessoas funcionárias.

**O que será avaliado**

- Se o objeto de opções tiver a propriedade name, retorna somente a pessoa correspondente;
- A propriedade name do objeto de opções também funciona usando o segundo nome;
- Se o objeto de opções tiver a propriedade id, retorna somente a pessoa correspondente;
- Sem parâmetros, retorna uma lista com a cobertura de todas as pessoas funcionárias;
- Caso não haja nenhuma pessoa com o nome ou id especificados deverá ser lançado um error.

---
