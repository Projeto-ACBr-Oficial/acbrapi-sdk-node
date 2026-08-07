# CteSefazDest

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **CNPJ** | **string** | Número do CNPJ.  Em caso de empresa não estabelecida no Brasil, será informado o CNPJ com zeros.  Informar os zeros não significativos. | [opcional]  |
| **CPF** | **string** | Número do CPF.  Informar os zeros não significativos. | [opcional]  |
| **IE** | **string** | Inscrição Estadual.  Informar a IE do destinatário ou ISENTO se destinatário é contribuinte do ICMS isento de inscrição no cadastro de contribuintes do ICMS. Caso o destinatário não seja contribuinte do ICMS não informar o conteúdo. | [opcional]  |
| **xNome** | **string** | Razão Social ou Nome do destinatário. |  |
| **fone** | **string** | Telefone. | [opcional]  |
| **ISUF** | **string** | Inscrição na SUFRAMA.  (Obrigatório nas operações com as áreas com benefícios de incentivos fiscais sob controle da SUFRAMA). | [opcional]  |
| **enderDest** | [**CteSefazEndereco**](CteSefazEndereco.md) |  |  |
| **email** | **string** | Endereço de email. | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

