# Implementação de um Quicksort
def quicksort(lista):
    if len(lista) < 2:
        return lista
    else:
        pivo = lista[len(lista)//2]
        menores = [i for i in lista[:len(lista)//2] + lista[len(lista)//2+1:] if i <= pivo]
        maiores = [i for i in lista[:len(lista)//2] + lista[len(lista)//2+1:] if i > pivo]
        return quicksort(menores) + [pivo] + quicksort(maiores)

print(quicksort([3,2,7,32,27,1,9,10,78]))
