# Estruturas de Dados: lista de estudo

> Arquivo de apoio do minicurso **Claude na Prática**.
> Anexe este arquivo ao projeto "Monitor de Estruturas de Dados" no Claude.

## Sobre este arquivo

Este é um exemplo de arquivo **Markdown** (`.md`). A estrutura fica explícita no próprio texto, e é por isso que o Claude lê este formato com tanta fidelidade:

- `#` marca o título; `##` e `###` marcam subtítulos
- `**negrito**` vira **negrito** e `*itálico*` vira *itálico*
- `-` cria listas e `1.` cria listas numeradas
- `` ``` `` abre e fecha um bloco de código
- `|` monta tabelas
- `[texto](endereço)` cria um link, como este [guia de sintaxe Markdown](https://www.markdownguide.org/basic-syntax/)

## Tópicos da disciplina

| Tópico | O que estudar | Complexidade típica |
|---|---|---|
| Pilha | push, pop, topo | O(1) |
| Fila | enfileirar, desenfileirar | O(1) |
| Lista encadeada | inserção, remoção, busca | busca em O(n) |
| Árvore binária de busca | inserção, busca, percursos | O(log n) a O(n) |
| Árvore AVL | balanceamento e rotações | O(log n) |
| Tabela hash | função hash, tratamento de colisões | O(1) em média |

## Exercícios

### 1. Pilha (fácil)

Escreva uma função que verifique se os parênteses de uma expressão estão balanceados.

```python
def balanceado(expr: str) -> bool:
    ...
```

Casos de teste: `"(a+b)*(c-d)"` → `True` e `"((a+b)"` → `False`.

### 2. Fila (fácil)

Implemente uma fila usando **duas pilhas**. Qual é a complexidade amortizada de desenfileirar?

### 3. Lista encadeada (médio)

Inverta uma lista simplesmente encadeada **sem** criar nós novos.

### 4. Árvore binária de busca (médio)

Insira, nesta ordem, os valores `50, 30, 70, 20, 40, 60, 80` e escreva o resultado do percurso **em ordem**.

### 5. Árvore AVL (difícil)

Insira, nesta ordem, `30, 10, 20` numa árvore AVL vazia. Qual rotação é necessária? Desenhe a árvore antes e depois.

### 6. Tabela hash (difícil)

Com a função `h(k) = k mod 7` e tratamento de colisões por encadeamento, insira `10, 17, 24, 3, 5`. Quantas colisões ocorrem?

## Checklist de revisão

- [ ] Sei explicar a diferença entre pilha e fila
- [ ] Sei analisar a complexidade de cada operação
- [ ] Sei fazer rotações AVL à mão
- [ ] Sei explicar por que a busca em hash é O(1) em média, e quando deixa de ser

## Como o Claude deve usar este arquivo

1. Não entregue as respostas dos exercícios.
2. Dê uma dica por vez e espere a minha tentativa.
3. Use exemplos em Python.
4. Termine cada explicação com uma pergunta de verificação.
