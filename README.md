# Dicionario de Produtos e Precos

1. Crie um dicionario com precos pelo menos 4 produtos e seus respectivos PARSE_COLNAMES2. 
2. Solicite ao usuario que insira o nome de um produtos
3. Verifique se o produtos está no dicionario e exiba o preco. Caso o produtos estea no dicionario,
exiba uma mensagem informando que o produtos não foi encontrado

Resultado:


# Passo 1: Criar o dicionário com produtos e preços
produtos_precos = {
    "maçã": 2.50,
    "banana": 1.20,
    "laranja": 3.00,
    "abacaxi": 5.00
}

# Passo 2: Solicitar ao usuário que insira o nome de um produto
produto_usuario = input("Digite o nome do produto: ").lower()

# Passo 3: Verificar se o produto está no dicionário
if produto_usuario in produtos_precos:
    preco = produtos_precos[produto_usuario]
    print(f"O preço do(a) {produto_usuario} é R${preco:.2f}.")
else:
    print(f"Produto '{produto_usuario}' não foi encontrado.")
