# CteSimpSefazTomaSimp

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **toma** | **number** | Tomador do Serviço.  Preencher com:  * 0 - Remetente  * 1 - Expedidor  * 2 - Recebedor  * 3 - Destinatário  * 4 - Terceiro |  |
| **indIEToma** | **number** | Indicador do papel do tomador na prestação do serviço:  * 1 - Contribuinte ICMS  * 2 - Contribuinte isento de inscrição  * 9 - Não Contribuinte  Aplica-se ao tomador que for indicado no toma. |  |
| **CNPJ** | **string** | Número do CNPJ.  Em caso de empresa não estabelecida no Brasil, será informado o CNPJ com zeros.  Informar os zeros não significativos. | [opcional]  |
| **CPF** | **string** | Número do CPF.  Informar os zeros não significativos. | [opcional]  |
| **IE** | **string** | Inscrição Estadual.  Informar a IE do tomador ou ISENTO se tomador é contribuinte do ICMS isento de inscrição no cadastro de contribuintes do ICMS. Caso o tomador não seja contribuinte do ICMS não informar o conteúdo. | [opcional]  |
| **xNome** | **string** | Razão Social ou Nome. |  |
| **ISUF** | **string** | Inscrição na SUFRAMA.  (Obrigatório nas operações com as áreas com benefícios de incentivos fiscais sob controle da SUFRAMA). | [opcional]  |
| **fone** | **string** | Telefone. | [opcional]  |
| **enderToma** | [**CteSimpSefazEnderecoSimp**](CteSimpSefazEnderecoSimp.md) |  |  |
| **email** | **string** | Endereço de email. | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

