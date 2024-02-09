```cpp
void imprimirProcessos()
{
    if (VerificaListaVazia())
        cout << "\n Lista de processos vazia\n";

    else
    {
        pro aux = topo;

        do{
            cout << aux->num << "\t";
            aux = aux->prox;

        } while ((aux != topo));
        
    }
 
    cout << endl;
}
```