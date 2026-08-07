# NfeSefazICMS51

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **orig** | **number** | Origem da mercadoria:  * 0 - Nacional, exceto as indicadas nos códigos 3, 4, 5 e 8;  * 1 - Estrangeira - Importação direta, exceto a indicada no código 6;  * 2 - Estrangeira - Adquirida no mercado interno, exceto a indicada no código 7;  * 3 - Nacional, mercadoria ou bem com Conteúdo de Importação superior a 40%% e inferior ou igual a 70%%;  * 4 - Nacional, cuja produção tenha sido feita em conformidade com os processos produtivos básicos de que tratam as legislações citadas nos Ajustes;  * 5 - Nacional, mercadoria ou bem com Conteúdo de Importação inferior ou igual a 40%%;  * 6 - Estrangeira - Importação direta, sem similar nacional, constante em lista da CAMEX e gás natural;  * 7 - Estrangeira - Adquirida no mercado interno, sem similar nacional, constante lista CAMEX e gás natural;  * 8 - Nacional, mercadoria ou bem com Conteúdo de Importação superior a 70%%. |  |
| **CST** | **string** | Tributação pelo ICMS 51 - Tributação com Diferimento. |  |
| **modBC** | **number** | Modalidade de determinação da BC do ICMS:  * 0 - Margem Valor Agregado (%%)  * 1 - Pauta (valor)  * 2 - Preço Tabelado Máximo (valor)  * 3 - Valor da Operação | [opcional]  |
| **pRedBC** | **number** | Percentual de redução da BC. | [opcional]  |
| **cBenefRBC** | **string** | Código de Benefício Fiscal na UF aplicado ao item quando houver RBC. | [opcional]  |
| **vBC** | **number** | Valor da BC do ICMS. | [opcional]  |
| **pICMS** | **number** | Alíquota do imposto. | [opcional]  |
| **vICMSOp** | **number** | Valor do ICMS da Operação. | [opcional]  |
| **pDif** | **number** | Percentual do diferemento. | [opcional]  |
| **vICMSDif** | **number** | Valor do ICMS da diferido. | [opcional]  |
| **vICMS** | **number** | Valor do ICMS. | [opcional]  |
| **vBCFCP** | **number** | Valor da Base de cálculo do FCP. | [opcional]  |
| **pFCP** | **number** | Percentual de ICMS relativo ao Fundo de Combate à Pobreza (FCP). | [opcional]  |
| **vFCP** | **number** | Valor do ICMS relativo ao Fundo de Combate à Pobreza (FCP). | [opcional]  |
| **pFCPDif** | **number** | Percentual do diferimento do ICMS relativo ao Fundo de Combate à Pobreza (FCP). | [opcional]  |
| **vFCPDif** | **number** | Valor do ICMS relativo ao Fundo de Combate à Pobreza (FCP) diferido. | [opcional]  |
| **vFCPEfet** | **number** | Valor efetivo do ICMS relativo ao Fundo de Combate à Pobreza (FCP). | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

