```cpp
void incluiProcesso()
{

    pro pont = new process;
    int num = geraNumeroParaProcesso();

    pont->num = num;

    if (VerificaListaVazia())
    {
        topo = pont;
        ultimo = pont;
        pont->prox = topo;

    }
    else
    {
        
        pont->prox = topo;
        ultimo->prox = pont;
        ultimo=pont;

    }
}
```