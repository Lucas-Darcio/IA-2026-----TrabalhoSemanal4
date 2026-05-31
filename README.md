# Trabalho Semanal 4 - Redes Neurais Artificiais (Solucionador de Sudoku)

**Autores:**
* Amanda Nicole Silveira Spellen
* Lucas de Oliveira Darcio

---

## 📌 Descrição do Projeto
Este repositório contém o desenvolvimento e a análise de abordagens de Inteligência Artificial para a resolução de quebra-cabeças do tipo **Sudoku**. O objetivo principal é avaliar o comportamento de redes neurais artificiais contínuas (como perceptrons multicamadas e transformers) frente a problemas de lógica discreta e satisfação de restrições.

O arquivo principal do projeto é o notebook `IA_Trabalho_Semanal_4.ipynb`.

---

## 🏗️ Estrutura do Código

O notebook está dividido em duas abordagens principais e uma seção teórica:

1. **Modelo Principal (Sudoku 4x4)**
   * **Dataset:** Geração automática e dinâmica de tabuleiros válidos de Sudoku 4x4 utilizando técnicas de permutação e codificação *One-Hot Encoding*.
   * **Arquitetura (RNA):** Uma rede neural clássica do tipo Multi-Layer Perceptron (MLP/Feedforward) construída com PyTorch.
   * **Treinamento:** Mapeamento probabilístico das 16 células simultaneamente com otimizador Adam e perda por Entropia Cruzada (*CrossEntropyLoss*).

2. **Seção de Análise Teórica**
   * Discussão fundamentada no livro texto (Russell & Norvig, Cap. 6) abordando a maldição da dimensionalidade no Sudoku 9x9, as limitações do método puramente empírico de "gerar e testar", e os Problemas de Satisfação de Restrições (CSPs).

3. **Modelo Generalizado para NxN (Tentativa)**
   * Uma abordagem experimental utilizando uma rede baseada em **Transformer** (`SudokuTransformer`) combinada com um motor lógico simbólico de *Backtracking* orientado por restrições matemáticas e probabilísticas.

---

## 🛠️ Tecnologias Utilizadas
* Python 3
* PyTorch (`torch`)
* NumPy
* Tqdm (Barra de progresso)

---

## 🤖 Declaração de Uso de Assistentes de IA (Chatbots)

Em conformidade com as boas práticas acadêmicas e diretrizes de transparência, declara-se que ferramentas de modelos de linguagem (Chatbots/LLMs) foram integradas no fluxo de trabalho deste projeto das seguintes formas:

* **Desenvolvimento do Código:** Utilizados como copilotos técnicos para acelerar a escrita e estruturação da arquitetura no PyTorch, na implementação eficiente das lógicas de permutação matemática de matrizes para o dataset, e na criação da heurística baseada em MRV (*Minimum Remaining Values*) guiada por probabilidades.
* **Formatação e Documentação:** Empregados para refinar e padronizar o estilo visual e os comentários do código-fonte (limpeza e organização dos blocos), além da estruturação e estilização textual em Markdown das análises teóricas apresentadas no notebook e deste arquivo README.
