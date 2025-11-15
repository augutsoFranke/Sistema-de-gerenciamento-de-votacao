# Sistema de Gerenciamento de Votação (CLI em Java)

Projeto desenvolvido para a disciplina **Programação Orientada a Objeto**, ministrada pelo professor **André Martins do Nascimento**.

Aplicação em linha de comando (CLI) para gerenciamento de um processo de votação simples, com **cadastro de candidatos e eleitores**, **registro de votos** e **contagem de resultados**, utilizando **conceitos de POO em Java** e **persistência em arquivos**.

---

## 📚 Informações do Projeto

- **Disciplina:** Programação Orientada a Objeto  
- **Professor:** André Martins do Nascimento  

### 👨‍🎓 Alunos

- Augusto do Rêgo Franke  
- Henrique Patta Rodrigues  

---

## 📝 Descrição Geral

O sistema permite:

- Cadastrar, listar, atualizar e remover **candidatos**;
- Cadastrar, listar, atualizar e remover **eleitores**;
- Registrar **votos** associando um eleitor a um candidato;
- Garantir que cada eleitor vote **apenas uma vez**;
- Contar votos por candidato e exibir o **resultado da eleição**;
- Salvar e carregar dados (candidatos, eleitores e votos) em **arquivos**, garantindo persistência entre execuções;
- Interagir via **linha de comando**, com menus e opções numéricas.

---

## 🧩 Funcionalidades Principais

- **Cadastro de candidatos**
  - Inclusão de novos candidatos com nome e número.
- **Cadastro de eleitores**
  - Inclusão de eleitores com nome e identificador (ex.: matrícula).
- **Registro de voto**
  - Identificação do eleitor;
  - Escolha de um candidato;
  - Verificação se o eleitor já votou.
- **Contagem de votos**
  - Quantidade de votos por candidato;
  - Exibição de resultados no terminal.
- **Persistência em arquivos**
  - Salvamento e carregamento de dados de candidatos, eleitores e votos.

---

## 🧱 Organização do Sistema (Visão de POO)

O projeto é organizado em camadas simples, para reforçar conceitos de POO em Java:

- **Domínio**
  - `Candidato`
  - `Eleitor`
  - `Voto`

- **Serviço / Controle**
  - `SistemaVotacao`  
    - Orquestra operações de cadastro, votação e contagem de votos.

- **Persistência**
  - `RepositorioCandidatos` / `RepositorioCandidatosArquivo`
  - `RepositorioEleitores` / `RepositorioEleitoresArquivo`
  - `RepositorioVotos` / `RepositorioVotosArquivo`

- **Interface (CLI)**
  - `AplicacaoVotacao` (classe `main`)  
    - Exibe menus;  
    - Lê opções do usuário;  
    - Chama métodos de `SistemaVotacao`.

---

## ⚙️ Tecnologias Utilizadas

- **Linguagem:** Java  
- **Interface:** Linha de comando (CLI)  
- **Persistência:** Arquivos em disco
- **Paradigma:** Programação Orientada a Objetos

---
