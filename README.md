# combining-tree-interrupting

```
O algoritmo retorna combinações entre elementos com bastante otimização e permite o input de restrições.
As restrições são realizadas através de números primos, permitindo-se, assim, filtrar as combinações indesejadas.
Para melhor otmização as arvores de combinações são interropidas quando rejetadas pelas restrições dando bastanto velocidade.
```

## Parametros
```
main(elements, restrictions, group_size, n_results)

elements: ['pedra', 'papel', 'tesoura', 'lagarto', 'spock']

restrictions: {
  mutualExclusive: [['pedra', 'papel']],
  invalidGroups: [['papel', 'lagarto'], ['spock', 'papel']],
};

n_results: 2

```

#### elements
```
Um array de elementos a serem combinados
```

#### restrictions.mutualExclusive
```
Restringe elementos mutualmente exclusivos.
No caso qualquer combinação em que 'papel' e 'pedra' apareçam juntos serão filtrados
```

#### restrictions.invalidGroups
```
Restringe as cominações exatas inputadas.
No caso as cominações 'papel' e 'lagarto'; e 'spock' e 'papel' serão filtrados
```

#### n_results
```
O numero de combinações a serem retornados
```
