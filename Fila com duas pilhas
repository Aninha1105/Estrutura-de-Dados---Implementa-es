# Implementação de uma fila a partir de duas pilhas

class Stack:
    
    def __init__(self):
        self.items = []
        
    def isEmpty(self):
        return self.items == []  #vê se a pilha está vazia
    
    def push(self,item):
        self.items.append(item)  #adiciona um item ao final da pilha
    
    def pop(self):
        return self.items.pop()  #remove o último item da pilha
    
    def peek(self):
        return self.items[-1]    #mostra o último item da pilha
    
    def size(self):
        return len(self.items)   #retorna o tamanho da pilha
    
class Fila_comPilhas:
    
    def __init__(self):
        self.pilha1 = Stack() #ordem normal
        self.pilha2 = Stack() #ordem invertida
        
    def enqueue (self, item):
        while not self.pilha2.isEmpty():          #se a pilha2 não estiver vazia 
            self.pilha1.push(self.pilha2.pop())   #reverte a pilha2(fila) para pilha1
        self.pilha1.push(item)
            
    def dequeue (self):
        while not self.pilha1.isEmpty():          #se a pilha1 não estiver vazia
            self.pilha2.push(self.pilha1.pop())   #reverte a pilha1 para a pilha2(fila)
        return self.pilha2.pop()

    def imprime(self):
        print(fila.dequeue())
        while not self.pilha2.isEmpty():
            print(self.pilha2.pop())

#enqueue = adiciona um item no final da fila
#dequeue = retorna o item do início da fila. Caso a pilha esteja vazia retorna None
#imprime = imprime todos os itens da fila em ordem (do início para o fim)
