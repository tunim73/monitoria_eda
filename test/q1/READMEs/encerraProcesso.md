```cpp
void encerraProcesso()
{  
    if (VerificaListaVazia())
    {
        cout << "Lista de processos vazia";
    } 
    else {
      pro aux = topo;
      topo = topo->prox;
        if(topo == topo->prox){

            ultimo = NULL;
            topo = NULL;

            cout << "\n O ultimo processo: " << aux->num << " foi encerrado\n";
            cout << "\nAgora a lista de Processos Vazia\n";

            delete (aux);
        }
        else{

            ultimo->prox = topo;
            cout << "\n O processo: " << aux->num << " foi encerrado\n";

            delete (aux);
        }
      }
    
}
```