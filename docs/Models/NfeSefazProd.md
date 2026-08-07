# NfeSefazProd

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **cProd** | **string** | Código do produto ou serviço. Preencher com CFOP caso se trate de itens não relacionados com mercadorias/produto e que o contribuinte não possua codificação própria  Formato ”CFOP9999”. |  |
| **cEAN** | **string** | GTIN (Global Trade Item Number) do produto, antigo código EAN ou código de barras. |  |
| **cBarra** | **string** | Codigo de barras diferente do padrão GTIN. | [opcional]  |
| **xProd** | **string** | Descrição do produto ou serviço. |  |
| **NCM** | **string** | Código NCM (8 posições), será permitida a informação do gênero (posição do capítulo do NCM) quando a operação não for de comércio exterior (importação/exportação) ou o produto não seja tributado pelo IPI. Em caso de item de serviço ou item que não tenham produto (Ex. transferência de crédito, crédito do ativo imobilizado, etc.), informar o código 00 (zeros) (v2.0). |  |
| **NVE** | **Array** | Nomenclatura de Valor aduaneio e Estatístico. | [opcional]  |
| **CEST** | **string** | Codigo especificador da Substuicao Tributaria - CEST, que identifica a mercadoria sujeita aos regimes de  substituicao tributária e de antecipação do recolhimento  do imposto. | [opcional]  |
| **indEscala** | **string** |  | [opcional]  |
| **CNPJFab** | **string** | CNPJ do Fabricante da Mercadoria, obrigatório para produto em escala NÃO relevante. | [opcional]  |
| **cBenef** | **string** |  | [opcional]  |
| **gCred** | [**Array**](NfeSefazGCred.md) |  | [opcional]  |
| **tpCredPresIBSZFM** | **number** | Classificação para subapuração do IBS na ZFM. | [opcional]  |
| **EXTIPI** | **string** | Código EX TIPI (3 posições). | [opcional]  |
| **CFOP** | **string** | Cfop. |  |
| **uCom** | **string** | Unidade comercial. |  |
| **qCom** | **number** | Quantidade Comercial  do produto, alterado para aceitar de 0 a 4 casas decimais e 11 inteiros. |  |
| **vUnCom** | **number** | Valor unitário de comercialização  - alterado para aceitar 0 a 10 casas decimais e 11 inteiros. |  |
| **vProd** | **number** | Valor bruto do produto ou serviço. |  |
| **cEANTrib** | **string** | GTIN (Global Trade Item Number) da unidade tributável, antigo código EAN ou código de barras. |  |
| **cBarraTrib** | **string** | Código de barras da unidade tributável diferente do padrão GTIN. | [opcional]  |
| **uTrib** | **string** | Unidade Tributável. |  |
| **qTrib** | **number** | Quantidade Tributável - alterado para aceitar de 0 a 4 casas decimais e 11 inteiros. |  |
| **vUnTrib** | **number** | Valor unitário de tributação - alterado para aceitar 0 a 10 casas decimais e 11 inteiros. |  |
| **vFrete** | **number** | Valor Total do Frete. | [opcional]  |
| **vSeg** | **number** | Valor Total do Seguro. | [opcional]  |
| **vDesc** | **number** | Valor do Desconto. | [opcional]  |
| **vOutro** | **number** | Outras despesas acessórias. | [opcional]  |
| **indTot** | **number** | Este campo deverá ser preenchido com:  * 0 - o valor do item (vProd) não compõe o valor total da NF-e (vProd)  * 1 - o valor do item (vProd) compõe o valor total da NF-e (vProd) |  |
| **indBemMovelUsado** | **number** | Indicador de fornecimento de bem móvel usado: 1-Bem Móvel Usado. | [opcional]  |
| **DI** | [**Array**](NfeSefazDI.md) |  | [opcional]  |
| **detExport** | [**Array**](NfeSefazDetExport.md) |  | [opcional]  |
| **xPed** | **string** | pedido de compra - Informação de interesse do emissor para controle do B2B. | [opcional]  |
| **nItemPed** | **number** | Número do Item do Pedido de Compra - Identificação do número do item do pedido de Compra. | [opcional]  |
| **nFCI** | **string** | Número de controle da FCI - Ficha de Conteúdo de Importação. | [opcional]  |
| **rastro** | [**Array**](NfeSefazRastro.md) |  | [opcional]  |
| **infProdNFF** | [**NfeSefazInfProdNFF**](NfeSefazInfProdNFF.md) |  | [opcional]  |
| **infProdEmb** | [**NfeSefazInfProdEmb**](NfeSefazInfProdEmb.md) |  | [opcional]  |
| **veicProd** | [**NfeSefazVeicProd**](NfeSefazVeicProd.md) |  | [opcional]  |
| **med** | [**NfeSefazMed**](NfeSefazMed.md) |  | [opcional]  |
| **arma** | [**Array**](NfeSefazArma.md) |  | [opcional]  |
| **comb** | [**NfeSefazComb**](NfeSefazComb.md) |  | [opcional]  |
| **nRECOPI** | **string** | Número do RECOPI. | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

