# Respostas-do-Est-gio-Ribeir-o-Preto
1) def fibonacci(n):
    fib_sequence = [0, 1]
    
    # Gera a sequência de Fibonacci até o número n
    while True:
        next_value = fib_sequence[-1] + fib_sequence[-2]
        if next_value > n:
            break
        fib_sequence.append(next_value)
    
    return fib_sequence

def pertence_fibonacci(num):
    fib_sequence = fibonacci(num)
    
    if num in fib_sequence:
        return f"O número {num} pertence à sequência de Fibonacci."
    else:
        return f"O número {num} não pertence à sequência de Fibonacci."

# Solicita um número ao usuário
try:
    numero = int(input("Informe um número: "))
    print(pertence_fibonacci(numero))
except ValueError:
    print("Por favor, insira um número válido.")


2)def contar_a(s):
    # Conta quantas vezes 'a' ou 'A' aparecem na string
    contador = s.lower().count('a')
    return contador

def verificar_a(s):
    # Verifica se 'a' ou 'A' estão na string e retorna o resultado
    contador = contar_a(s)
    if contador > 0:
        return f"A letra 'a' aparece {contador} vez(es) na string."
    else:
        return "A letra 'a' não está presente na string."

# Entrada de string pelo usuário
string_usuario = input("Informe uma string: ")

# Verificação e resultado
resultado = verificar_a(string_usuario)
print(resultado)

# Exemplo de string previamente definida
string_predefinida = "A arte é uma forma de expressão."
resultado_predefinido = verificar_a(string_predefinida)
print(resultado_predefinido)

3) 77
4)
a)9
b)128
c)49
d)100
e)13
f)20

5) Lâmpada acesa: Interruptor B (que está ligado no momento).
Lâmpada apagada, mas quente: Interruptor A (que estava ligado antes, mas foi desligado).
Lâmpada apagada e fria: Interruptor C (que nunca foi ligado).
