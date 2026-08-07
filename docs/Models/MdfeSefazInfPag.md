# MdfeSefazInfPag

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **xNome** | **string** | Razão social ou Nome do respnsável pelo pagamento. | [opcional]  |
| **CPF** | **string** | Número do CPF do responsável pelo pgto.  Informar os zeros não significativos. | [opcional]  |
| **CNPJ** | **string** | Número do CNPJ do responsável pelo pgto.  Informar os zeros não significativos. | [opcional]  |
| **idEstrangeiro** | **string** | Identificador do responsável pelo pgto em caso de ser estrangeiro. | [opcional]  |
| **Comp** | [**Array**](MdfeSefazComp.md) |  |  |
| **vContrato** | **number** | Valor Total do Contrato. |  |
| **indAltoDesemp** | **number** | Indicador de operação de transporte de alto desempenho.  Operação de transporte com utilização de veículos de frotas dedicadas ou fidelizadas.  Preencher com “1” para indicar operação de transporte de alto desempenho, demais casos não informar a tag. | [opcional]  |
| **indPag** | **number** | Indicador da Forma de Pagamento:0-Pagamento à Vista  * 1 - Pagamento à Prazo |  |
| **vAdiant** | **number** | Valor do Adiantamento (usar apenas em pagamento à Prazo. | [opcional]  |
| **indAntecipaAdiant** | **number** | Indicador para declarar concordância em antecipar o adiantamento.  Informar a tag somente se for autorizado antecipar o adiantamento. | [opcional]  |
| **infPrazo** | [**Array**](MdfeSefazInfPrazo.md) |  | [opcional]  |
| **tpAntecip** | **number** | Tipo de Permissão em relação a antecipação das parcelas.  * 0 - Não permite antecipar  * 1 - Permite antecipar as parcelas  * 2 - Permite antecipar as parcelas mediante confirmação | [opcional]  |
| **infBanc** | [**MdfeSefazInfBanc**](MdfeSefazInfBanc.md) |  |  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

