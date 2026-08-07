# NfcomSefazProd

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **cProd** | **string** | Código do produto ou serviço. |  |
| **xProd** | **string** | Descrição do produto ou serviço. |  |
| **cClass** | **string** | Código de classificação.  Tabela de Classificação de Item da NFCom (validar por RV). |  |
| **CFOP** | **string** | CFOP.  Utilizar Tabela de CFOP. | [opcional]  |
| **CNPJLD** | **string** | CNPJ da operadora LD.  Informar o CNPJ da operadora LD que irá lançar o item de cofaturamento em nota do tipo faturamento 2. | [opcional]  |
| **uMed** | **number** | Unidade Básica de Medida.  * 1 - Minuto  * 2 - MB  * 3 - GB  * 4 - UN |  |
| **qFaturada** | **number** | Quantidade Faturada.  Informar a quantidade de comercialização do produto . |  |
| **vItem** | **number** | Valor unitário do item. |  |
| **vDesc** | **number** | Valor do Desconto. | [opcional]  |
| **vOutro** | **number** | Outras despesas acessórias. | [opcional]  |
| **vProd** | **number** | Valor total do item. |  |
| **dExpiracao** | **Date** | Data de expiração de crédito.  Formato AAAA-MM-DD. | [opcional]  |
| **indDevolucao** | **number** | Indicador de devolução do valor do item.  * 1 - Devolução do valor do item | [opcional]  |
| **CNPJCobrTerc** | **string** | CNPJ de cobrança de terceiro.  Informar quando cClass do grupo 110 - Cobrança de terceiros. | [opcional]  |
| **gPagAntecipado** | [**NfcomSefazGPagAntecipado**](NfcomSefazGPagAntecipado.md) |  | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

