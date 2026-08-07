# NfeApi

Todas as URIs relativas a *https://prod.acbr.api.br*

| Método | Endpoint | Descrição |
|------------- | ------------- | -------------|
| [**baixarPdfCancelamentoNfe**](NfeApi.md#baixarPdfCancelamentoNfe) | **GET** /nfe/{id}/cancelamento/pdf | Baixar PDF do cancelamento |
| [**baixarPdfCartaCorrecaoNfe**](NfeApi.md#baixarPdfCartaCorrecaoNfe) | **GET** /nfe/{id}/carta-correcao/pdf | Baixar PDF da carta de correção |
| [**baixarPdfEventoNfe**](NfeApi.md#baixarPdfEventoNfe) | **GET** /nfe/eventos/{id}/pdf | Baixar PDF do evento |
| [**baixarPdfInutilizacaoNfe**](NfeApi.md#baixarPdfInutilizacaoNfe) | **GET** /nfe/inutilizacoes/{id}/pdf | Baixar PDF da inutilização |
| [**baixarPdfNfe**](NfeApi.md#baixarPdfNfe) | **GET** /nfe/{id}/pdf | Baixar PDF do DANFE |
| [**baixarPreviaPdfNfe**](NfeApi.md#baixarPreviaPdfNfe) | **POST** /nfe/previa/pdf | Prévia do PDF do DANFE |
| [**baixarPreviaXmlNfe**](NfeApi.md#baixarPreviaXmlNfe) | **POST** /nfe/previa/xml | Prévia do XML da NF-e |
| [**baixarXmlCancelamentoNfe**](NfeApi.md#baixarXmlCancelamentoNfe) | **GET** /nfe/{id}/cancelamento/xml | Baixar XML do cancelamento |
| [**baixarXmlCartaCorrecaoNfe**](NfeApi.md#baixarXmlCartaCorrecaoNfe) | **GET** /nfe/{id}/carta-correcao/xml | Baixar XML da carta de correção |
| [**baixarXmlEventoNfe**](NfeApi.md#baixarXmlEventoNfe) | **GET** /nfe/eventos/{id}/xml | Baixar XML do evento |
| [**baixarXmlInutilizacaoNfe**](NfeApi.md#baixarXmlInutilizacaoNfe) | **GET** /nfe/inutilizacoes/{id}/xml | Baixar XML da inutilização |
| [**baixarXmlNfe**](NfeApi.md#baixarXmlNfe) | **GET** /nfe/{id}/xml | Baixar XML da NF-e processada |
| [**baixarXmlNfeNota**](NfeApi.md#baixarXmlNfeNota) | **GET** /nfe/{id}/xml/nota | Baixar XML da NF-e |
| [**baixarXmlNfeProtocolo**](NfeApi.md#baixarXmlNfeProtocolo) | **GET** /nfe/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ |
| [**cancelarNfe**](NfeApi.md#cancelarNfe) | **POST** /nfe/{id}/cancelamento | Cancelar uma NF-e autorizada |
| [**consultarCancelamentoNfe**](NfeApi.md#consultarCancelamentoNfe) | **GET** /nfe/{id}/cancelamento | Consultar o cancelamento da NF-e |
| [**consultarCartaCorrecaoNfe**](NfeApi.md#consultarCartaCorrecaoNfe) | **GET** /nfe/{id}/carta-correcao | Consultar a solicitação de correção da NF-e |
| [**consultarContribuinteNfe**](NfeApi.md#consultarContribuinteNfe) | **GET** /nfe/cadastro-contribuinte | Consultar contribuinte |
| [**consultarEventoNfe**](NfeApi.md#consultarEventoNfe) | **GET** /nfe/eventos/{id} | Consultar evento |
| [**consultarInutilizacaoNfe**](NfeApi.md#consultarInutilizacaoNfe) | **GET** /nfe/inutilizacoes/{id} | Consultar a inutilização de sequência de numeração |
| [**consultarLoteNfe**](NfeApi.md#consultarLoteNfe) | **GET** /nfe/lotes/{id} | Consultar lote de NF-e |
| [**consultarNfe**](NfeApi.md#consultarNfe) | **GET** /nfe/{id} | Consultar NF-e |
| [**consultarStatusSefazNfe**](NfeApi.md#consultarStatusSefazNfe) | **GET** /nfe/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora |
| [**criarCartaCorrecaoNfe**](NfeApi.md#criarCartaCorrecaoNfe) | **POST** /nfe/{id}/carta-correcao | Solicitar correção da NF-e |
| [**emitirLoteNfe**](NfeApi.md#emitirLoteNfe) | **POST** /nfe/lotes | Emitir lote de NF-e |
| [**emitirNfe**](NfeApi.md#emitirNfe) | **POST** /nfe | Emitir NF-e |
| [**enviarEmailNfe**](NfeApi.md#enviarEmailNfe) | **POST** /nfe/{id}/email | Enviar e-mail |
| [**inutilizarNumeracaoNfe**](NfeApi.md#inutilizarNumeracaoNfe) | **POST** /nfe/inutilizacoes | Inutilizar uma sequência de numeração de NF-e |
| [**listarEventosNfe**](NfeApi.md#listarEventosNfe) | **GET** /nfe/eventos | Listar eventos |
| [**listarLotesNfe**](NfeApi.md#listarLotesNfe) | **GET** /nfe/lotes | Listar lotes de NF-e |
| [**listarNfe**](NfeApi.md#listarNfe) | **GET** /nfe | Listar NF-e |
| [**sincronizarNfe**](NfeApi.md#sincronizarNfe) | **POST** /nfe/{id}/sincronizar | Sincroniza dados na NF-e a partir da SEFAZ |


<a name="baixarPdfCancelamentoNfe"></a>
# **baixarPdfCancelamentoNfe**
> Blob baixarPdfCancelamentoNfe(id)

Baixar PDF do cancelamento

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NF-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarPdfCartaCorrecaoNfe"></a>
# **baixarPdfCartaCorrecaoNfe**
> Blob baixarPdfCartaCorrecaoNfe(id)

Baixar PDF da carta de correção

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NF-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarPdfEventoNfe"></a>
# **baixarPdfEventoNfe**
> Blob baixarPdfEventoNfe(id)

Baixar PDF do evento

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do evento gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarPdfInutilizacaoNfe"></a>
# **baixarPdfInutilizacaoNfe**
> Blob baixarPdfInutilizacaoNfe(id)

Baixar PDF da inutilização

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do evento gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarPdfNfe"></a>
# **baixarPdfNfe**
> Blob baixarPdfNfe(id, logotipo, nomeFantasia, formato, mensagemRodape, canhoto)

Baixar PDF do DANFE

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NF-e gerado pela API. | |
| **logotipo** | **boolean**| Imprime o documento com logotipo, desde que esteja cadastrado na empresa. | [opcional] |
| **nomeFantasia** | **boolean**| Exibe o nome fantasia do emitente, desde que esteja presente no XML da nota. | [opcional] |
| **formato** | **string**| Formato de impressão do DANFE.    Valores disponíveis:  - &#x60;padrao&#x60;: será utilizado o formato definido no XML da NF-e (tag \&quot;tpImp\&quot;);  - &#x60;retrato&#x60;: tamanho A4 em modo retrato;  - &#x60;paisagem&#x60;: tamanho A4 em modo paisagem;  - &#x60;simplificado&#x60;: formato simplificado utilizado nas operações realizadas fora do estabelecimento (Anexo II do MOC, item 3.11);  - &#x60;etiqueta&#x60;: formato simplificado utilizado nas operações em comércio eletrônico (Anexo II do MOC, item 3.12 e NT 2020.004). | [opcional] |
| **mensagemRodape** | **string**| Imprime mensagem no rodapé do documento.    O caractere &#x60;|&#x60; (pipe) poderá ser utilizado para definir a quantidade e o alinhamento das mensagens.    **Exemplos de Uso:**  * &#x60;\&quot;esquerda\&quot;&#x60;  * &#x60;\&quot;esquerda|centro\&quot;&#x60;  * &#x60;\&quot;esquerda|centro|direita\&quot;&#x60;  * &#x60;\&quot;|centro\&quot;&#x60;, &#x60;\&quot;|centro|\&quot;&#x60;  * &#x60;\&quot;|centro|direita\&quot;&#x60;  * &#x60;\&quot;||direita\&quot;&#x60;  * &#x60;\&quot;esquerda||direita\&quot;&#x60; | [opcional] |
| **canhoto** | **boolean**| Imprime o documento com o bloco de canhoto. | [opcional] |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarPreviaPdfNfe"></a>
# **baixarPreviaPdfNfe**
> Blob baixarPreviaPdfNfe(body, logotipo, nomeFantasia, formato, mensagemRodape, canhoto)

Prévia do PDF do DANFE

    Através desse endpoint, é possível enviar os dados de uma NF-e e gerar uma prévia do DANFE.    Os dados de entrada são os mesmos do endpoint de emissão de NF-e (&#x60;POST /nfe&#x60;).    **Atenção**: O DANFE gerado por este endpoint é apenas para fins de visualização e não possui valor fiscal. Para a emissão de uma NF-e com valor fiscal, utilize o processo de emissão padrão descrito na documentação.    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**NfePedidoEmissao**](../Models/NfePedidoEmissao.md)|  | |
| **logotipo** | **boolean**| Imprime o documento com logotipo, desde que esteja cadastrado na empresa. | [opcional] |
| **nomeFantasia** | **boolean**| Exibe o nome fantasia do emitente, desde que esteja presente no XML da nota. | [opcional] |
| **formato** | **string**| Formato de impressão do DANFE.    Valores disponíveis:  - &#x60;padrao&#x60;: será utilizado o formato definido no XML da NF-e (tag \&quot;tpImp\&quot;);  - &#x60;retrato&#x60;: tamanho A4 em modo retrato;  - &#x60;paisagem&#x60;: tamanho A4 em modo paisagem;  - &#x60;simplificado&#x60;: formato simplificado utilizado nas operações realizadas fora do estabelecimento (Anexo II do MOC, item 3.11);  - &#x60;etiqueta&#x60;: formato simplificado utilizado nas operações em comércio eletrônico (Anexo II do MOC, item 3.12 e NT 2020.004). | [opcional] |
| **mensagemRodape** | **string**| Imprime mensagem no rodapé do documento.    O caractere &#x60;|&#x60; (pipe) poderá ser utilizado para definir a quantidade e o alinhamento das mensagens.    **Exemplos de Uso:**  * &#x60;\&quot;esquerda\&quot;&#x60;  * &#x60;\&quot;esquerda|centro\&quot;&#x60;  * &#x60;\&quot;esquerda|centro|direita\&quot;&#x60;  * &#x60;\&quot;|centro\&quot;&#x60;, &#x60;\&quot;|centro|\&quot;&#x60;  * &#x60;\&quot;|centro|direita\&quot;&#x60;  * &#x60;\&quot;||direita\&quot;&#x60;  * &#x60;\&quot;esquerda||direita\&quot;&#x60; | [opcional] |
| **canhoto** | **boolean**| Imprime o documento com o bloco de canhoto. | [opcional] |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarPreviaXmlNfe"></a>
# **baixarPreviaXmlNfe**
> Blob baixarPreviaXmlNfe(body)

Prévia do XML da NF-e

    Através desse endpoint, é possível enviar os dados de uma NF-e e gerar uma prévia do XML, sem a assinatura digital.    Os dados de entrada são os mesmos do endpoint de emissão de NF-e (&#x60;POST /nfe&#x60;).    **Atenção**: O XML gerado por este endpoint é apenas para fins de visualização e não possui valor fiscal. Para a emissão de uma NF-e com valor fiscal, utilize o processo de emissão padrão descrito na documentação.    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**NfePedidoEmissao**](../Models/NfePedidoEmissao.md)|  | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlCancelamentoNfe"></a>
# **baixarXmlCancelamentoNfe**
> Blob baixarXmlCancelamentoNfe(id)

Baixar XML do cancelamento

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NF-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlCartaCorrecaoNfe"></a>
# **baixarXmlCartaCorrecaoNfe**
> Blob baixarXmlCartaCorrecaoNfe(id)

Baixar XML da carta de correção

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NF-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlEventoNfe"></a>
# **baixarXmlEventoNfe**
> Blob baixarXmlEventoNfe(id)

Baixar XML do evento

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do evento gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlInutilizacaoNfe"></a>
# **baixarXmlInutilizacaoNfe**
> Blob baixarXmlInutilizacaoNfe(id)

Baixar XML da inutilização

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do evento gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlNfe"></a>
# **baixarXmlNfe**
> Blob baixarXmlNfe(id)

Baixar XML da NF-e processada

    Utilize esse endpoint para obter o XML da nota enviado para a SEFAZ, complementado com a informação do protocolo de autorização ou denegação de uso (TAG raiz &#x60;nfeProc&#x60;).    O XML só estará disponível nesse endpoint caso a nota tenha sido autorizada ou denegada pela SEFAZ. Para obter o XML nos demais casos, utilize o endpoint &#x60;GET /nfe/{id}/xml/nota&#x60;.    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NF-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlNfeNota"></a>
# **baixarXmlNfeNota**
> Blob baixarXmlNfeNota(id)

Baixar XML da NF-e

    Utilize esse endpoint para obter o XML da nota enviado para a SEFAZ.    O XML estará disponível nesse endpoint mesmo em casos que a nota tenha sido rejeitada.    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NF-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlNfeProtocolo"></a>
# **baixarXmlNfeProtocolo**
> Blob baixarXmlNfeProtocolo(id)

Baixar XML do Protocolo da SEFAZ

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NF-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="cancelarNfe"></a>
# **cancelarNfe**
> DfeCancelamento cancelarNfe(id, body)

Cancelar uma NF-e autorizada

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NF-e gerado pela API. | |
| **body** | [**NfePedidoCancelamento**](../Models/NfePedidoCancelamento.md)|  | [opcional] |

### Tipo do retorno

[**DfeCancelamento**](../Models/DfeCancelamento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarCancelamentoNfe"></a>
# **consultarCancelamentoNfe**
> DfeCancelamento consultarCancelamentoNfe(id)

Consultar o cancelamento da NF-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NF-e gerado pela API. | |

### Tipo do retorno

[**DfeCancelamento**](../Models/DfeCancelamento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarCartaCorrecaoNfe"></a>
# **consultarCartaCorrecaoNfe**
> DfeCartaCorrecao consultarCartaCorrecaoNfe(id)

Consultar a solicitação de correção da NF-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NF-e gerado pela API. | |

### Tipo do retorno

[**DfeCartaCorrecao**](../Models/DfeCartaCorrecao.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarContribuinteNfe"></a>
# **consultarContribuinteNfe**
> DfeContribuinteInfCons consultarContribuinteNfe(cpfCnpj, argumento, documento, uf)

Consultar contribuinte

    Consulta o Cadastro Centralizado de Contribuintes (CCC) do ICMS da unidade federada.    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.    *Utilize o valor sem máscara*. | |
| **argumento** | **string**| Argumento de pesquisa.    Valores válidos:  * &#x60;CNPJ&#x60;  * &#x60;CPF&#x60;  * &#x60;IE&#x60; | |
| **documento** | **string**| Documento a ser consultado (CNPJ, CPF ou Inscrição Estadual). | |
| **uf** | **string**| Sigla da UF consultada.     Utilize &#x60;SU&#x60; para SUFRAMA.    *Caso não seja informada, será utilizada a UF da empresa.* | [opcional] |

### Tipo do retorno

[**DfeContribuinteInfCons**](../Models/DfeContribuinteInfCons.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarEventoNfe"></a>
# **consultarEventoNfe**
> DfeEvento consultarEventoNfe(id)

Consultar evento

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do evento gerado pela API. | |

### Tipo do retorno

[**DfeEvento**](../Models/DfeEvento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarInutilizacaoNfe"></a>
# **consultarInutilizacaoNfe**
> DfeInutilizacao consultarInutilizacaoNfe(id)

Consultar a inutilização de sequência de numeração

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do evento gerado pela API. | |

### Tipo do retorno

[**DfeInutilizacao**](../Models/DfeInutilizacao.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarLoteNfe"></a>
# **consultarLoteNfe**
> DfeLote consultarLoteNfe(id)

Consultar lote de NF-e

    Consulta os detalhes de um lote já existente. Forneça o ID único obtido de uma requisição de emissão ou de listagem de lotes e a API irá retornar as informações do lote correspondente.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do lote gerado pela API. | |

### Tipo do retorno

[**DfeLote**](../Models/DfeLote.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarNfe"></a>
# **consultarNfe**
> Dfe consultarNfe(id)

Consultar NF-e

    Consulta os detalhes de uma NF-e já existente. Forneça o ID único obtido de uma requisição de emissão ou de listagem de notas e a API irá retornar as informações da nota correspondente.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NF-e gerado pela API. | |

### Tipo do retorno

[**Dfe**](../Models/Dfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarStatusSefazNfe"></a>
# **consultarStatusSefazNfe**
> DfeSefazStatus consultarStatusSefazNfe(cpfCnpj, autorizador)

Consulta do Status do Serviço na SEFAZ Autorizadora

    Consulta do status do serviço prestado pelo Portal da Secretaria de Fazenda Estadual.    A API mantém a última consulta em cache por 5 minutos, evitando sobrecarregar desnecessariamente os servidores da SEFAZ (conforme orientação do MOC - versão 7.0, item 5.5.3). Dessa forma, você poderá chamar esse endpoint quantas vezes quiser, sem preocupar-se em ter o seu CNPJ bloqueado por consumo indevido (Rejeição 656).

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF/CNPJ do emitente.  Utilize o valor sem máscara. | |
| **autorizador** | **string**| Ambiente Autorizador.    Autorizadores disponíveis: &#x60;AM&#x60;, &#x60;BA&#x60;, &#x60;GO&#x60;, &#x60;MG&#x60;, &#x60;MS&#x60;, &#x60;MT&#x60;, &#x60;PE&#x60;, &#x60;PR&#x60;, &#x60;RS&#x60;, &#x60;SP&#x60;, &#x60;SVAN&#x60;, &#x60;SVRS&#x60;, &#x60;SVCAN&#x60;, &#x60;SVCRS&#x60;, &#x60;AN&#x60;.    *Caso não seja informado, será utilizado o ambiente autorizador da UF do emitente.* | [opcional] |

### Tipo do retorno

[**DfeSefazStatus**](../Models/DfeSefazStatus.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="criarCartaCorrecaoNfe"></a>
# **criarCartaCorrecaoNfe**
> DfeCartaCorrecao criarCartaCorrecaoNfe(id, body)

Solicitar correção da NF-e

    é possível enviar até 20 correções diferentes, sendo que será válido sempre a última correção enviada.    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NF-e gerado pela API. | |
| **body** | [**NfePedidoCartaCorrecao**](../Models/NfePedidoCartaCorrecao.md)| Contém os dados do pedido para carta de correção. | |

### Tipo do retorno

[**DfeCartaCorrecao**](../Models/DfeCartaCorrecao.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="emitirLoteNfe"></a>
# **emitirLoteNfe**
> DfeLote emitirLoteNfe(body)

Emitir lote de NF-e

    **Informações adicionais**:  - Consumo: 1 unidade por NF-e.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**NfePedidoEmissaoLote**](../Models/NfePedidoEmissaoLote.md)|  | |

### Tipo do retorno

[**DfeLote**](../Models/DfeLote.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="emitirNfe"></a>
# **emitirNfe**
> Dfe emitirNfe(body)

Emitir NF-e

    Este endpoint permite a emissão de Notas Fiscais Eletrônicas (NF-e).  A solicitação deve ser feita enviando os dados necessários para a  emissão de uma NF-e.     A estrutura do JSON utilizado na solicitação segue a hierarquia e  nomenclatura de campos definidos no &lt;a href&#x3D;\&quot;https://www.nfe.fazenda.gov.br/portal/principal.aspx\&quot; target&#x3D;\&quot;_blank\&quot;&gt;  Manual de Orientação ao Contribuinte (MOC)&lt;/a&gt;.  Esta conformidade visa facilitar a integração de novos usuários que já  possuem familiaridade com o padrão, além de permitir a resolução de  dúvidas diretamente no MOC, com um profissional de contabilidade  habilitado ou em outras fontes confiáveis que tratam do mesmo assunto.    **Comportamento Assíncrono**    A resposta desse endpoint inclui a propriedade *status* no JSON.  Caso o valor retornado seja *pendente*, significa que a solicitação está  sendo realizada de forma assíncrona pela API. Nesse caso, o usuário deverá  adotar um fluxo que consiste em requisitar periodicamente o endpoint  &lt;a href&#x3D;\&quot;#tag/Nfe/operation/ConsultarNfe\&quot;&gt;Consultar NF-e&lt;/a&gt; até que  seja retornado um status indicando o fim da emissão.    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**NfePedidoEmissao**](../Models/NfePedidoEmissao.md)|  | |

### Tipo do retorno

[**Dfe**](../Models/Dfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="enviarEmailNfe"></a>
# **enviarEmailNfe**
> EmailStatusResponse enviarEmailNfe(id, logotipo, nomeFantasia, formato, mensagemRodape, canhoto, body)

Enviar e-mail

    Envia o XML e PDF da nota via email.    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NF-e gerado pela API. | |
| **logotipo** | **boolean**| Imprime o documento com logotipo, desde que esteja cadastrado na empresa. | [opcional] |
| **nomeFantasia** | **boolean**| Exibe o nome fantasia do emitente, desde que esteja presente no XML da nota. | [opcional] |
| **formato** | **string**| Formato de impressão do DANFE.    Valores disponíveis:  - &#x60;padrao&#x60;: será utilizado o formato definido no XML da NF-e (tag \&quot;tpImp\&quot;);  - &#x60;retrato&#x60;: tamanho A4 em modo retrato;  - &#x60;paisagem&#x60;: tamanho A4 em modo paisagem;  - &#x60;simplificado&#x60;: formato simplificado utilizado nas operações realizadas fora do estabelecimento (Anexo II do MOC, item 3.11);  - &#x60;etiqueta&#x60;: formato simplificado utilizado nas operações em comércio eletrônico (Anexo II do MOC, item 3.12 e NT 2020.004). | [opcional] |
| **mensagemRodape** | **string**| Imprime mensagem no rodapé do documento.    O caractere &#x60;|&#x60; (pipe) poderá ser utilizado para definir a quantidade e o alinhamento das mensagens.    **Exemplos de Uso:**  * &#x60;\&quot;esquerda\&quot;&#x60;  * &#x60;\&quot;esquerda|centro\&quot;&#x60;  * &#x60;\&quot;esquerda|centro|direita\&quot;&#x60;  * &#x60;\&quot;|centro\&quot;&#x60;, &#x60;\&quot;|centro|\&quot;&#x60;  * &#x60;\&quot;|centro|direita\&quot;&#x60;  * &#x60;\&quot;||direita\&quot;&#x60;  * &#x60;\&quot;esquerda||direita\&quot;&#x60; | [opcional] |
| **canhoto** | **boolean**| Imprime o documento com o bloco de canhoto. | [opcional] |
| **body** | [**DfePedidoEnvioEmail**](../Models/DfePedidoEnvioEmail.md)|  | [opcional] |

### Tipo do retorno

[**EmailStatusResponse**](../Models/EmailStatusResponse.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="inutilizarNumeracaoNfe"></a>
# **inutilizarNumeracaoNfe**
> DfeInutilizacao inutilizarNumeracaoNfe(body)

Inutilizar uma sequência de numeração de NF-e

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**DfePedidoInutilizacao**](../Models/DfePedidoInutilizacao.md)|  | |

### Tipo do retorno

[**DfeInutilizacao**](../Models/DfeInutilizacao.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarEventosNfe"></a>
# **listarEventosNfe**
> DfeEventoListagem listarEventosNfe(dfeId, $top, $skip, $inlinecount)

Listar eventos

    Retorna a lista de eventos vinculados a um documento fiscal de acordo com os critérios de busca utilizados. Os eventos são retornados ordenados pela data da criação, com as mais recentes aparecendo primeiro.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **dfeId** | **string**| ID único gerado pela API para o documento fiscal. | |
| **$top** | **number**| Limite no número de objetos a serem retornados pela API, entre 1 e 100. | [opcional] |
| **$skip** | **number**| Quantidade de objetos que serão ignorados antes da lista começar a ser retornada. | [opcional] |
| **$inlinecount** | **boolean**| Inclui no JSON de resposta, na propriedade &#x60;@count&#x60;, o número total de registros que o filtro retornaria, independente dos filtros de paginação. | [opcional] |

### Tipo do retorno

[**DfeEventoListagem**](../Models/DfeEventoListagem.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarLotesNfe"></a>
# **listarLotesNfe**
> DfeLoteListagem listarLotesNfe(cpfCnpj, ambiente, $top, $skip, $inlinecount, referencia)

Listar lotes de NF-e

    Retorna a lista dos lotes de acordo com os critérios de busca utilizados. Os lotes são retornados ordenados pela data da criação, com os mais recentes aparecendo primeiro.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| Filtrar pelo CPF ou CNPJ do emitente.  Utilize o valor sem máscara. | |
| **ambiente** | **string**| Identificação do Ambiente.    Valores aceitos: homologacao, producao | |
| **$top** | **number**| Limite no número de objetos a serem retornados pela API, entre 1 e 100. | [opcional] |
| **$skip** | **number**| Quantidade de objetos que serão ignorados antes da lista começar a ser retornada. | [opcional] |
| **$inlinecount** | **boolean**| Inclui no JSON de resposta, na propriedade &#x60;@count&#x60;, o número total de registros que o filtro retornaria, independente dos filtros de paginação. | [opcional] |
| **referencia** | **string**|  | [opcional] |

### Tipo do retorno

[**DfeLoteListagem**](../Models/DfeLoteListagem.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarNfe"></a>
# **listarNfe**
> DfeListagem listarNfe(cpfCnpj, ambiente, $top, $skip, $inlinecount, referencia, chave, serie)

Listar NF-e

    Retorna a lista de notas de acordo com os critérios de busca utilizados. As notas são retornadas ordenadas pela data da criação, com as mais recentes aparecendo primeiro.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| Filtrar pelo CPF ou CNPJ do emitente.    Utilize o valor sem máscara. | |
| **ambiente** | **string**| Identificação do Ambiente.    Valores aceitos: homologacao, producao | |
| **$top** | **number**| Limite no número de objetos a serem retornados pela API, entre 1 e 100. | [opcional] |
| **$skip** | **number**| Quantidade de objetos que serão ignorados antes da lista começar a ser retornada. | [opcional] |
| **$inlinecount** | **boolean**| Inclui no JSON de resposta, na propriedade &#x60;@count&#x60;, o número total de registros que o filtro retornaria, independente dos filtros de paginação. | [opcional] |
| **referencia** | **string**| Seu identificador único para o documento. | [opcional] |
| **chave** | **string**| Chave de acesso do DF-e. | [opcional] |
| **serie** | **string**| Série do DF-e. | [opcional] |

### Tipo do retorno

[**DfeListagem**](../Models/DfeListagem.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="sincronizarNfe"></a>
# **sincronizarNfe**
> DfeSincronizacao sincronizarNfe(id)

Sincroniza dados na NF-e a partir da SEFAZ

    Realiza a sincronização dos dados a partir da consulta da situação atual da NF-e na Base de Dados do Portal da Secretaria de Fazenda Estadual.    **Cenários de uso**:  * Sincronizar uma nota que se encontra com o status &#x60;erro&#x60; na API, mas está autorizada na SEFAZ (útil em casos de erros de transmissão com a SEFAZ, como instabilidades e timeouts).  * Sincronizar uma nota que se encontra com o status &#x60;autorizado&#x60;na API, mas está cancelada na SEFAZ.  * Sincronizar todos os eventos de Cancelamento, Carta de Correção e EPEC de uma nota que porventura não tenham sido feitos a partir da API.    **Informações adicionais**:  - Consumo: 1 unidade por evento sincronizado ou requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NF-e gerado pela API. | |

### Tipo do retorno

[**DfeSincronizacao**](../Models/DfeSincronizacao.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

