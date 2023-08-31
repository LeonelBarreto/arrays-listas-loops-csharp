# Exercício 12

## Fila do banco

Neste exercício iremos controlar a fila de um banco que tem um limite de pessoas que podem ficar do lado de dentro.
Portanto, enquanto houver pessoas do lado de fora e do lado de dentro ainda não tenha atingido o limite permitido, deveremos permitir a entrada.

Para isso, teremos dois arrays (um para controlar a fila do lado de dentro do banco e outro para controlar a fila do lado de fora) de strings onde cada elemento é o nome da pessoa que está na fila.

Portanto, enquanto houverem elementos na fila de fora e espaços disponíveis dentro do limite na fila de dentro, deveremos passar o primeiro elemento da fila de fora para a última posição da fila de dentro.

Ao final, imprima todos os elementos da fila de dentro e em seguida imprima todos os elementos da fila de fora.

Exemplo:

Suponha que existam 3 pessoas na fila de dentro e 4 pessoas na fila de fora:

```
string[] filaDeDentro = { "Léo", "Laerte", "Marcelo" };
string[] filaDeFora = { "Igor", "Felippe", "João", "Iuri" };
```

Escreva o código que verificará a fila de fora, um elemento de cada vez, e se caso a fila de dentro ainda não estiver alcançado o limite máximo, por exemplo, de 5 pessoas, deverá passar a primeira pessoa da fila de fora para a última posição da fila de dentro, até que complete o limite de 5 pessoas.

No exemplo dado acima, o que deve ser impresso no console ao final do programa é:

```
Fila de dentro: Léo, Laerte, Marcelo, Igor, Felippe
Fila de fora: João, Iuri
```
