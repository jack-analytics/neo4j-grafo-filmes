# 🎬 Grafo Neo4j – Streaming, Indicações e Globo de Ouro 2026

Este projeto consiste na criação de um **grafo em Neo4j** que simula **perfis de usuários em diferentes plataformas de streaming** e suas interações com **filmes e séries** relacionados à **premiação Globo de Ouro 2026**.

O modelo permite analisar **padrões de indicação**, **obras assistidas ou não assistidas**, e **correlações entre atores, diretores, gêneros e premiações**, utilizando a linguagem **Cypher**.

---

## 🧠 Objetivo do Projeto

O objetivo principal é representar, por meio de grafos:

- Usuários de plataformas de streaming  
- Filmes e séries indicados ou vencedores do **Globo de Ouro 2026**  
- A relação entre **atores que atuaram tanto em filmes quanto em séries**
- Diretores que podem ser **iguais ou diferentes** entre as obras
- A classificação das obras por **gênero**

A partir dessas relações, o grafo permite:
- Simular **indicações de conteúdo** para usuários  
- Explorar **correlações entre premiações e tipos de relacionamento**
- Identificar **padrões recorrentes** em obras premiadas ou indicadas  

---

## 🎯 Regras de Modelagem Aplicadas

O projeto segue algumas regras conceituais centrais:

1. Um usuário pode:
   - Ter assistido a uma série
   - Receber indicação para assistir a um filme (ou vice-versa)

2. A indicação ocorre quando:
   - O **mesmo ator** atuou tanto no filme quanto na série  
   - As obras estão relacionadas à **premiação Globo de Ouro 2026**  
   - Os diretores podem ser:
     - O mesmo em ambas as obras
     - Ou diretores diferentes

3. Toda obra (filme ou série):
   - Está associada a **um ou mais gêneros**
   - Pode estar marcada como **Indicado** ou **Vencedor**

---

## 🧩 Estrutura do Grafo

### 🔹 Tipos de Nós (Labels)

- `User` – Perfis de usuários de streaming  
- `Filme` – Filmes  
- `Serie` – Séries  
- `Ator` / `Atriz` – Elenco  
- `Diretor` – Diretores das obras  
- `Genre` – Gêneros cinematográficos  

---

### 🔹 Tipos de Relacionamentos

- `WATCHED` – Usuário assistiu a uma obra  
- `DIDNT_WATCH` – Usuário não assistiu, mas recebeu indicação  
- `ACTED_IN` – Ator/Atriz atuou em filme ou série  
- `DIRECTED` – Diretor dirigiu obra  
- `IN_GENRE` – Classificação por gênero  

Alguns relacionamentos possuem **propriedades temporais ou contextuais**, como o ano em que a obra foi assistida ou se a indicação foi apenas uma possibilidade.

---

## 🛠 Tecnologias Utilizadas

- **Neo4j**
- **Cypher Query Language**
- **Neo4j Browser**
- **GitHub**

---

## ▶️ Como executar o projeto

1. Instale o **Neo4j Desktop** ou utilize o **Neo4j Aura**
2. Crie e inicie um banco de dados
3. Abra o **Neo4j Browser**
4. Copie o conteúdo do arquivo `.cypher` deste repositório
5. Cole no editor do Browser
6. Execute as queries para gerar o grafo

---

## 📊 Possibilidades de Análise

Com o grafo criado, é possível:

- Identificar **atores recorrentes** em obras indicadas ou vencedoras  
- Analisar se determinados **gêneros** aparecem com mais frequência em premiações  
- Avaliar **padrões de indicação** entre filmes e séries  
- Explorar **relacionamentos predominantes** no contexto do Globo de Ouro  

---

## 🎓 Contexto Acadêmico

Este projeto foi desenvolvido como parte de um **módulo do curso de Neo4j**  
na plataforma **DIO (Digital Innovation One)**, iniciado em **janeiro de 2026**.

O foco do módulo é a prática de:
- Modelagem de grafos
- Relacionamentos complexos
- Consultas e inferências utilizando Cypher

---

## 👩‍💻 Autora

Projeto desenvolvido por **Jackelinne Micali**  
Curso de Neo4j – Plataforma DIO
