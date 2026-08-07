# DistribuicaoNfePedido

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **cpf\_cnpj** | **string** | CPF ou CNPJ da empresa.    *Utilize o valor sem máscara*. |  |
| **ambiente** | **string** | Identificação do Ambiente. |  |
| **uf\_autor** | **string** | Sigla da UF do autor. | [opcional]  |
| **tipo\_consulta** | **string** | Tipo de consulta.   Valores possíveis: * &#x60;dist-nsu&#x60; - Consulta pelo último NSU recebido. * &#x60;cons-nsu&#x60; - Consulta por um NSU específico. * &#x60;cons-chave&#x60; - Consulta pela chave de acesso da NF-e. |  |
| **dist\_nsu** | **number** | Distribuição de conjunto de DF-e a partir do NSU informado.    *Obrigatório quando \&quot;tipo_consulta\&quot; for \&quot;dist-nsu\&quot;.* | [opcional]  |
| **cons\_nsu** | **number** | Consulta DF-e vinculado ao NSU informado.    *Obrigatório quando \&quot;tipo_consulta\&quot; for \&quot;cons-nsu\&quot;.* | [opcional]  |
| **cons\_chave** | **string** | Consulta de NF-e por chave de acesso informada.    *Obrigatório quando \&quot;tipo_consulta\&quot; for \&quot;cons-chave\&quot;.* | [opcional]  |
| **ignorar\_tempo\_espera** | **boolean** | Deve ser utilizado em situações em que o cliente  deseja ignorar o intervalo mínimo de 1 hora entre pedidos de distribuição  de NF-e. Quando habilitado, o cliente reconhece os riscos associados,  incluindo o bloqueio do CNPJ no Ambiente Nacional da SEFAZ, caso seja  caracterizado consumo indevido.    Valores:  * &#x60;false&#x60;: Respeita a regra de intervalo mínimo de 1 hora entre consultas    quando não há mais documentos disponíveis.    * &#x60;true&#x60;: Ignora o tempo de espera e força a requisição. | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

