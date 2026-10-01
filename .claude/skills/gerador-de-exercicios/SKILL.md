---
name: gerador-de-exercicios
description: Gera listas de 5 exercícios de programação em Python sobre estruturas de dados, em ordem crescente de dificuldade, com casos de teste executáveis e o gabarito separado no fim. Use quando o estudante ou o professor pedir exercícios, uma lista de exercícios, prática ou questões sobre um tópico (pilha, fila, lista encadeada, árvores, AVL, hash, ordenação etc.).
---

# Gerador de exercícios

Gera uma lista com **5 exercícios** sobre o tópico pedido, do mais fácil ao
mais difícil, com casos de teste em Python e o **gabarito separado no fim**.
Quando esta skill for usada, este formato substitui o formato de três partes
de `INSTRUCOES.md`.

## Passo a passo

1. **Identifique o tópico.** Se o pedido não disser, use o tópico em discussão
   na conversa. Consulte a tabela de tópicos de `lista-de-estudo.md` para
   manter a nomenclatura e as complexidades da disciplina.
2. **Planeje a progressão de dificuldade:**
   1. Fácil: usar uma operação básica da estrutura.
   2. Fácil/médio: combinar duas operações.
   3. Médio: implementar uma operação da estrutura à mão.
   4. Médio/difícil: aplicar a estrutura para resolver um problema.
   5. Difícil: variação, otimização ou análise de complexidade.
3. **Não repita** os exercícios de `lista-de-estudo.md`: eles são resolvidos
   pelo estudante com dicas do monitor.
4. **Escreva cada exercício** com:
   - título com o número e a dificuldade (`### 1. <título> (fácil)`);
   - enunciado curto e sem ambiguidade;
   - assinatura da função em Python com tipos e corpo `...`;
   - bloco de casos de teste com `assert`, cobrindo o caso comum, um caso de
     borda (vazio, um elemento, valores repetidos) e, quando couber, um caso
     de erro.
5. **Escreva o gabarito** depois de todos os exercícios, separado por uma
   linha horizontal (`---`) e o título `## Gabarito`, para que o estudante
   não o veja por acidente. Para cada exercício, dê uma solução comentada e a
   complexidade de tempo e espaço.
6. **Verifique antes de responder:** rode cada solução do gabarito junto com
   os seus casos de teste e corrija o que falhar. Use apenas a biblioteca
   padrão do Python 3.

## Formato da resposta

````markdown
# Exercícios: <tópico>

Como usar: implemente cada função e rode o bloco de testes logo abaixo dela.
Se nenhum `AssertionError` aparecer, os testes passaram.

### 1. <título> (fácil)

<enunciado>

```python
def nome_da_funcao(param: tipo) -> tipo:
    ...

# Casos de teste
assert nome_da_funcao(...) == ...
assert nome_da_funcao(...) == ...  # caso de borda
print("Exercício 1: todos os testes passaram!")
```

### 2. ... (fácil/médio)
### 3. ... (médio)
### 4. ... (médio/difícil)
### 5. ... (difícil)

---

## Gabarito

> Tente resolver antes de olhar!

### 1. <título>

```python
# solução comentada
```

**Complexidade:** O(...) de tempo e O(...) de espaço, porque <motivo>.

### 2. ...
````
