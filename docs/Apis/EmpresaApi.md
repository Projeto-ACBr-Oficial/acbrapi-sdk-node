# EmpresaApi

Todas as URIs relativas a *https://prod.acbr.api.br*

| Método | Endpoint | Descrição |
|------------- | ------------- | -------------|
| [**alterarConfigCte**](EmpresaApi.md#alterarConfigCte) | **PUT** /empresas/{cpf_cnpj}/cte | Alterar configuração de CT-e |
| [**alterarConfigCteOs**](EmpresaApi.md#alterarConfigCteOs) | **PUT** /empresas/{cpf_cnpj}/cteos | Alterar configuração de CT-e OS |
| [**alterarConfigDce**](EmpresaApi.md#alterarConfigDce) | **PUT** /empresas/{cpf_cnpj}/dce | Alterar configuração de DC-e |
| [**alterarConfigDistribuicaoNfe**](EmpresaApi.md#alterarConfigDistribuicaoNfe) | **PUT** /empresas/{cpf_cnpj}/distnfe | Alterar configuração de Distribuição de NF-e |
| [**alterarConfigMdfe**](EmpresaApi.md#alterarConfigMdfe) | **PUT** /empresas/{cpf_cnpj}/mdfe | Alterar configuração de MDF-e |
| [**alterarConfigNfce**](EmpresaApi.md#alterarConfigNfce) | **PUT** /empresas/{cpf_cnpj}/nfce | Alterar configuração de NFC-e |
| [**alterarConfigNfcom**](EmpresaApi.md#alterarConfigNfcom) | **PUT** /empresas/{cpf_cnpj}/nfcom | Alterar configuração de NFCom |
| [**alterarConfigNfe**](EmpresaApi.md#alterarConfigNfe) | **PUT** /empresas/{cpf_cnpj}/nfe | Alterar configuração de NF-e |
| [**alterarConfigNfse**](EmpresaApi.md#alterarConfigNfse) | **PUT** /empresas/{cpf_cnpj}/nfse | Alterar configuração de NFS-e |
| [**atualizarEmpresa**](EmpresaApi.md#atualizarEmpresa) | **PUT** /empresas/{cpf_cnpj} | Alterar empresa |
| [**baixarLogotipoEmpresa**](EmpresaApi.md#baixarLogotipoEmpresa) | **GET** /empresas/{cpf_cnpj}/logotipo | Baixar logotipo |
| [**cadastrarCertificadoEmpresa**](EmpresaApi.md#cadastrarCertificadoEmpresa) | **PUT** /empresas/{cpf_cnpj}/certificado | Cadastrar certificado |
| [**consultarCertificadoEmpresa**](EmpresaApi.md#consultarCertificadoEmpresa) | **GET** /empresas/{cpf_cnpj}/certificado | Consultar certificado |
| [**consultarConfigCte**](EmpresaApi.md#consultarConfigCte) | **GET** /empresas/{cpf_cnpj}/cte | Consultar configuração de CT-e |
| [**consultarConfigCteOs**](EmpresaApi.md#consultarConfigCteOs) | **GET** /empresas/{cpf_cnpj}/cteos | Consultar configuração de CT-e OS |
| [**consultarConfigDce**](EmpresaApi.md#consultarConfigDce) | **GET** /empresas/{cpf_cnpj}/dce | Consultar configuração de DC-e |
| [**consultarConfigDistribuicaoNfe**](EmpresaApi.md#consultarConfigDistribuicaoNfe) | **GET** /empresas/{cpf_cnpj}/distnfe | Consultar configuração de Distribuição de NF-e |
| [**consultarConfigMdfe**](EmpresaApi.md#consultarConfigMdfe) | **GET** /empresas/{cpf_cnpj}/mdfe | Consultar configuração de MDF-e |
| [**consultarConfigNfce**](EmpresaApi.md#consultarConfigNfce) | **GET** /empresas/{cpf_cnpj}/nfce | Consultar configuração de NFC-e |
| [**consultarConfigNfcom**](EmpresaApi.md#consultarConfigNfcom) | **GET** /empresas/{cpf_cnpj}/nfcom | Consultar configuração de NFCom |
| [**consultarConfigNfe**](EmpresaApi.md#consultarConfigNfe) | **GET** /empresas/{cpf_cnpj}/nfe | Consultar configuração de NF-e |
| [**consultarConfigNfse**](EmpresaApi.md#consultarConfigNfse) | **GET** /empresas/{cpf_cnpj}/nfse | Consultar configuração de NFS-e |
| [**consultarEmpresa**](EmpresaApi.md#consultarEmpresa) | **GET** /empresas/{cpf_cnpj} | Consultar empresa |
| [**criarEmpresa**](EmpresaApi.md#criarEmpresa) | **POST** /empresas | Cadastrar empresa |
| [**enviarCertificadoEmpresa**](EmpresaApi.md#enviarCertificadoEmpresa) | **PUT** /empresas/{cpf_cnpj}/certificado/upload | Upload de certificado |
| [**enviarLogotipoEmpresa**](EmpresaApi.md#enviarLogotipoEmpresa) | **PUT** /empresas/{cpf_cnpj}/logotipo | Enviar logotipo |
| [**excluirCertificadoEmpresa**](EmpresaApi.md#excluirCertificadoEmpresa) | **DELETE** /empresas/{cpf_cnpj}/certificado | Deletar certificado |
| [**excluirEmpresa**](EmpresaApi.md#excluirEmpresa) | **DELETE** /empresas/{cpf_cnpj} | Deletar empresa |
| [**excluirLogotipoEmpresa**](EmpresaApi.md#excluirLogotipoEmpresa) | **DELETE** /empresas/{cpf_cnpj}/logotipo | Deletar logotipo |
| [**listarCertificados**](EmpresaApi.md#listarCertificados) | **GET** /empresas/certificados | Listar certificados |
| [**listarEmpresas**](EmpresaApi.md#listarEmpresas) | **GET** /empresas | Listar empresas |


<a name="alterarConfigCte"></a>
# **alterarConfigCte**
> EmpresaConfigCte alterarConfigCte(cpfCnpj, body)

Alterar configuração de CT-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |
| **body** | [**EmpresaConfigCte**](../Models/EmpresaConfigCte.md)|  | |

### Tipo do retorno

[**EmpresaConfigCte**](../Models/EmpresaConfigCte.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="alterarConfigCteOs"></a>
# **alterarConfigCteOs**
> EmpresaConfigCteOs alterarConfigCteOs(cpfCnpj, body)

Alterar configuração de CT-e OS

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |
| **body** | [**EmpresaConfigCteOs**](../Models/EmpresaConfigCteOs.md)|  | |

### Tipo do retorno

[**EmpresaConfigCteOs**](../Models/EmpresaConfigCteOs.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="alterarConfigDce"></a>
# **alterarConfigDce**
> EmpresaConfigDce alterarConfigDce(cpfCnpj, body)

Alterar configuração de DC-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |
| **body** | [**EmpresaConfigDce**](../Models/EmpresaConfigDce.md)|  | |

### Tipo do retorno

[**EmpresaConfigDce**](../Models/EmpresaConfigDce.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="alterarConfigDistribuicaoNfe"></a>
# **alterarConfigDistribuicaoNfe**
> EmpresaConfigDistribuicaoNfe alterarConfigDistribuicaoNfe(cpfCnpj, body)

Alterar configuração de Distribuição de NF-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |
| **body** | [**EmpresaConfigDistribuicaoNfe**](../Models/EmpresaConfigDistribuicaoNfe.md)|  | |

### Tipo do retorno

[**EmpresaConfigDistribuicaoNfe**](../Models/EmpresaConfigDistribuicaoNfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="alterarConfigMdfe"></a>
# **alterarConfigMdfe**
> EmpresaConfigMdfe alterarConfigMdfe(cpfCnpj, body)

Alterar configuração de MDF-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |
| **body** | [**EmpresaConfigMdfe**](../Models/EmpresaConfigMdfe.md)|  | |

### Tipo do retorno

[**EmpresaConfigMdfe**](../Models/EmpresaConfigMdfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="alterarConfigNfce"></a>
# **alterarConfigNfce**
> EmpresaConfigNfce alterarConfigNfce(cpfCnpj, body)

Alterar configuração de NFC-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |
| **body** | [**EmpresaConfigNfce**](../Models/EmpresaConfigNfce.md)|  | |

### Tipo do retorno

[**EmpresaConfigNfce**](../Models/EmpresaConfigNfce.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="alterarConfigNfcom"></a>
# **alterarConfigNfcom**
> EmpresaConfigNfcom alterarConfigNfcom(cpfCnpj, body)

Alterar configuração de NFCom

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |
| **body** | [**EmpresaConfigNfcom**](../Models/EmpresaConfigNfcom.md)|  | |

### Tipo do retorno

[**EmpresaConfigNfcom**](../Models/EmpresaConfigNfcom.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="alterarConfigNfe"></a>
# **alterarConfigNfe**
> EmpresaConfigNfe alterarConfigNfe(cpfCnpj, body)

Alterar configuração de NF-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |
| **body** | [**EmpresaConfigNfe**](../Models/EmpresaConfigNfe.md)|  | |

### Tipo do retorno

[**EmpresaConfigNfe**](../Models/EmpresaConfigNfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="alterarConfigNfse"></a>
# **alterarConfigNfse**
> EmpresaConfigNfse alterarConfigNfse(cpfCnpj, body)

Alterar configuração de NFS-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |
| **body** | [**EmpresaConfigNfse**](../Models/EmpresaConfigNfse.md)|  | |

### Tipo do retorno

[**EmpresaConfigNfse**](../Models/EmpresaConfigNfse.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="atualizarEmpresa"></a>
# **atualizarEmpresa**
> Empresa atualizarEmpresa(cpfCnpj, body)

Alterar empresa

    Altera o cadastro de uma empresa (emitente/prestador) que esteja associada a sua conta.  Nesse método, por tratar-se de um PUT, caso algum campo não seja informado, o valor dele será apagado.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |
| **body** | [**Empresa**](../Models/Empresa.md)|  | |

### Tipo do retorno

[**Empresa**](../Models/Empresa.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarLogotipoEmpresa"></a>
# **baixarLogotipoEmpresa**
> Blob baixarLogotipoEmpresa(cpfCnpj)

Baixar logotipo

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="cadastrarCertificadoEmpresa"></a>
# **cadastrarCertificadoEmpresa**
> EmpresaCertificado cadastrarCertificadoEmpresa(cpfCnpj, body)

Cadastrar certificado

    Cadastre ou atualize um certificado digital e vincule a sua empresa, para que possa iniciar a emissão de notas.  * No parâmetro &#x60;certificado&#x60;, envie o binário do certificado digital (.pfx ou .p12) codificado em **base64**.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |
| **body** | [**EmpresaPedidoCadastroCertificado**](../Models/EmpresaPedidoCadastroCertificado.md)|  | |

### Tipo do retorno

[**EmpresaCertificado**](../Models/EmpresaCertificado.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarCertificadoEmpresa"></a>
# **consultarCertificadoEmpresa**
> EmpresaCertificado consultarCertificadoEmpresa(cpfCnpj)

Consultar certificado

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |

### Tipo do retorno

[**EmpresaCertificado**](../Models/EmpresaCertificado.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarConfigCte"></a>
# **consultarConfigCte**
> EmpresaConfigCte consultarConfigCte(cpfCnpj)

Consultar configuração de CT-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |

### Tipo do retorno

[**EmpresaConfigCte**](../Models/EmpresaConfigCte.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarConfigCteOs"></a>
# **consultarConfigCteOs**
> EmpresaConfigCteOs consultarConfigCteOs(cpfCnpj)

Consultar configuração de CT-e OS

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |

### Tipo do retorno

[**EmpresaConfigCteOs**](../Models/EmpresaConfigCteOs.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarConfigDce"></a>
# **consultarConfigDce**
> EmpresaConfigDce consultarConfigDce(cpfCnpj)

Consultar configuração de DC-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |

### Tipo do retorno

[**EmpresaConfigDce**](../Models/EmpresaConfigDce.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarConfigDistribuicaoNfe"></a>
# **consultarConfigDistribuicaoNfe**
> EmpresaConfigDistribuicaoNfe consultarConfigDistribuicaoNfe(cpfCnpj)

Consultar configuração de Distribuição de NF-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |

### Tipo do retorno

[**EmpresaConfigDistribuicaoNfe**](../Models/EmpresaConfigDistribuicaoNfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarConfigMdfe"></a>
# **consultarConfigMdfe**
> EmpresaConfigMdfe consultarConfigMdfe(cpfCnpj)

Consultar configuração de MDF-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |

### Tipo do retorno

[**EmpresaConfigMdfe**](../Models/EmpresaConfigMdfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarConfigNfce"></a>
# **consultarConfigNfce**
> EmpresaConfigNfce consultarConfigNfce(cpfCnpj)

Consultar configuração de NFC-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |

### Tipo do retorno

[**EmpresaConfigNfce**](../Models/EmpresaConfigNfce.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarConfigNfcom"></a>
# **consultarConfigNfcom**
> EmpresaConfigNfcom consultarConfigNfcom(cpfCnpj)

Consultar configuração de NFCom

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |

### Tipo do retorno

[**EmpresaConfigNfcom**](../Models/EmpresaConfigNfcom.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarConfigNfe"></a>
# **consultarConfigNfe**
> EmpresaConfigNfe consultarConfigNfe(cpfCnpj)

Consultar configuração de NF-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |

### Tipo do retorno

[**EmpresaConfigNfe**](../Models/EmpresaConfigNfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarConfigNfse"></a>
# **consultarConfigNfse**
> EmpresaConfigNfse consultarConfigNfse(cpfCnpj)

Consultar configuração de NFS-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |

### Tipo do retorno

[**EmpresaConfigNfse**](../Models/EmpresaConfigNfse.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarEmpresa"></a>
# **consultarEmpresa**
> Empresa consultarEmpresa(cpfCnpj)

Consultar empresa

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |

### Tipo do retorno

[**Empresa**](../Models/Empresa.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="criarEmpresa"></a>
# **criarEmpresa**
> Empresa criarEmpresa(body)

Cadastrar empresa

    Cadastre uma nova empresa (emitente ou prestador) à sua conta.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**Empresa**](../Models/Empresa.md)|  | |

### Tipo do retorno

[**Empresa**](../Models/Empresa.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="enviarCertificadoEmpresa"></a>
# **enviarCertificadoEmpresa**
> EmpresaCertificado enviarCertificadoEmpresa(cpfCnpj, input)

Upload de certificado

    Cadastre ou atualize um certificado digital e vincule a sua empresa, para que possa iniciar a emissão de notas.  * Utilize o &#x60;content-type&#x60; igual a &#x60;multipart/form-data&#x60;.  * No parâmetro &#x60;file&#x60;, envie o binário do arquivo (.pfx ou .p12) do certificado digital.  * No parâmetro &#x60;password&#x60;, envie a senha do certificado.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |
| **input** | **Blob**|  | [opcional] |

### Tipo do retorno

[**EmpresaCertificado**](../Models/EmpresaCertificado.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="enviarLogotipoEmpresa"></a>
# **enviarLogotipoEmpresa**
> enviarLogotipoEmpresa(cpfCnpj, input)

Enviar logotipo

    Cadastre ou atualize um logotipo e vincule a sua empresa.    **Restrições:**  * Tipos de mídia (MIME) suportados: &#x60;image/png&#x60; e &#x60;image/jpeg&#x60;  * Tamanho máximo do arquivo: 200 KB    **Cenários de uso:**  * Quero que minhas notas sejam impressas com esse logotipo.  * Quero trocar o logotipo utilizado em minhas impressões.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |
| **input** | **Blob**|  | [opcional] |

### Tipo do retorno

null (corpo de resposta vazio)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: multipart/form-data
- **Accept**: Não definido

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="excluirCertificadoEmpresa"></a>
# **excluirCertificadoEmpresa**
> excluirCertificadoEmpresa(cpfCnpj)

Deletar certificado

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |

### Tipo do retorno

null (corpo de resposta vazio)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: Não definido

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="excluirEmpresa"></a>
# **excluirEmpresa**
> excluirEmpresa(cpfCnpj)

Deletar empresa

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |

### Tipo do retorno

null (corpo de resposta vazio)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: Não definido

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="excluirLogotipoEmpresa"></a>
# **excluirLogotipoEmpresa**
> excluirLogotipoEmpresa(cpfCnpj)

Deletar logotipo

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF ou CNPJ da empresa.  Utilize o valor sem máscara. | |

### Tipo do retorno

null (corpo de resposta vazio)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: Não definido

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarCertificados"></a>
# **listarCertificados**
> EmpresaCertificadoListagem listarCertificados($top, $skip, $inlinecount, expiresIn, includeExpired)

Listar certificados

    Retorna a lista dos certificados associadas à sua conta. Os certificados são retornados ordenados pela data da criação, com as mais recentes aparecendo primeiro.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **$top** | **number**| Limite no número de objetos a serem retornados pela API, entre 1 e 100. | [opcional] |
| **$skip** | **number**| Quantidade de objetos que serão ignorados antes da lista começar a ser retornada. | [opcional] |
| **$inlinecount** | **boolean**| Inclui no JSON de resposta, na propriedade &#x60;@count&#x60;, o número total de registros que o filtro retornaria, independente dos filtros de paginação. | [opcional] |
| **expiresIn** | **number**| Filtrar certificados que expiram dentro de X dias.    Informe um número inteiro correspondente à quantidade de dias até o vencimento.  Exemplos:   - expires_in&#x3D;30 -&amp;gt; certificados que vencem nos próximos 30 dias.   - expires_in&#x3D;7  -&amp;gt; certificados que vencem nos próximos 7 dias. | [opcional] |
| **includeExpired** | **boolean**| Indicar se os certificados já vencidos devem ser incluídos no resultado.    Valores aceitos:   - &#x60;true&#x60;: incluir certificados vencidos.   - &#x60;false&#x60;: exibir apenas certificados válidos. | [opcional] |

### Tipo do retorno

[**EmpresaCertificadoListagem**](../Models/EmpresaCertificadoListagem.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarEmpresas"></a>
# **listarEmpresas**
> EmpresaListagem listarEmpresas($top, $skip, $inlinecount, cpfCnpj, nomeRazaoSocial)

Listar empresas

    Retorna a lista das empresas associadas à sua conta. As empresas são retornadas ordenadas pela data da criação, com as mais recentes aparecendo primeiro.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **$top** | **number**| Limite no número de objetos a serem retornados pela API, entre 1 e 100. | [opcional] |
| **$skip** | **number**| Quantidade de objetos que serão ignorados antes da lista começar a ser retornada. | [opcional] |
| **$inlinecount** | **boolean**| Inclui no JSON de resposta, na propriedade &#x60;@count&#x60;, o número total de registros que o filtro retornaria, independente dos filtros de paginação. | [opcional] |
| **cpfCnpj** | **string**| Filtrar pelo CPF ou CNPJ da empresa.    *Utilize o valor sem máscara*. | [opcional] |
| **nomeRazaoSocial** | **string**| Filtrar pelo nome ou razão social da empresa.    Esse filtro realiza uma correspondência pelo início do texto,  retornando apenas empresas cujo nome ou razão social começam com  o valor informado.    *Caso o filtro pelo CPF ou CNPJ também seja informado na requisição,  este filtro é ignorado*. | [opcional] |

### Tipo do retorno

[**EmpresaListagem**](../Models/EmpresaListagem.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

