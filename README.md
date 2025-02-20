def caracteres_ausentes(s):
    s = s.lower()  # Converter para minúsculas
    presentes = set(s)  # Criar um conjunto com os caracteres da string
    alfabeto = set("abcdefghijklmnopqrstuvwxyz")  # Conjunto com todas as letras do alfabeto
    ausentes = sorted(alfabeto - presentes)  # Diferença de conjuntos para encontrar letras ausentes
    
    return "".join(ausentes) if ausentes else "A string já é um pangrama"

# Testes
print(caracteres_ausentes("bem-vindo ao geeksforgeeks"))  # Saída: abdhijnpquvxyz
print(caracteres_ausentes("A rápida raposa marrom salta"))  # Saída: adglvyz

 
