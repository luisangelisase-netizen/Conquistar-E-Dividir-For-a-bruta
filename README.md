# Conquistar-E-Dividir-For-a-bruta


Q4 ( Força bruta )
_________________________________________
dna = input()
procurada = input()

encontrada = False

for i in range(len(dna) - len(procurada) + 1):
    j = 0

    while j < len(procurada) and dna[i + j] == procurada[j]:
        j += 1

    if j == len(procurada):
        print("Sequência encontrada na posição", i + 1)
        encontrada = True
        break

if not encontrada:
    print("Sequência não encontrada")

__________________________________________________

Q3 ( DIvidir para COnquistar )


def mdc(L, A):
    if A == 0:
        return L
    return mdc(A, L % A)

L = int(input("L =  "))
A = int(input("A = "))

print(mdc(L, A))
  
