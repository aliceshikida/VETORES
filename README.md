# 🧮 Manipulador de Vetores em C

Este programa em linguagem C permite que o usuário insira **10 números inteiros** e, em seguida, escolha entre diferentes operações matemáticas e manipulações sobre esses valores, por meio de um menu interativo.

## 🚀 Como usar

1. Compile o programa:
- Digite 10 números inteiros conforme solicitado.
- Escolha um caso de 0 a 14 para realizar uma operação específica.

## 📋 Funcionalidades

| Caso         | Operação                                                                 |
|--------------|--------------------------------------------------------------------------|
| `0`          | Finaliza o programa (não faz nada).                                      |
| `1`          | Substitui um número em uma posição específica.                           |
| `2`          | Mostra os números na ordem original.                                     |
| `3`          | Mostra os números na ordem reversa.                                      |
| `4`          | Soma todos os valores do vetor.                                          |
| `5`          | Conta quantos números se repetem.                                        |
| `6`          | Imprime os números diferentes (⚠️ implementação incorreta).              |
| `7`          | Exibe quantas vezes cada número aparece.                                 |
| `8`          | Ordena o vetor em ordem crescente e mostra mínimo, máximo e valor médio. |
| `9`          | Calcula e exibe a mediana (posição 4 + 5 / 2).                           |
| `10`         | Ordena o vetor em ordem crescente.                                       |
| `11`         | Ordena o vetor em ordem decrescente.                                     |
| `12`         | Exibe separadamente os números pares e ímpares (sem repetições).         |
| Outro número | Mostra “inválido”.                                                       |


📌 Observações
- O vetor é fixo com 10 elementos.
- As posições no código vão de 0 a 9, mas o usuário insere posições de 1 a 10.
- O programa não verifica erros de entrada (por exemplo, posição inválida).
- O caso 6 contém uma lógica incorreta: imprime muitos valores repetidos. Pode ser corrigido com verificações de duplicidade.
