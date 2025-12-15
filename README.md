# 📝 Trabalho Prático: Sistema Interativo de Gestão de Turmas

## 📅 Prazo de Entrega
**Data:** 17/12/2025
**Formato:** Entrega do arquivo JavaScript (.js) no lms cada integrante do grupo.

## 🎯 Objetivo
Desenvolver um programa em JavaScript que utilize **Funções**, **Arrays**, **Objetos** e **Estruturas de Repetição** para simular o cadastro e o cálculo da média de notas de uma turma. O programa deverá interagir com o usuário via *prompt*.

## 👨‍👩‍👧‍👦 Equipe
Trabalho em trio. (Máximo 3 Pessoas)

## 🧩 Requisitos e Conceitos Obrigatórios

O projeto deve, obrigatoriamente, incluir o uso dos seguintes conceitos:

| Conceito | Aplicação Obrigatória |
| :--- | :--- |
| **Array** | Um *Array* principal (`const turma = []`) para armazenar todos os alunos. |
| **Objeto** | Cada aluno deve ser armazenado como um **objeto** (ex: `{ nome: '...', nota: 0 }`). |
| **Funções** | Mínimo de **4 funções distintas** para modularizar as etapas do trabalho. |
| **Estrutura de Repetição** | Uso de laços (`for`, `while`, ou `forEach`) em pelo menos **3 momentos** diferentes (cadastro de alunos, lançamento de notas e cálculo da média). |
| **Interatividade** | Uso do comando `prompt()` para coletar todas as informações do usuário. |

## 🛠️ Especificação do Sistema

O sistema deverá seguir as seguintes etapas, utilizando uma função específica para cada uma:

### Etapa 1: Cadastro Inicial da Turma (`cadastrarTurma()`)
1.  A função deve usar `prompt()` para perguntar o **nome da turma** (ex: "Turma 301").
2.  A função deve usar `prompt()` para perguntar a **quantidade de alunos** na turma.
3.  Deve iniciar um **laço de repetição** com base na quantidade informada.
4.  Dentro do laço, deve chamar a função de cadastro de aluno (Etapa 2).

### Etapa 2: Cadastro de Aluno (`cadastrarAluno(indice)`)
1.  Esta função deve ser chamada dentro do laço da Etapa 1.
2.  Usa `prompt()` para perguntar o **nome do aluno** (usando o `indice` para indicar qual aluno está sendo cadastrado).
3.  Cria um **objeto** para o aluno com o nome fornecido e a nota inicializada como `null` ou `0`.
4.  Adiciona este novo objeto ao *Array* principal (`turma.push(...)`).

### Etapa 3: Lançamento das Notas (`lancarNotas()`)
1.  Esta função deve ser chamada somente **após** o cadastro de todos os alunos.
2.  Inicia um **laço de repetição** para percorrer o *Array* `turma`.
3.  Para cada aluno, usa `prompt()` para pedir e coletar a **nota** correspondente.
4.  **Atualiza a propriedade `nota`** no objeto do aluno dentro do *Array*.

### Etapa 4: Cálculo e Exibição da Média (`calcularMedia()`)
1.  Esta função deve ser chamada por último.
2.  Inicia um **terceiro laço de repetição** para somar todas as notas no *Array*.
3.  Calcula a média da turma (**Soma das Notas / Número de Alunos**).
4.  Exibe o resultado no console com uma mensagem clara, indicando o **nome da turma** e a **média final**.

## 📝 Sugestão de Divisão de Tarefas

A divisão abaixo é sugerida para garantir que todos os membros trabalhem com os requisitos principais:

| Aluno(a) | Foco | Tarefas Envolvidas |
| :--- | :--- | :--- |
| **A** | **Fluxo Principal e Laços de Cadastro** | Implementar `cadastrarTurma()` e garantir o fluxo de repetição do cadastro inicial. |
| **B** | **Interação com Dados e Atualização** | Implementar `lancarNotas()`, incluindo o *prompt* e a lógica de atualização dos objetos no *Array*. |
| **C** | **Cálculo e Exibição de Resultados** | Implementar `calcularMedia()`, garantindo o laço para a soma das notas e a exibição formatada. |

---

## ✅ Avaliação

O trabalho será avaliado com base em:

1.  **Funcionalidade:** O programa executa todas as etapas e calcula a média corretamente.
2.  **Uso dos Conceitos:** Aplicação correta e clara de Funções, Arrays, Objetos e Estruturas de Repetição.
3.  **Organização:** Código bem formatado, com comentários e nomes de variáveis e funções claros.
