# NfceApi

Todas as URIs relativas a *https://prod.acbr.api.br*

| Método | Endpoint | Descrição |
|------------- | ------------- | -------------|
| [**baixarEscPosNfce**](NfceApi.md#baixarEscPosNfce) | **GET** /nfce/{id}/escpos | Comandos ESC/POS para impressão do DANFCE |
| [**baixarPdfCancelamentoNfce**](NfceApi.md#baixarPdfCancelamentoNfce) | **GET** /nfce/{id}/cancelamento/pdf | Baixar PDF do cancelamento |
| [**baixarPdfEventoNfce**](NfceApi.md#baixarPdfEventoNfce) | **GET** /nfce/eventos/{id}/pdf | Baixar PDF do evento |
| [**baixarPdfInutilizacaoNfce**](NfceApi.md#baixarPdfInutilizacaoNfce) | **GET** /nfce/inutilizacoes/{id}/pdf | Baixar PDF da inutilização |
| [**baixarPdfNfce**](NfceApi.md#baixarPdfNfce) | **GET** /nfce/{id}/pdf | Baixar PDF do DANFCE |
| [**baixarPreviaPdfNfce**](NfceApi.md#baixarPreviaPdfNfce) | **POST** /nfce/previa/pdf | Prévia do PDF do DANFCE |
| [**baixarPreviaXmlNfce**](NfceApi.md#baixarPreviaXmlNfce) | **POST** /nfce/previa/xml | Prévia do XML da NFC-e |
| [**baixarXmlCancelamentoNfce**](NfceApi.md#baixarXmlCancelamentoNfce) | **GET** /nfce/{id}/cancelamento/xml | Baixar XML do cancelamento |
| [**baixarXmlEventoNfce**](NfceApi.md#baixarXmlEventoNfce) | **GET** /nfce/eventos/{id}/xml | Baixar XML do evento |
| [**baixarXmlInutilizacaoNfce**](NfceApi.md#baixarXmlInutilizacaoNfce) | **GET** /nfce/inutilizacoes/{id}/xml | Baixar XML da inutilização |
| [**baixarXmlNfce**](NfceApi.md#baixarXmlNfce) | **GET** /nfce/{id}/xml | Baixar XML da NFC-e processada |
| [**baixarXmlNfceNota**](NfceApi.md#baixarXmlNfceNota) | **GET** /nfce/{id}/xml/nota | Baixar XML da NFC-e |
| [**baixarXmlNfceProtocolo**](NfceApi.md#baixarXmlNfceProtocolo) | **GET** /nfce/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ |
| [**cancelarNfce**](NfceApi.md#cancelarNfce) | **POST** /nfce/{id}/cancelamento | Cancelar uma NFC-e autorizada |
| [**consultarCancelamentoNfce**](NfceApi.md#consultarCancelamentoNfce) | **GET** /nfce/{id}/cancelamento | Consultar o cancelamento da NFC-e |
| [**consultarEventoNfce**](NfceApi.md#consultarEventoNfce) | **GET** /nfce/eventos/{id} | Consultar evento |
| [**consultarInutilizacaoNfce**](NfceApi.md#consultarInutilizacaoNfce) | **GET** /nfce/inutilizacoes/{id} | Consultar a inutilização de sequência de numeração |
| [**consultarLoteNfce**](NfceApi.md#consultarLoteNfce) | **GET** /nfce/lotes/{id} | Consultar lote de NFC-e |
| [**consultarNfce**](NfceApi.md#consultarNfce) | **GET** /nfce/{id} | Consultar NFC-e |
| [**consultarStatusSefazNfce**](NfceApi.md#consultarStatusSefazNfce) | **GET** /nfce/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora |
| [**emitirLoteNfce**](NfceApi.md#emitirLoteNfce) | **POST** /nfce/lotes | Emitir lote de NFC-e |
| [**emitirNfce**](NfceApi.md#emitirNfce) | **POST** /nfce | Emitir NFC-e |
| [**enviarEmailNfce**](NfceApi.md#enviarEmailNfce) | **POST** /nfce/{id}/email | Enviar e-mail |
| [**inutilizarNumeracaoNfce**](NfceApi.md#inutilizarNumeracaoNfce) | **POST** /nfce/inutilizacoes | Inutilizar uma sequência de numeração de NFC-e |
| [**listarEventosNfce**](NfceApi.md#listarEventosNfce) | **GET** /nfce/eventos | Listar eventos |
| [**listarLotesNfce**](NfceApi.md#listarLotesNfce) | **GET** /nfce/lotes | Listar lotes de NFC-e |
| [**listarNfce**](NfceApi.md#listarNfce) | **GET** /nfce | Listar NFC-e |
| [**sincronizarNfce**](NfceApi.md#sincronizarNfce) | **POST** /nfce/{id}/sincronizar | Sincroniza dados na NFC-e a partir da SEFAZ |


<a name="baixarEscPosNfce"></a>
# **baixarEscPosNfce**
> Blob baixarEscPosNfce(id, modelo, colunas, qrcodeLateral)

Comandos ESC/POS para impressão do DANFCE

    ESC/POS é um sistema de comando criado pela Epson usado em diversos sistemas de impressoras POS.    Com o formato ESC/POS, você poderá imprimir nativamente em uma vasta quantidade de modelos de impressora térmicas utilizadas no Brasil e no mundo. Com ela, você consegue fazer o envio de comandos em ESC/POS direto para a porta da impressora.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFC-e gerado pela API. | |
| **modelo** | **number**| Modelo da impressora:  * &#x60;0&#x60; - Texto  * &#x60;1&#x60; - Epson  * &#x60;2&#x60; - Bematech  * &#x60;3&#x60; - Daruma  * &#x60;4&#x60; - Vox  * &#x60;5&#x60; - Diebold  * &#x60;6&#x60; - Epson P2  * &#x60;7&#x60; - CustomPos  * &#x60;8&#x60; - Star  * &#x60;9&#x60; - Zjiang  * &#x60;10&#x60; - GPrinter  * &#x60;11&#x60; - Datecs  * &#x60;12&#x60; - Sunmi  * &#x60;13&#x60; - Externo | [opcional] |
| **colunas** | **number**| Define o máximo de caracteres, em uma linha, usando a fonte normal.    Ex: 40, 42, 48, 58, 80. | [opcional] |
| **qrcodeLateral** | **boolean**| Imprime o QRCode na lateral do DANFCe.    OBS: não suportado por alguns modelos de impressora. | [opcional] |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarPdfCancelamentoNfce"></a>
# **baixarPdfCancelamentoNfce**
> Blob baixarPdfCancelamentoNfce(id)

Baixar PDF do cancelamento

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFC-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarPdfEventoNfce"></a>
# **baixarPdfEventoNfce**
> Blob baixarPdfEventoNfce(id)

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

<a name="baixarPdfInutilizacaoNfce"></a>
# **baixarPdfInutilizacaoNfce**
> Blob baixarPdfInutilizacaoNfce(id)

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

<a name="baixarPdfNfce"></a>
# **baixarPdfNfce**
> Blob baixarPdfNfce(id, logotipo, nomeFantasia, mensagemRodape, resumido, qrcodeLateral, largura, margem)

Baixar PDF do DANFCE

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFC-e gerado pela API. | |
| **logotipo** | **boolean**| Imprime o documento com logotipo, desde que esteja cadastrado na empresa. | [opcional] |
| **nomeFantasia** | **boolean**| Exibe o nome fantasia do emitente, desde que esteja presente no XML da nota. | [opcional] |
| **mensagemRodape** | **string**| Imprime mensagem no rodapé do documento.    O caractere &#x60;|&#x60; (pipe) poderá ser utilizado para definir a quantidade e o alinhamento das mensagens.    **Exemplos de Uso:**  * &#x60;\&quot;esquerda\&quot;&#x60;  * &#x60;\&quot;esquerda|centro\&quot;&#x60;  * &#x60;\&quot;esquerda|centro|direita\&quot;&#x60;  * &#x60;\&quot;|centro\&quot;&#x60;, &#x60;\&quot;|centro|\&quot;&#x60;  * &#x60;\&quot;|centro|direita\&quot;&#x60;  * &#x60;\&quot;||direita\&quot;&#x60;  * &#x60;\&quot;esquerda||direita\&quot;&#x60; | [opcional] |
| **resumido** | **boolean**| Poderá ser impresso apenas o DANFE NFC-e resumido ou ecológico, sem o detalhamento dos itens da venda, desde que a Unidade Federada permita esta opção em sua legislação e o consumidor assim o solicite. | [opcional] |
| **qrcodeLateral** | **boolean**| Imprime o QRCode na lateral do DANFE NFC-e.    *Disponível apenas para DANFE com 80 milímetros de largura*. | [opcional] |
| **largura** | **number**| Largura do DANFE NFC-e (em milímetros). | [opcional] |
| **margem** | **string**| Define as margens do DANFE NFC-e (em milímetros).    Essa propriedade pode ser especificada usando um, dois, três ou quatro valores (separados por vírgulas). Cada valor deve ser um número entre &#x60;0&#x60; e &#x60;9&#x60;.  * Quando **um** valor é especificado, a mesma margem é aplicada para **todos os quatro lados**.  * Quando **dois** valores são especificados, a primeira margem é aplicada aos **lados esquerdo e direito**, e a segunda aos **lados superior e inferior**.  * Quando **três** valores são especificados, a primeira margem é aplicada ao **lado esquerdo**, a segunda aos **lados superior e inferior**, e a terceira ao **lado direito**.  * Quando **quatro** valores são especificados, as margens são aplicadas aos lados **esquerdo**, **superior**, **direito** e **inferior**, nesta ordem (sentido horário).    **Exemplos de uso**:  * &#x60;margem&#x3D;1&#x60;    - Margem esquerda: 1mm    - Margem superior: 1mm    - Margem direita: 1mm    - Margem inferior: 1mm  * &#x60;margem&#x3D;1,2&#x60;    - Margem esquerda: 1mm    - Margem superior: 2mm    - Margem direita: 1mm    - Margem inferior: 2mm  * &#x60;margem&#x3D;1,2,3&#x60;    - Margem esquerda: 1mm    - Margem superior: 2mm    - Margem direita: 3mm    - Margem inferior: 2mm  * &#x60;margem&#x3D;1,2,3,4&#x60;    - Margem esquerda: 1mm    - Margem superior: 2mm    - Margem direita: 3mm    - Margem inferior: 4mm | [opcional] |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarPreviaPdfNfce"></a>
# **baixarPreviaPdfNfce**
> Blob baixarPreviaPdfNfce(body, logotipo, nomeFantasia, mensagemRodape, resumido, qrcodeLateral, largura, margem)

Prévia do PDF do DANFCE

    Através desse endpoint, é possível enviar os dados de uma NFC-e e gerar uma prévia do DANFCE.    Os dados de entrada são os mesmos do endpoint de emissão de NFC-e (&#x60;POST /nfce&#x60;).    **Atenção**: O DANFE gerado por este endpoint é apenas para fins de visualização e não possui valor fiscal. Para a emissão de uma NF-e com valor fiscal, utilize o processo de emissão padrão descrito na documentação.    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**NfePedidoEmissao**](../Models/NfePedidoEmissao.md)|  | |
| **logotipo** | **boolean**| Imprime o documento com logotipo, desde que esteja cadastrado na empresa. | [opcional] |
| **nomeFantasia** | **boolean**| Exibe o nome fantasia do emitente, desde que esteja presente no XML da nota. | [opcional] |
| **mensagemRodape** | **string**| Imprime mensagem no rodapé do documento.    O caractere &#x60;|&#x60; (pipe) poderá ser utilizado para definir a quantidade e o alinhamento das mensagens.    **Exemplos de Uso:**  * &#x60;\&quot;esquerda\&quot;&#x60;  * &#x60;\&quot;esquerda|centro\&quot;&#x60;  * &#x60;\&quot;esquerda|centro|direita\&quot;&#x60;  * &#x60;\&quot;|centro\&quot;&#x60;, &#x60;\&quot;|centro|\&quot;&#x60;  * &#x60;\&quot;|centro|direita\&quot;&#x60;  * &#x60;\&quot;||direita\&quot;&#x60;  * &#x60;\&quot;esquerda||direita\&quot;&#x60; | [opcional] |
| **resumido** | **boolean**| Poderá ser impresso apenas o DANFE NFC-e resumido ou ecológico, sem o detalhamento dos itens da venda, desde que a Unidade Federada permita esta opção em sua legislação e o consumidor assim o solicite. | [opcional] |
| **qrcodeLateral** | **boolean**| Imprime o QRCode na lateral do DANFE NFC-e.    *Disponível apenas para DANFE com 80 milímetros de largura*. | [opcional] |
| **largura** | **number**| Largura do DANFE NFC-e (em milímetros). | [opcional] |
| **margem** | **string**| Define as margens do DANFE NFC-e (em milímetros).    Essa propriedade pode ser especificada usando um, dois, três ou quatro valores (separados por vírgulas). Cada valor deve ser um número entre &#x60;0&#x60; e &#x60;9&#x60;.  * Quando **um** valor é especificado, a mesma margem é aplicada para **todos os quatro lados**.  * Quando **dois** valores são especificados, a primeira margem é aplicada aos **lados esquerdo e direito**, e a segunda aos **lados superior e inferior**.  * Quando **três** valores são especificados, a primeira margem é aplicada ao **lado esquerdo**, a segunda aos **lados superior e inferior**, e a terceira ao **lado direito**.  * Quando **quatro** valores são especificados, as margens são aplicadas aos lados **esquerdo**, **superior**, **direito** e **inferior**, nesta ordem (sentido horário).    **Exemplos de uso**:  * &#x60;margem&#x3D;1&#x60;    - Margem esquerda: 1mm    - Margem superior: 1mm    - Margem direita: 1mm    - Margem inferior: 1mm  * &#x60;margem&#x3D;1,2&#x60;    - Margem esquerda: 1mm    - Margem superior: 2mm    - Margem direita: 1mm    - Margem inferior: 2mm  * &#x60;margem&#x3D;1,2,3&#x60;    - Margem esquerda: 1mm    - Margem superior: 2mm    - Margem direita: 3mm    - Margem inferior: 2mm  * &#x60;margem&#x3D;1,2,3,4&#x60;    - Margem esquerda: 1mm    - Margem superior: 2mm    - Margem direita: 3mm    - Margem inferior: 4mm | [opcional] |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarPreviaXmlNfce"></a>
# **baixarPreviaXmlNfce**
> Blob baixarPreviaXmlNfce(body)

Prévia do XML da NFC-e

    Através desse endpoint, é possível enviar os dados de uma NFC-e e gerar uma prévia do XML, sem a assinatura digital.    Os dados de entrada são os mesmos do endpoint de emissão de NFC-e (&#x60;POST /nfce&#x60;).    **Atenção**: O XML gerado por este endpoint é apenas para fins de visualização e não possui valor fiscal. Para a emissão de uma NF-e com valor fiscal, utilize o processo de emissão padrão descrito na documentação.    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

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

<a name="baixarXmlCancelamentoNfce"></a>
# **baixarXmlCancelamentoNfce**
> Blob baixarXmlCancelamentoNfce(id)

Baixar XML do cancelamento

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFC-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlEventoNfce"></a>
# **baixarXmlEventoNfce**
> Blob baixarXmlEventoNfce(id)

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

<a name="baixarXmlInutilizacaoNfce"></a>
# **baixarXmlInutilizacaoNfce**
> Blob baixarXmlInutilizacaoNfce(id)

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

<a name="baixarXmlNfce"></a>
# **baixarXmlNfce**
> Blob baixarXmlNfce(id)

Baixar XML da NFC-e processada

    Utilize esse endpoint para obter o XML da nota enviado para a SEFAZ, complementado com a informação do protocolo de autorização ou denegação de uso (TAG raiz &#x60;nfeProc&#x60;).    O XML só estará disponível nesse endpoint caso a nota tenha sido autorizada ou denegada pela SEFAZ. Para obter o XML nos demais casos, utilize o endpoint &#x60;GET /nfce/{id}/xml/nota&#x60;.    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFC-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlNfceNota"></a>
# **baixarXmlNfceNota**
> Blob baixarXmlNfceNota(id)

Baixar XML da NFC-e

    Utilize esse endpoint para obter o XML da nota enviado para a SEFAZ.    O XML estará disponível nesse endpoint mesmo em casos que a nota tenha sido rejeitada.    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFC-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlNfceProtocolo"></a>
# **baixarXmlNfceProtocolo**
> Blob baixarXmlNfceProtocolo(id)

Baixar XML do Protocolo da SEFAZ

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFC-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="cancelarNfce"></a>
# **cancelarNfce**
> DfeCancelamento cancelarNfce(id, body)

Cancelar uma NFC-e autorizada

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFC-e gerado pela API. | |
| **body** | [**NfePedidoCancelamento**](../Models/NfePedidoCancelamento.md)|  | [opcional] |

### Tipo do retorno

[**DfeCancelamento**](../Models/DfeCancelamento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarCancelamentoNfce"></a>
# **consultarCancelamentoNfce**
> DfeCancelamento consultarCancelamentoNfce(id)

Consultar o cancelamento da NFC-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFC-e gerado pela API. | |

### Tipo do retorno

[**DfeCancelamento**](../Models/DfeCancelamento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarEventoNfce"></a>
# **consultarEventoNfce**
> DfeEvento consultarEventoNfce(id)

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

<a name="consultarInutilizacaoNfce"></a>
# **consultarInutilizacaoNfce**
> DfeInutilizacao consultarInutilizacaoNfce(id)

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

<a name="consultarLoteNfce"></a>
# **consultarLoteNfce**
> DfeLote consultarLoteNfce(id)

Consultar lote de NFC-e

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

<a name="consultarNfce"></a>
# **consultarNfce**
> Dfe consultarNfce(id)

Consultar NFC-e

    Consulta os detalhes de uma NFC-e já existente. Forneça o ID único obtido de uma requisição de emissão ou de listagem de notas e a API irá retornar as informações da nota correspondente.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFC-e gerado pela API. | |

### Tipo do retorno

[**Dfe**](../Models/Dfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarStatusSefazNfce"></a>
# **consultarStatusSefazNfce**
> DfeSefazStatus consultarStatusSefazNfce(cpfCnpj, autorizador)

Consulta do Status do Serviço na SEFAZ Autorizadora

    Consulta do status do serviço prestado pelo Portal da Secretaria de Fazenda Estadual.    A API mantém a última consulta em cache por 5 minutos, evitando sobrecarregar desnecessariamente os servidores da SEFAZ (conforme orientação do MOC - versão 7.0, item 5.5.3). Dessa forma, você poderá chamar esse endpoint quantas vezes quiser, sem preocupar-se em ter o seu CNPJ bloqueado por consumo indevido (Rejeição 656).

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF/CNPJ do emitente.  Utilize o valor sem máscara. | |
| **autorizador** | **string**| Ambiente Autorizador.    Autorizadores disponíveis: &#x60;AM&#x60;, &#x60;BA&#x60;, &#x60;CE&#x60;, &#x60;GO&#x60;, &#x60;MG&#x60;, &#x60;MS&#x60;, &#x60;MT&#x60;, &#x60;PE&#x60;, &#x60;PR&#x60;, &#x60;RS&#x60;, &#x60;SP&#x60;, &#x60;SVRS&#x60;.    *Caso não seja informado, será utilizado o ambiente autorizador da UF do emitente.* | [opcional] |

### Tipo do retorno

[**DfeSefazStatus**](../Models/DfeSefazStatus.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="emitirLoteNfce"></a>
# **emitirLoteNfce**
> DfeLote emitirLoteNfce(body)

Emitir lote de NFC-e

    **Informações adicionais**:  - Consumo: 1 unidade por NFC-e.

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

<a name="emitirNfce"></a>
# **emitirNfce**
> Dfe emitirNfce(body)

Emitir NFC-e

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

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

<a name="enviarEmailNfce"></a>
# **enviarEmailNfce**
> EmailStatusResponse enviarEmailNfce(id, logotipo, nomeFantasia, mensagemRodape, resumido, qrcodeLateral, largura, margem, body)

Enviar e-mail

    Envia o XML e PDF da nota via email.    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFC-e gerado pela API. | |
| **logotipo** | **boolean**| Imprime o documento com logotipo, desde que esteja cadastrado na empresa. | [opcional] |
| **nomeFantasia** | **boolean**| Exibe o nome fantasia do emitente, desde que esteja presente no XML da nota. | [opcional] |
| **mensagemRodape** | **string**| Imprime mensagem no rodapé do documento.    O caractere &#x60;|&#x60; (pipe) poderá ser utilizado para definir a quantidade e o alinhamento das mensagens.    **Exemplos de Uso:**  * &#x60;\&quot;esquerda\&quot;&#x60;  * &#x60;\&quot;esquerda|centro\&quot;&#x60;  * &#x60;\&quot;esquerda|centro|direita\&quot;&#x60;  * &#x60;\&quot;|centro\&quot;&#x60;, &#x60;\&quot;|centro|\&quot;&#x60;  * &#x60;\&quot;|centro|direita\&quot;&#x60;  * &#x60;\&quot;||direita\&quot;&#x60;  * &#x60;\&quot;esquerda||direita\&quot;&#x60; | [opcional] |
| **resumido** | **boolean**| Poderá ser impresso apenas o DANFE NFC-e resumido ou ecológico, sem o detalhamento dos itens da venda, desde que a Unidade Federada permita esta opção em sua legislação e o consumidor assim o solicite. | [opcional] |
| **qrcodeLateral** | **boolean**| Imprime o QRCode na lateral do DANFE NFC-e.    *Disponível apenas para DANFE com 80 milímetros de largura*. | [opcional] |
| **largura** | **number**| Largura do DANFE NFC-e (em milímetros). | [opcional] |
| **margem** | **string**| Define as margens do DANFE NFC-e (em milímetros).    Essa propriedade pode ser especificada usando um, dois, três ou quatro valores (separados por vírgulas). Cada valor deve ser um número entre &#x60;0&#x60; e &#x60;9&#x60;.  * Quando **um** valor é especificado, a mesma margem é aplicada para **todos os quatro lados**.  * Quando **dois** valores são especificados, a primeira margem é aplicada aos **lados esquerdo e direito**, e a segunda aos **lados superior e inferior**.  * Quando **três** valores são especificados, a primeira margem é aplicada ao **lado esquerdo**, a segunda aos **lados superior e inferior**, e a terceira ao **lado direito**.  * Quando **quatro** valores são especificados, as margens são aplicadas aos lados **esquerdo**, **superior**, **direito** e **inferior**, nesta ordem (sentido horário).    **Exemplos de uso**:  * &#x60;margem&#x3D;1&#x60;    - Margem esquerda: 1mm    - Margem superior: 1mm    - Margem direita: 1mm    - Margem inferior: 1mm  * &#x60;margem&#x3D;1,2&#x60;    - Margem esquerda: 1mm    - Margem superior: 2mm    - Margem direita: 1mm    - Margem inferior: 2mm  * &#x60;margem&#x3D;1,2,3&#x60;    - Margem esquerda: 1mm    - Margem superior: 2mm    - Margem direita: 3mm    - Margem inferior: 2mm  * &#x60;margem&#x3D;1,2,3,4&#x60;    - Margem esquerda: 1mm    - Margem superior: 2mm    - Margem direita: 3mm    - Margem inferior: 4mm | [opcional] |
| **body** | [**DfePedidoEnvioEmail**](../Models/DfePedidoEnvioEmail.md)|  | [opcional] |

### Tipo do retorno

[**EmailStatusResponse**](../Models/EmailStatusResponse.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="inutilizarNumeracaoNfce"></a>
# **inutilizarNumeracaoNfce**
> DfeInutilizacao inutilizarNumeracaoNfce(body)

Inutilizar uma sequência de numeração de NFC-e

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

<a name="listarEventosNfce"></a>
# **listarEventosNfce**
> DfeEventoListagem listarEventosNfce(dfeId, $top, $skip, $inlinecount)

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

<a name="listarLotesNfce"></a>
# **listarLotesNfce**
> DfeLoteListagem listarLotesNfce(cpfCnpj, ambiente, $top, $skip, $inlinecount, referencia)

Listar lotes de NFC-e

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

<a name="listarNfce"></a>
# **listarNfce**
> DfeListagem listarNfce(cpfCnpj, ambiente, $top, $skip, $inlinecount, referencia, chave, serie)

Listar NFC-e

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

<a name="sincronizarNfce"></a>
# **sincronizarNfce**
> DfeSincronizacao sincronizarNfce(id)

Sincroniza dados na NFC-e a partir da SEFAZ

    Realiza a sincronização dos dados a partir da consulta da situação atual da NFC-e na Base de Dados do Portal da Secretaria de Fazenda Estadual.    **Cenários de uso**:  * Sincronizar uma nota que se encontra com o status &#x60;erro&#x60; na API, mas está autorizada na SEFAZ (útil em casos de erros de transmissão com a SEFAZ, como instabilidades e timeouts).  * Sincronizar uma nota que se encontra com o status &#x60;autorizado&#x60;na API, mas está cancelada na SEFAZ.  * Sincronizar todos os eventos de Cancelamento, Carta de Correção e EPEC de uma nota que porventura não tenham sido feitos a partir da API.    **Informações adicionais**:  - Consumo: 1 unidade por evento sincronizado ou requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFC-e gerado pela API. | |

### Tipo do retorno

[**DfeSincronizacao**](../Models/DfeSincronizacao.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

