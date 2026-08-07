# EmailApi

Todas as URIs relativas a *https://prod.acbr.api.br*

| Método | Endpoint | Descrição |
|------------- | ------------- | -------------|
| [**consultarEmail**](EmailApi.md#consultarEmail) | **GET** /emails/{id} | Consultar e-mail |
| [**listarEmails**](EmailApi.md#listarEmails) | **GET** /emails | Listar e-mails |


<a name="consultarEmail"></a>
# **consultarEmail**
> Email consultarEmail(id)

Consultar e-mail

    Obtém informações detalhadas sobre o envio de um email. Este endpoint  permite rastrear todos os eventos relacionados ao email, como envio,  entrega, falhas e outros eventos relevantes.    Com este endpoint, é possível ter uma visão completa do ciclo de vida  de um email enviado, permitindo que os usuários acompanhem e analisem  o status e o histórico de eventos do email. Isso é particularmente  útil para identificar problemas de entrega e entender o comportamento  do email ao longo do tempo.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do e-mail.    Esse parâmetro é obtido após o envio do email por qualquer endpoint da  API que realize disparos de email.    Exemplos:  * &lt;a href&#x3D;\&quot;#tag/Nfe/operation/EnviarEmailNfe\&quot;&gt;Envio de XML e PDF de NF-e&lt;/a&gt;.  * &lt;a href&#x3D;\&quot;#tag/Nfce/operation/EnviarEmailNfce\&quot;&gt;Envio de XML e PDF de NFC-e&lt;/a&gt;. | |

### Tipo do retorno

[**Email**](../Models/Email.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarEmails"></a>
# **listarEmails**
> EmailListagem listarEmails(cpfCnpj, $top, $skip, $inlinecount, undelivered, email)

Listar e-mails

    Retorna a lista dos emails associadas à sua conta. Os e-emails são  retornados ordenados pela data da criação, com os mais recentes  aparecendo primeiro.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| Filtra pelo CPF ou CNPJ da empresa.    *Utilize o valor sem máscara*. | |
| **$top** | **number**| Limite no número de objetos a serem retornados pela API, entre 1 e 100. | [opcional] |
| **$skip** | **number**| Quantidade de objetos que serão ignorados antes da lista começar a ser retornada. | [opcional] |
| **$inlinecount** | **boolean**| Inclui no JSON de resposta, na propriedade &#x60;@count&#x60;, o número total de registros que o filtro retornaria, independente dos filtros de paginação. | [opcional] |
| **undelivered** | **boolean**| Filtra apenas emails com problemas de entrega. | [opcional] |
| **email** | **string**| Filtra pelo endereço de e-mail do destinatário para qual o email foi enviado. | [opcional] |

### Tipo do retorno

[**EmailListagem**](../Models/EmailListagem.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

