# NfeSefazEmit

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **CNPJ** | **string** | Número do CNPJ do emitente.    ***Obrigatório caso o emitente seja pessoa jurídica***. | [opcional]  |
| **CPF** | **string** | Número do CPF do emitente.    ***Obrigatório caso o emitente seja pessoa física***. | [opcional]  |
| **xNome** | **string** | Razão Social ou Nome do emitente.    *Caso não seja informado, será utilizado o do cadastro da empresa.* | [opcional]  |
| **xFant** | **string** | Nome fantasia.    *Caso não seja informado, será utilizado o do cadastro da empresa.* | [opcional]  |
| **enderEmit** | [**NfeSefazEnderEmi**](NfeSefazEnderEmi.md) |  | [opcional]  |
| **IE** | **string** | Inscrição Estadual do Emitente.    *Caso não seja informado, será utilizado o do cadastro da empresa.* | [opcional]  |
| **IEST** | **string** | Inscricao Estadual do Substituto Tributário.    *Caso não seja informado, será utilizado o do cadastro da empresa.* | [opcional]  |
| **IM** | **string** | Inscrição Municipal.    *Caso não seja informado, será utilizado o do cadastro da empresa.* | [opcional]  |
| **CNAE** | **string** | CNAE Fiscal.    *Caso não seja informado, será utilizado o do cadastro da empresa.* | [opcional]  |
| **CRT** | **number** | Código de Regime Tributário.  Este campo será obrigatoriamente preenchido com:  * 1 - Simples Nacional  * 2 - Simples Nacional - excesso de sublimite de receita bruta  * 3 - Regime Normal  * 4 - Simples Nacional - Microempreendedor individual - MEI    *Caso não seja informado, será utilizado o do cadastro da empresa.* | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

