# cockadoodledoolearning
For personal Learning
Este código usa a função "input()" para receber uma entrada do usuário como uma string, e usa "map()" e "split()" para converter a string em uma lista de números inteiros. Em seguida, usa a biblioteca "collections" para contar as ocorrências de cada número e obter os 6 números mais comuns usando o método "most_common()" do objeto "Counter". Por fim, imprime esses 6 números mais comuns.

from collections import Counter

# Receber a entrada como uma string
sequence = input("Digite uma sequência de números inteiros, separados por espaço: ")

# Converter a string em uma lista de números
numbers = list(map(int, sequence.split()))

# Contar as ocorrências de cada número
counts = Counter(numbers)

# Obter os 6 números mais comuns
common_nums = counts.most_common(6)

# Imprimir os 6 números mais comuns
print("Os 6 números mais comuns são:", [num for num, count in common_nums])


