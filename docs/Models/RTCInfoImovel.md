# RTCInfoImovel

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **cMun** | **string** | Código do município do endereço do imóvel (Tabela do IBGE).  *Disponível a partir da NT 009 (leiaute 009.1.01).* | [opcional]  |
| **gLocacao** | [**RTCLocacaoImovel**](RTCLocacaoImovel.md) |  | [opcional]  |
| **gUnidImob** | [**Array**](RTCUnidadesImobiliarias.md) |  | [opcional]  |
| **inscImobFisc** | **string** | &#x60;Deprecated&#x60;    **Propriedade depreciada** a partir da NT 009 (leiaute 009.1.01).    *Utilize &#x60;IBSCBS.imovel.gUnidImob[].inscImobFisc&#x60;*.  Inscrição imobiliária fiscal (código fornecido pela Prefeitura Municipal para a identificação da obra ou para fins de recolhimento do IPTU). | [opcional]  |
| **cCIB** | **string** | &#x60;Deprecated&#x60;    **Propriedade depreciada** a partir da NT 009 (leiaute 009.1.01).    *Utilize &#x60;IBSCBS.imovel.gUnidImob[].cCIB&#x60;*.  Código do Cadastro Imobiliário Brasileiro - CIB. | [opcional]  |
| **end** | [**EnderObraEvento**](EnderObraEvento.md) |  | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

