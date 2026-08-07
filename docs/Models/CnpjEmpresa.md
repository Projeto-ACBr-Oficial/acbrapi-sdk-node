# CnpjEmpresa

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **cnpj** | **string** | Número de inscrição do CNPJ. | [opcional]  |
| **razao\_social** | **string** | Nome empresarial da pessoa jurídica. | [opcional]  |
| **nome\_fantasia** | **string** | Corresponde ao nome fantasia. | [opcional]  |
| **data\_inicio\_atividade** | **Date** | Data de início da atividade. | [opcional]  |
| **matriz** | **boolean** | Indicador de matriz/filial:  * &#x60;true&#x60; - É matriz  * &#x60;false&#x60; - É filial | [opcional]  |
| **natureza\_juridica** | [**CnpjNaturezaJuridica**](CnpjNaturezaJuridica.md) |  | [opcional]  |
| **capital\_social** | **number** | Capital social da empresa. | [opcional]  |
| **porte** | [**CnpjPorteEmpresa**](CnpjPorteEmpresa.md) |  | [opcional]  |
| **ente\_federativo\_responsavel** | **string** | O ente federativo responsável é preenchido para os casos de órgãos e  entidades do grupo de natureza jurídica 1XXX. Para as demais naturezas,  este atributo fica em branco. | [opcional]  |
| **situacao\_cadastral** | [**CnpjSituacaoCadastral**](CnpjSituacaoCadastral.md) |  | [opcional]  |
| **motivo\_situacao\_cadastral** | [**CnpjMotivoSituacaoCadastral**](CnpjMotivoSituacaoCadastral.md) |  | [opcional]  |
| **nome\_da\_cidade\_no\_exterior** | **string** | Nome da cidade no exterior. | [opcional]  |
| **pais** | [**CnpjPais**](CnpjPais.md) |  | [opcional]  |
| **atividade\_principal** | [**CnpjCnae**](CnpjCnae.md) |  | [opcional]  |
| **atividades\_secundarias** | [**Array**](CnpjCnaeSecundario.md) |  | [opcional]  |
| **endereco** | [**CnpjEndereco**](CnpjEndereco.md) |  | [opcional]  |
| **telefones** | [**Array**](CnpjTelefone.md) |  | [opcional]  |
| **email** | **string** | E-mail do contribuinte. | [opcional]  |
| **situacao\_especial** | [**CnpjSituacaoEspecial**](CnpjSituacaoEspecial.md) |  | [opcional]  |
| **simples** | [**CnpjOpcaoSimples**](CnpjOpcaoSimples.md) |  | [opcional]  |
| **simei** | [**CnpjOpcaoSimei**](CnpjOpcaoSimei.md) |  | [opcional]  |
| **socios** | [**Array**](CnpjSocio.md) |  | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

