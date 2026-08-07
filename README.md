# ACBr API: SDK para Node.js

Biblioteca para uso da [ACBr API](https://www.acbr.api.br) com [Node.js](https://nodejs.org).
Consultar também a [documentação oficial da ACBr API](https://dev.acbr.api.br/docs).

Índice dos [endpoints](#documentation-for-api-endpoints) e dos
[DTOs](#documentation-for-models) no fim desta página. A referência detalhada
de cada um fica em [docs/](docs/README.md).

## Instalação

Instale direto do GitHub. Rode o comando na pasta do seu projeto
(onde fica o `package.json`). O pacote é compilado automaticamente no momento
da instalação (script `prepare`), então não é preciso rodar o build manualmente:

```sh
npm install git+https://github.com/projeto-acbr-oficial/acbrapi-sdk-node.git --save
```

ou na forma curta:

```sh
npm install projeto-acbr-oficial/acbrapi-sdk-node --save
```

Fixando a branch `main` (ou troque por uma tag/commit quando disponível):

```sh
npm install "git+https://github.com/projeto-acbr-oficial/acbrapi-sdk-node.git#main" --save
```

No `package.json` do seu projeto isso equivale a:

```json
{
  "dependencies": {
    "acbrapi-sdk": "git+https://github.com/projeto-acbr-oficial/acbrapi-sdk-node.git#main"
  }
}
```

### Importando o pacote

Depois de instalar por qualquer um dos métodos acima:

```typescript
import { Configuration, CnpjApi } from 'acbrapi-sdk';
```

## Desenvolvimento (build a partir do código-fonte)

Para compilar os fontes TypeScript para JavaScript:

```sh
npm install
npm run build
```

<a name="documentation-for-api-endpoints"></a>
## Documentação dos endpoints

Todas as URIs relativas a *https://prod.acbr.api.br*

Classe | Método | Endpoint | Descrição
------------ | ------------- | ------------- | -------------
*CepApi* | [**consultarCep**](docs/Apis/CepApi.md#consultarCep) | **GET** /cep/{Cep} | Consultar endereço através do CEP
*CnpjApi* | [**consultarCnpj**](docs/Apis/CnpjApi.md#consultarCnpj) | **GET** /cnpj/{Cnpj} | Consultar dados do CNPJ
*CnpjApi* | [**listarCnpj**](docs/Apis/CnpjApi.md#listarCnpj) | **GET** /cnpj | Listar estabelecimentos ativos a partir da base de CNPJ
*ContaApi* | [**consultarCotaConta**](docs/Apis/ContaApi.md#consultarCotaConta) | **GET** /conta/cotas/{nome} | Consultar o limite de uso e o consumo de uma cota específica.
*ContaApi* | [**consultarCotaPrePago**](docs/Apis/ContaApi.md#consultarCotaPrePago) | **GET** /conta/cotas/prepago | Consultar o resumo da cota de créditos pré-pagos.
*ContaApi* | [**listarCotasConta**](docs/Apis/ContaApi.md#listarCotasConta) | **GET** /conta/cotas | Consultar os limites de uso e consumo das cotas disponíveis, exceto a cota de créditos pré-pagos.
*ContaApi* | [**listarExtratoCreditosConta**](docs/Apis/ContaApi.md#listarExtratoCreditosConta) | **GET** /conta/extrato | Consultar o extrato de movimentação de créditos do tenant atual.
*CteApi* | [**baixarPdfCancelamentoCte**](docs/Apis/CteApi.md#baixarPdfCancelamentoCte) | **GET** /cte/{id}/cancelamento/pdf | Baixar PDF do cancelamento
*CteApi* | [**baixarPdfCartaCorrecaoCte**](docs/Apis/CteApi.md#baixarPdfCartaCorrecaoCte) | **GET** /cte/{id}/carta-correcao/pdf | Baixar PDF da carta de correção
*CteApi* | [**baixarPdfCte**](docs/Apis/CteApi.md#baixarPdfCte) | **GET** /cte/{id}/pdf | Baixar PDF do DACTE
*CteApi* | [**baixarPdfEventoCte**](docs/Apis/CteApi.md#baixarPdfEventoCte) | **GET** /cte/eventos/{id}/pdf | Baixar PDF do evento
*CteApi* | [**baixarXmlCancelamentoCte**](docs/Apis/CteApi.md#baixarXmlCancelamentoCte) | **GET** /cte/{id}/cancelamento/xml | Baixar XML do cancelamento
*CteApi* | [**baixarXmlCartaCorrecaoCte**](docs/Apis/CteApi.md#baixarXmlCartaCorrecaoCte) | **GET** /cte/{id}/carta-correcao/xml | Baixar XML da carta de correção
*CteApi* | [**baixarXmlCte**](docs/Apis/CteApi.md#baixarXmlCte) | **GET** /cte/{id}/xml | Baixar XML do CT-e processado
*CteApi* | [**baixarXmlCteConhecimento**](docs/Apis/CteApi.md#baixarXmlCteConhecimento) | **GET** /cte/{id}/xml/conhecimento | Baixar XML do CT-e
*CteApi* | [**baixarXmlCteProtocolo**](docs/Apis/CteApi.md#baixarXmlCteProtocolo) | **GET** /cte/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ
*CteApi* | [**baixarXmlEventoCte**](docs/Apis/CteApi.md#baixarXmlEventoCte) | **GET** /cte/eventos/{id}/xml | Baixar XML do evento
*CteApi* | [**cancelarCte**](docs/Apis/CteApi.md#cancelarCte) | **POST** /cte/{id}/cancelamento | Cancelar um CT-e autorizado
*CteApi* | [**consultarCancelamentoCte**](docs/Apis/CteApi.md#consultarCancelamentoCte) | **GET** /cte/{id}/cancelamento | Consultar o cancelamento do CT-e
*CteApi* | [**consultarCartaCorrecaoCte**](docs/Apis/CteApi.md#consultarCartaCorrecaoCte) | **GET** /cte/{id}/carta-correcao | Consultar a solicitação de correção do CT-e
*CteApi* | [**consultarCte**](docs/Apis/CteApi.md#consultarCte) | **GET** /cte/{id} | Consultar CT-e
*CteApi* | [**consultarEventoCte**](docs/Apis/CteApi.md#consultarEventoCte) | **GET** /cte/eventos/{id} | Consultar evento
*CteApi* | [**consultarStatusSefazCte**](docs/Apis/CteApi.md#consultarStatusSefazCte) | **GET** /cte/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora
*CteApi* | [**criarCartaCorrecaoCte**](docs/Apis/CteApi.md#criarCartaCorrecaoCte) | **POST** /cte/{id}/carta-correcao | Solicitar correção do CT-e
*CteApi* | [**emitirCte**](docs/Apis/CteApi.md#emitirCte) | **POST** /cte | Emitir CT-e
*CteApi* | [**emitirCteSimp**](docs/Apis/CteApi.md#emitirCteSimp) | **POST** /cte/simp | Emitir CT-e Simplificado
*CteApi* | [**listarCte**](docs/Apis/CteApi.md#listarCte) | **GET** /cte | Listar CT-e
*CteApi* | [**sincronizarCte**](docs/Apis/CteApi.md#sincronizarCte) | **POST** /cte/{id}/sincronizar | Sincroniza dados no CT-e a partir da SEFAZ
*CteOsApi* | [**baixarPdfCancelamentoCteOs**](docs/Apis/CteOsApi.md#baixarPdfCancelamentoCteOs) | **GET** /cteos/{id}/cancelamento/pdf | Baixar PDF do cancelamento
*CteOsApi* | [**baixarPdfCartaCorrecaoCteOs**](docs/Apis/CteOsApi.md#baixarPdfCartaCorrecaoCteOs) | **GET** /cteos/{id}/carta-correcao/pdf | Baixar PDF da carta de correção
*CteOsApi* | [**baixarPdfCteOs**](docs/Apis/CteOsApi.md#baixarPdfCteOs) | **GET** /cteos/{id}/pdf | Baixar PDF do DACTE
*CteOsApi* | [**baixarPdfEventoCteOs**](docs/Apis/CteOsApi.md#baixarPdfEventoCteOs) | **GET** /cteos/eventos/{id}/pdf | Baixar PDF do evento
*CteOsApi* | [**baixarXmlCancelamentoCteOs**](docs/Apis/CteOsApi.md#baixarXmlCancelamentoCteOs) | **GET** /cteos/{id}/cancelamento/xml | Baixar XML do cancelamento
*CteOsApi* | [**baixarXmlCartaCorrecaoCteOs**](docs/Apis/CteOsApi.md#baixarXmlCartaCorrecaoCteOs) | **GET** /cteos/{id}/carta-correcao/xml | Baixar XML da carta de correção
*CteOsApi* | [**baixarXmlCteOs**](docs/Apis/CteOsApi.md#baixarXmlCteOs) | **GET** /cteos/{id}/xml | Baixar XML do CT-e OS processado
*CteOsApi* | [**baixarXmlCteOsConhecimento**](docs/Apis/CteOsApi.md#baixarXmlCteOsConhecimento) | **GET** /cteos/{id}/xml/conhecimento | Baixar XML do CT-e OS
*CteOsApi* | [**baixarXmlCteOsProtocolo**](docs/Apis/CteOsApi.md#baixarXmlCteOsProtocolo) | **GET** /cteos/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ
*CteOsApi* | [**baixarXmlEventoCteOs**](docs/Apis/CteOsApi.md#baixarXmlEventoCteOs) | **GET** /cteos/eventos/{id}/xml | Baixar XML do evento
*CteOsApi* | [**cancelarCteOs**](docs/Apis/CteOsApi.md#cancelarCteOs) | **POST** /cteos/{id}/cancelamento | Cancelar um CT-e OS autorizado
*CteOsApi* | [**consultarCancelamentoCteOs**](docs/Apis/CteOsApi.md#consultarCancelamentoCteOs) | **GET** /cteos/{id}/cancelamento | Consultar o cancelamento do CT-e OS
*CteOsApi* | [**consultarCartaCorrecaoCteOs**](docs/Apis/CteOsApi.md#consultarCartaCorrecaoCteOs) | **GET** /cteos/{id}/carta-correcao | Consultar a solicitação de correção do CT-e OS
*CteOsApi* | [**consultarCteOs**](docs/Apis/CteOsApi.md#consultarCteOs) | **GET** /cteos/{id} | Consultar CT-e OS
*CteOsApi* | [**consultarEventoCteOs**](docs/Apis/CteOsApi.md#consultarEventoCteOs) | **GET** /cteos/eventos/{id} | Consultar evento
*CteOsApi* | [**consultarStatusSefazCteOs**](docs/Apis/CteOsApi.md#consultarStatusSefazCteOs) | **GET** /cteos/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora
*CteOsApi* | [**criarCartaCorrecaoCteOs**](docs/Apis/CteOsApi.md#criarCartaCorrecaoCteOs) | **POST** /cteos/{id}/carta-correcao | Solicitar correção do CT-e OS
*CteOsApi* | [**emitirCteOs**](docs/Apis/CteOsApi.md#emitirCteOs) | **POST** /cteos | Emitir CT-e OS
*CteOsApi* | [**listarCteOs**](docs/Apis/CteOsApi.md#listarCteOs) | **GET** /cteos | Listar CT-e OS
*CteOsApi* | [**sincronizarCteOs**](docs/Apis/CteOsApi.md#sincronizarCteOs) | **POST** /cteos/{id}/sincronizar | Sincroniza dados no CT-e OS a partir da SEFAZ
*DceApi* | [**baixarPdfDce**](docs/Apis/DceApi.md#baixarPdfDce) | **GET** /dce/{id}/pdf | Baixar PDF do DACE
*DceApi* | [**baixarXmlCancelamentoDce**](docs/Apis/DceApi.md#baixarXmlCancelamentoDce) | **GET** /dce/{id}/cancelamento/xml | Baixar XML do cancelamento
*DceApi* | [**baixarXmlDce**](docs/Apis/DceApi.md#baixarXmlDce) | **GET** /dce/{id}/xml | Baixar XML da DC-e processada
*DceApi* | [**baixarXmlDceDeclaracao**](docs/Apis/DceApi.md#baixarXmlDceDeclaracao) | **GET** /dce/{id}/xml/declaracao | Baixar XML da DC-e
*DceApi* | [**baixarXmlDceProtocolo**](docs/Apis/DceApi.md#baixarXmlDceProtocolo) | **GET** /dce/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ
*DceApi* | [**cancelarDce**](docs/Apis/DceApi.md#cancelarDce) | **POST** /dce/{id}/cancelamento | Cancelar uma DC-e autorizada
*DceApi* | [**consultarCancelamentoDce**](docs/Apis/DceApi.md#consultarCancelamentoDce) | **GET** /dce/{id}/cancelamento | Consultar o cancelamento da DC-e
*DceApi* | [**consultarDce**](docs/Apis/DceApi.md#consultarDce) | **GET** /dce/{id} | Consultar DC-e
*DceApi* | [**consultarStatusSefazDce**](docs/Apis/DceApi.md#consultarStatusSefazDce) | **GET** /dce/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora
*DceApi* | [**emitirDce**](docs/Apis/DceApi.md#emitirDce) | **POST** /dce | Emitir DC-e
*DceApi* | [**listarDce**](docs/Apis/DceApi.md#listarDce) | **GET** /dce | Listar DC-e
*DebugApi* | [**debugDfe**](docs/Apis/DebugApi.md#debugDfe) | **GET** /debug/{id} | Debug de DF-e
*DebugApi* | [**debugDfeOriginalPayload**](docs/Apis/DebugApi.md#debugDfeOriginalPayload) | **GET** /debug/{id}/original-payload | Payload original recebido
*DebugApi* | [**debugHttpRequestContent**](docs/Apis/DebugApi.md#debugHttpRequestContent) | **GET** /debug/http-requests/{id}/request-content | Corpo da requisição HTTP
*DebugApi* | [**debugHttpResponseContent**](docs/Apis/DebugApi.md#debugHttpResponseContent) | **GET** /debug/http-requests/{id}/response-content | Corpo da resposta HTTP
*DistribuioNFEApi* | [**baixarPdfDocumentoDistribuicaoNfe**](docs/Apis/DistribuioNFEApi.md#baixarPdfDocumentoDistribuicaoNfe) | **GET** /distribuicao/nfe/documentos/{id}/pdf | Baixar PDF do documento
*DistribuioNFEApi* | [**baixarXmlDocumentoDistribuicaoNfe**](docs/Apis/DistribuioNFEApi.md#baixarXmlDocumentoDistribuicaoNfe) | **GET** /distribuicao/nfe/documentos/{id}/xml | Baixar XML do documento
*DistribuioNFEApi* | [**consultarDistribuicaoNfe**](docs/Apis/DistribuioNFEApi.md#consultarDistribuicaoNfe) | **GET** /distribuicao/nfe/{id} | Consultar distribuição
*DistribuioNFEApi* | [**consultarDocumentoDistribuicaoNfe**](docs/Apis/DistribuioNFEApi.md#consultarDocumentoDistribuicaoNfe) | **GET** /distribuicao/nfe/documentos/{id} | Consultar documento
*DistribuioNFEApi* | [**consultarManifestacaoNfe**](docs/Apis/DistribuioNFEApi.md#consultarManifestacaoNfe) | **GET** /distribuicao/nfe/manifestacoes/{id} | Consultar manifestação
*DistribuioNFEApi* | [**gerarDistribuicaoNfe**](docs/Apis/DistribuioNFEApi.md#gerarDistribuicaoNfe) | **POST** /distribuicao/nfe | Distribuir documentos
*DistribuioNFEApi* | [**listarDistribuicaoNfe**](docs/Apis/DistribuioNFEApi.md#listarDistribuicaoNfe) | **GET** /distribuicao/nfe | Listar distribuições
*DistribuioNFEApi* | [**listarDocumentoDistribuicaoNfe**](docs/Apis/DistribuioNFEApi.md#listarDocumentoDistribuicaoNfe) | **GET** /distribuicao/nfe/documentos | Listar documentos
*DistribuioNFEApi* | [**listarManifestacaoNfe**](docs/Apis/DistribuioNFEApi.md#listarManifestacaoNfe) | **GET** /distribuicao/nfe/manifestacoes | Listar Manifestações
*DistribuioNFEApi* | [**listarNfeSemManifestacao**](docs/Apis/DistribuioNFEApi.md#listarNfeSemManifestacao) | **GET** /distribuicao/nfe/notas-sem-manifestacao | Listar notas sem manifestação
*DistribuioNFEApi* | [**manifestarNfe**](docs/Apis/DistribuioNFEApi.md#manifestarNfe) | **POST** /distribuicao/nfe/manifestacoes | Manifestar nota
*EmailApi* | [**consultarEmail**](docs/Apis/EmailApi.md#consultarEmail) | **GET** /emails/{id} | Consultar e-mail
*EmailApi* | [**listarEmails**](docs/Apis/EmailApi.md#listarEmails) | **GET** /emails | Listar e-mails
*EmpresaApi* | [**alterarConfigCte**](docs/Apis/EmpresaApi.md#alterarConfigCte) | **PUT** /empresas/{cpf_cnpj}/cte | Alterar configuração de CT-e
*EmpresaApi* | [**alterarConfigCteOs**](docs/Apis/EmpresaApi.md#alterarConfigCteOs) | **PUT** /empresas/{cpf_cnpj}/cteos | Alterar configuração de CT-e OS
*EmpresaApi* | [**alterarConfigDce**](docs/Apis/EmpresaApi.md#alterarConfigDce) | **PUT** /empresas/{cpf_cnpj}/dce | Alterar configuração de DC-e
*EmpresaApi* | [**alterarConfigDistribuicaoNfe**](docs/Apis/EmpresaApi.md#alterarConfigDistribuicaoNfe) | **PUT** /empresas/{cpf_cnpj}/distnfe | Alterar configuração de Distribuição de NF-e
*EmpresaApi* | [**alterarConfigMdfe**](docs/Apis/EmpresaApi.md#alterarConfigMdfe) | **PUT** /empresas/{cpf_cnpj}/mdfe | Alterar configuração de MDF-e
*EmpresaApi* | [**alterarConfigNfce**](docs/Apis/EmpresaApi.md#alterarConfigNfce) | **PUT** /empresas/{cpf_cnpj}/nfce | Alterar configuração de NFC-e
*EmpresaApi* | [**alterarConfigNfcom**](docs/Apis/EmpresaApi.md#alterarConfigNfcom) | **PUT** /empresas/{cpf_cnpj}/nfcom | Alterar configuração de NFCom
*EmpresaApi* | [**alterarConfigNfe**](docs/Apis/EmpresaApi.md#alterarConfigNfe) | **PUT** /empresas/{cpf_cnpj}/nfe | Alterar configuração de NF-e
*EmpresaApi* | [**alterarConfigNfse**](docs/Apis/EmpresaApi.md#alterarConfigNfse) | **PUT** /empresas/{cpf_cnpj}/nfse | Alterar configuração de NFS-e
*EmpresaApi* | [**atualizarEmpresa**](docs/Apis/EmpresaApi.md#atualizarEmpresa) | **PUT** /empresas/{cpf_cnpj} | Alterar empresa
*EmpresaApi* | [**baixarLogotipoEmpresa**](docs/Apis/EmpresaApi.md#baixarLogotipoEmpresa) | **GET** /empresas/{cpf_cnpj}/logotipo | Baixar logotipo
*EmpresaApi* | [**cadastrarCertificadoEmpresa**](docs/Apis/EmpresaApi.md#cadastrarCertificadoEmpresa) | **PUT** /empresas/{cpf_cnpj}/certificado | Cadastrar certificado
*EmpresaApi* | [**consultarCertificadoEmpresa**](docs/Apis/EmpresaApi.md#consultarCertificadoEmpresa) | **GET** /empresas/{cpf_cnpj}/certificado | Consultar certificado
*EmpresaApi* | [**consultarConfigCte**](docs/Apis/EmpresaApi.md#consultarConfigCte) | **GET** /empresas/{cpf_cnpj}/cte | Consultar configuração de CT-e
*EmpresaApi* | [**consultarConfigCteOs**](docs/Apis/EmpresaApi.md#consultarConfigCteOs) | **GET** /empresas/{cpf_cnpj}/cteos | Consultar configuração de CT-e OS
*EmpresaApi* | [**consultarConfigDce**](docs/Apis/EmpresaApi.md#consultarConfigDce) | **GET** /empresas/{cpf_cnpj}/dce | Consultar configuração de DC-e
*EmpresaApi* | [**consultarConfigDistribuicaoNfe**](docs/Apis/EmpresaApi.md#consultarConfigDistribuicaoNfe) | **GET** /empresas/{cpf_cnpj}/distnfe | Consultar configuração de Distribuição de NF-e
*EmpresaApi* | [**consultarConfigMdfe**](docs/Apis/EmpresaApi.md#consultarConfigMdfe) | **GET** /empresas/{cpf_cnpj}/mdfe | Consultar configuração de MDF-e
*EmpresaApi* | [**consultarConfigNfce**](docs/Apis/EmpresaApi.md#consultarConfigNfce) | **GET** /empresas/{cpf_cnpj}/nfce | Consultar configuração de NFC-e
*EmpresaApi* | [**consultarConfigNfcom**](docs/Apis/EmpresaApi.md#consultarConfigNfcom) | **GET** /empresas/{cpf_cnpj}/nfcom | Consultar configuração de NFCom
*EmpresaApi* | [**consultarConfigNfe**](docs/Apis/EmpresaApi.md#consultarConfigNfe) | **GET** /empresas/{cpf_cnpj}/nfe | Consultar configuração de NF-e
*EmpresaApi* | [**consultarConfigNfse**](docs/Apis/EmpresaApi.md#consultarConfigNfse) | **GET** /empresas/{cpf_cnpj}/nfse | Consultar configuração de NFS-e
*EmpresaApi* | [**consultarEmpresa**](docs/Apis/EmpresaApi.md#consultarEmpresa) | **GET** /empresas/{cpf_cnpj} | Consultar empresa
*EmpresaApi* | [**criarEmpresa**](docs/Apis/EmpresaApi.md#criarEmpresa) | **POST** /empresas | Cadastrar empresa
*EmpresaApi* | [**enviarCertificadoEmpresa**](docs/Apis/EmpresaApi.md#enviarCertificadoEmpresa) | **PUT** /empresas/{cpf_cnpj}/certificado/upload | Upload de certificado
*EmpresaApi* | [**enviarLogotipoEmpresa**](docs/Apis/EmpresaApi.md#enviarLogotipoEmpresa) | **PUT** /empresas/{cpf_cnpj}/logotipo | Enviar logotipo
*EmpresaApi* | [**excluirCertificadoEmpresa**](docs/Apis/EmpresaApi.md#excluirCertificadoEmpresa) | **DELETE** /empresas/{cpf_cnpj}/certificado | Deletar certificado
*EmpresaApi* | [**excluirEmpresa**](docs/Apis/EmpresaApi.md#excluirEmpresa) | **DELETE** /empresas/{cpf_cnpj} | Deletar empresa
*EmpresaApi* | [**excluirLogotipoEmpresa**](docs/Apis/EmpresaApi.md#excluirLogotipoEmpresa) | **DELETE** /empresas/{cpf_cnpj}/logotipo | Deletar logotipo
*EmpresaApi* | [**listarCertificados**](docs/Apis/EmpresaApi.md#listarCertificados) | **GET** /empresas/certificados | Listar certificados
*EmpresaApi* | [**listarEmpresas**](docs/Apis/EmpresaApi.md#listarEmpresas) | **GET** /empresas | Listar empresas
*MdfeApi* | [**baixarPdfCancelamentoMdfe**](docs/Apis/MdfeApi.md#baixarPdfCancelamentoMdfe) | **GET** /mdfe/{id}/cancelamento/pdf | Baixar PDF do cancelamento
*MdfeApi* | [**baixarPdfEncerramentoMdfe**](docs/Apis/MdfeApi.md#baixarPdfEncerramentoMdfe) | **GET** /mdfe/{id}/encerramento/pdf | Baixar PDF do encerramento
*MdfeApi* | [**baixarPdfEventoMdfe**](docs/Apis/MdfeApi.md#baixarPdfEventoMdfe) | **GET** /mdfe/eventos/{id}/pdf | Baixar PDF do evento
*MdfeApi* | [**baixarPdfMdfe**](docs/Apis/MdfeApi.md#baixarPdfMdfe) | **GET** /mdfe/{id}/pdf | Baixar PDF do DAMDFE
*MdfeApi* | [**baixarXmlCancelamentoMdfe**](docs/Apis/MdfeApi.md#baixarXmlCancelamentoMdfe) | **GET** /mdfe/{id}/cancelamento/xml | Baixar XML do cancelamento
*MdfeApi* | [**baixarXmlEncerramentoMdfe**](docs/Apis/MdfeApi.md#baixarXmlEncerramentoMdfe) | **GET** /mdfe/{id}/encerramento/xml | Baixar XML do encerramento
*MdfeApi* | [**baixarXmlEventoMdfe**](docs/Apis/MdfeApi.md#baixarXmlEventoMdfe) | **GET** /mdfe/eventos/{id}/xml | Baixar XML do evento
*MdfeApi* | [**baixarXmlMdfe**](docs/Apis/MdfeApi.md#baixarXmlMdfe) | **GET** /mdfe/{id}/xml | Baixar XML do MDF-e processado
*MdfeApi* | [**baixarXmlMdfeManifesto**](docs/Apis/MdfeApi.md#baixarXmlMdfeManifesto) | **GET** /mdfe/{id}/xml/manifesto | Baixar XML do MDF-e
*MdfeApi* | [**baixarXmlMdfeProtocolo**](docs/Apis/MdfeApi.md#baixarXmlMdfeProtocolo) | **GET** /mdfe/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ
*MdfeApi* | [**cancelarMdfe**](docs/Apis/MdfeApi.md#cancelarMdfe) | **POST** /mdfe/{id}/cancelamento | Cancelar um MDF-e autorizado
*MdfeApi* | [**consultarCancelamentoMdfe**](docs/Apis/MdfeApi.md#consultarCancelamentoMdfe) | **GET** /mdfe/{id}/cancelamento | Consultar o cancelamento do MDF-e
*MdfeApi* | [**consultarEncerramentoMdfe**](docs/Apis/MdfeApi.md#consultarEncerramentoMdfe) | **GET** /mdfe/{id}/encerramento | Consultar encerramento do MDF-e
*MdfeApi* | [**consultarEventoMdfe**](docs/Apis/MdfeApi.md#consultarEventoMdfe) | **GET** /mdfe/eventos/{id} | Consultar evento do MDF-e
*MdfeApi* | [**consultarLoteMdfe**](docs/Apis/MdfeApi.md#consultarLoteMdfe) | **GET** /mdfe/lotes/{id} | Consultar lote de MDF-e
*MdfeApi* | [**consultarMdfe**](docs/Apis/MdfeApi.md#consultarMdfe) | **GET** /mdfe/{id} | Consultar manifesto
*MdfeApi* | [**consultarMdfeNaoEncerrados**](docs/Apis/MdfeApi.md#consultarMdfeNaoEncerrados) | **GET** /mdfe/nao-encerrados | Consulta MDF-e não encerrados
*MdfeApi* | [**consultarStatusSefazMdfe**](docs/Apis/MdfeApi.md#consultarStatusSefazMdfe) | **GET** /mdfe/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora
*MdfeApi* | [**emitirLoteMdfe**](docs/Apis/MdfeApi.md#emitirLoteMdfe) | **POST** /mdfe/lotes | Emitir lote de MDF-e
*MdfeApi* | [**emitirMdfe**](docs/Apis/MdfeApi.md#emitirMdfe) | **POST** /mdfe | Emitir MDF-e
*MdfeApi* | [**encerrarMdfe**](docs/Apis/MdfeApi.md#encerrarMdfe) | **POST** /mdfe/{id}/encerramento | Encerrar um MDF-e autorizado
*MdfeApi* | [**incluirCondutorMdfe**](docs/Apis/MdfeApi.md#incluirCondutorMdfe) | **POST** /mdfe/{id}/inclusao-condutor | Incluir um condutor em um MDF-e autorizado
*MdfeApi* | [**incluirDfeMdfe**](docs/Apis/MdfeApi.md#incluirDfeMdfe) | **POST** /mdfe/{id}/inclusao-dfe | Incluir um DF-e em um MDF-e autorizado
*MdfeApi* | [**listarLotesMdfe**](docs/Apis/MdfeApi.md#listarLotesMdfe) | **GET** /mdfe/lotes | Listar lotes de MDF-e
*MdfeApi* | [**listarMdfe**](docs/Apis/MdfeApi.md#listarMdfe) | **GET** /mdfe | Listar MDF-e
*MdfeApi* | [**sincronizarMdfe**](docs/Apis/MdfeApi.md#sincronizarMdfe) | **POST** /mdfe/{id}/sincronizar | Sincroniza dados no MDF-e a partir da SEFAZ
*NfceApi* | [**baixarEscPosNfce**](docs/Apis/NfceApi.md#baixarEscPosNfce) | **GET** /nfce/{id}/escpos | Comandos ESC/POS para impressão do DANFCE
*NfceApi* | [**baixarPdfCancelamentoNfce**](docs/Apis/NfceApi.md#baixarPdfCancelamentoNfce) | **GET** /nfce/{id}/cancelamento/pdf | Baixar PDF do cancelamento
*NfceApi* | [**baixarPdfEventoNfce**](docs/Apis/NfceApi.md#baixarPdfEventoNfce) | **GET** /nfce/eventos/{id}/pdf | Baixar PDF do evento
*NfceApi* | [**baixarPdfInutilizacaoNfce**](docs/Apis/NfceApi.md#baixarPdfInutilizacaoNfce) | **GET** /nfce/inutilizacoes/{id}/pdf | Baixar PDF da inutilização
*NfceApi* | [**baixarPdfNfce**](docs/Apis/NfceApi.md#baixarPdfNfce) | **GET** /nfce/{id}/pdf | Baixar PDF do DANFCE
*NfceApi* | [**baixarPreviaPdfNfce**](docs/Apis/NfceApi.md#baixarPreviaPdfNfce) | **POST** /nfce/previa/pdf | Prévia do PDF do DANFCE
*NfceApi* | [**baixarPreviaXmlNfce**](docs/Apis/NfceApi.md#baixarPreviaXmlNfce) | **POST** /nfce/previa/xml | Prévia do XML da NFC-e
*NfceApi* | [**baixarXmlCancelamentoNfce**](docs/Apis/NfceApi.md#baixarXmlCancelamentoNfce) | **GET** /nfce/{id}/cancelamento/xml | Baixar XML do cancelamento
*NfceApi* | [**baixarXmlEventoNfce**](docs/Apis/NfceApi.md#baixarXmlEventoNfce) | **GET** /nfce/eventos/{id}/xml | Baixar XML do evento
*NfceApi* | [**baixarXmlInutilizacaoNfce**](docs/Apis/NfceApi.md#baixarXmlInutilizacaoNfce) | **GET** /nfce/inutilizacoes/{id}/xml | Baixar XML da inutilização
*NfceApi* | [**baixarXmlNfce**](docs/Apis/NfceApi.md#baixarXmlNfce) | **GET** /nfce/{id}/xml | Baixar XML da NFC-e processada
*NfceApi* | [**baixarXmlNfceNota**](docs/Apis/NfceApi.md#baixarXmlNfceNota) | **GET** /nfce/{id}/xml/nota | Baixar XML da NFC-e
*NfceApi* | [**baixarXmlNfceProtocolo**](docs/Apis/NfceApi.md#baixarXmlNfceProtocolo) | **GET** /nfce/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ
*NfceApi* | [**cancelarNfce**](docs/Apis/NfceApi.md#cancelarNfce) | **POST** /nfce/{id}/cancelamento | Cancelar uma NFC-e autorizada
*NfceApi* | [**consultarCancelamentoNfce**](docs/Apis/NfceApi.md#consultarCancelamentoNfce) | **GET** /nfce/{id}/cancelamento | Consultar o cancelamento da NFC-e
*NfceApi* | [**consultarEventoNfce**](docs/Apis/NfceApi.md#consultarEventoNfce) | **GET** /nfce/eventos/{id} | Consultar evento
*NfceApi* | [**consultarInutilizacaoNfce**](docs/Apis/NfceApi.md#consultarInutilizacaoNfce) | **GET** /nfce/inutilizacoes/{id} | Consultar a inutilização de sequência de numeração
*NfceApi* | [**consultarLoteNfce**](docs/Apis/NfceApi.md#consultarLoteNfce) | **GET** /nfce/lotes/{id} | Consultar lote de NFC-e
*NfceApi* | [**consultarNfce**](docs/Apis/NfceApi.md#consultarNfce) | **GET** /nfce/{id} | Consultar NFC-e
*NfceApi* | [**consultarStatusSefazNfce**](docs/Apis/NfceApi.md#consultarStatusSefazNfce) | **GET** /nfce/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora
*NfceApi* | [**emitirLoteNfce**](docs/Apis/NfceApi.md#emitirLoteNfce) | **POST** /nfce/lotes | Emitir lote de NFC-e
*NfceApi* | [**emitirNfce**](docs/Apis/NfceApi.md#emitirNfce) | **POST** /nfce | Emitir NFC-e
*NfceApi* | [**enviarEmailNfce**](docs/Apis/NfceApi.md#enviarEmailNfce) | **POST** /nfce/{id}/email | Enviar e-mail
*NfceApi* | [**inutilizarNumeracaoNfce**](docs/Apis/NfceApi.md#inutilizarNumeracaoNfce) | **POST** /nfce/inutilizacoes | Inutilizar uma sequência de numeração de NFC-e
*NfceApi* | [**listarEventosNfce**](docs/Apis/NfceApi.md#listarEventosNfce) | **GET** /nfce/eventos | Listar eventos
*NfceApi* | [**listarLotesNfce**](docs/Apis/NfceApi.md#listarLotesNfce) | **GET** /nfce/lotes | Listar lotes de NFC-e
*NfceApi* | [**listarNfce**](docs/Apis/NfceApi.md#listarNfce) | **GET** /nfce | Listar NFC-e
*NfceApi* | [**sincronizarNfce**](docs/Apis/NfceApi.md#sincronizarNfce) | **POST** /nfce/{id}/sincronizar | Sincroniza dados na NFC-e a partir da SEFAZ
*NfcomApi* | [**baixarPdfNfcom**](docs/Apis/NfcomApi.md#baixarPdfNfcom) | **GET** /nfcom/{id}/pdf | Baixar PDF do DANFE-COM
*NfcomApi* | [**baixarXmlCancelamentoNfcom**](docs/Apis/NfcomApi.md#baixarXmlCancelamentoNfcom) | **GET** /nfcom/{id}/cancelamento/xml | Baixar XML do cancelamento
*NfcomApi* | [**baixarXmlNfcom**](docs/Apis/NfcomApi.md#baixarXmlNfcom) | **GET** /nfcom/{id}/xml | Baixar XML da NFCom processada
*NfcomApi* | [**baixarXmlNfcomNota**](docs/Apis/NfcomApi.md#baixarXmlNfcomNota) | **GET** /nfcom/{id}/xml/nota | Baixar XML da NFCom
*NfcomApi* | [**baixarXmlNfcomProtocolo**](docs/Apis/NfcomApi.md#baixarXmlNfcomProtocolo) | **GET** /nfcom/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ
*NfcomApi* | [**cancelarNfcom**](docs/Apis/NfcomApi.md#cancelarNfcom) | **POST** /nfcom/{id}/cancelamento | Cancelar uma NFCom autorizada
*NfcomApi* | [**consultarCancelamentoNfcom**](docs/Apis/NfcomApi.md#consultarCancelamentoNfcom) | **GET** /nfcom/{id}/cancelamento | Consultar o cancelamento da NFCom
*NfcomApi* | [**consultarNfcom**](docs/Apis/NfcomApi.md#consultarNfcom) | **GET** /nfcom/{id} | Consultar NFCom
*NfcomApi* | [**consultarStatusSefazNfcom**](docs/Apis/NfcomApi.md#consultarStatusSefazNfcom) | **GET** /nfcom/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora
*NfcomApi* | [**emitirNfcom**](docs/Apis/NfcomApi.md#emitirNfcom) | **POST** /nfcom | Emitir NFCom
*NfcomApi* | [**listarNfcom**](docs/Apis/NfcomApi.md#listarNfcom) | **GET** /nfcom | Listar NFCom
*NfeApi* | [**baixarPdfCancelamentoNfe**](docs/Apis/NfeApi.md#baixarPdfCancelamentoNfe) | **GET** /nfe/{id}/cancelamento/pdf | Baixar PDF do cancelamento
*NfeApi* | [**baixarPdfCartaCorrecaoNfe**](docs/Apis/NfeApi.md#baixarPdfCartaCorrecaoNfe) | **GET** /nfe/{id}/carta-correcao/pdf | Baixar PDF da carta de correção
*NfeApi* | [**baixarPdfEventoNfe**](docs/Apis/NfeApi.md#baixarPdfEventoNfe) | **GET** /nfe/eventos/{id}/pdf | Baixar PDF do evento
*NfeApi* | [**baixarPdfInutilizacaoNfe**](docs/Apis/NfeApi.md#baixarPdfInutilizacaoNfe) | **GET** /nfe/inutilizacoes/{id}/pdf | Baixar PDF da inutilização
*NfeApi* | [**baixarPdfNfe**](docs/Apis/NfeApi.md#baixarPdfNfe) | **GET** /nfe/{id}/pdf | Baixar PDF do DANFE
*NfeApi* | [**baixarPreviaPdfNfe**](docs/Apis/NfeApi.md#baixarPreviaPdfNfe) | **POST** /nfe/previa/pdf | Prévia do PDF do DANFE
*NfeApi* | [**baixarPreviaXmlNfe**](docs/Apis/NfeApi.md#baixarPreviaXmlNfe) | **POST** /nfe/previa/xml | Prévia do XML da NF-e
*NfeApi* | [**baixarXmlCancelamentoNfe**](docs/Apis/NfeApi.md#baixarXmlCancelamentoNfe) | **GET** /nfe/{id}/cancelamento/xml | Baixar XML do cancelamento
*NfeApi* | [**baixarXmlCartaCorrecaoNfe**](docs/Apis/NfeApi.md#baixarXmlCartaCorrecaoNfe) | **GET** /nfe/{id}/carta-correcao/xml | Baixar XML da carta de correção
*NfeApi* | [**baixarXmlEventoNfe**](docs/Apis/NfeApi.md#baixarXmlEventoNfe) | **GET** /nfe/eventos/{id}/xml | Baixar XML do evento
*NfeApi* | [**baixarXmlInutilizacaoNfe**](docs/Apis/NfeApi.md#baixarXmlInutilizacaoNfe) | **GET** /nfe/inutilizacoes/{id}/xml | Baixar XML da inutilização
*NfeApi* | [**baixarXmlNfe**](docs/Apis/NfeApi.md#baixarXmlNfe) | **GET** /nfe/{id}/xml | Baixar XML da NF-e processada
*NfeApi* | [**baixarXmlNfeNota**](docs/Apis/NfeApi.md#baixarXmlNfeNota) | **GET** /nfe/{id}/xml/nota | Baixar XML da NF-e
*NfeApi* | [**baixarXmlNfeProtocolo**](docs/Apis/NfeApi.md#baixarXmlNfeProtocolo) | **GET** /nfe/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ
*NfeApi* | [**cancelarNfe**](docs/Apis/NfeApi.md#cancelarNfe) | **POST** /nfe/{id}/cancelamento | Cancelar uma NF-e autorizada
*NfeApi* | [**consultarCancelamentoNfe**](docs/Apis/NfeApi.md#consultarCancelamentoNfe) | **GET** /nfe/{id}/cancelamento | Consultar o cancelamento da NF-e
*NfeApi* | [**consultarCartaCorrecaoNfe**](docs/Apis/NfeApi.md#consultarCartaCorrecaoNfe) | **GET** /nfe/{id}/carta-correcao | Consultar a solicitação de correção da NF-e
*NfeApi* | [**consultarContribuinteNfe**](docs/Apis/NfeApi.md#consultarContribuinteNfe) | **GET** /nfe/cadastro-contribuinte | Consultar contribuinte
*NfeApi* | [**consultarEventoNfe**](docs/Apis/NfeApi.md#consultarEventoNfe) | **GET** /nfe/eventos/{id} | Consultar evento
*NfeApi* | [**consultarInutilizacaoNfe**](docs/Apis/NfeApi.md#consultarInutilizacaoNfe) | **GET** /nfe/inutilizacoes/{id} | Consultar a inutilização de sequência de numeração
*NfeApi* | [**consultarLoteNfe**](docs/Apis/NfeApi.md#consultarLoteNfe) | **GET** /nfe/lotes/{id} | Consultar lote de NF-e
*NfeApi* | [**consultarNfe**](docs/Apis/NfeApi.md#consultarNfe) | **GET** /nfe/{id} | Consultar NF-e
*NfeApi* | [**consultarStatusSefazNfe**](docs/Apis/NfeApi.md#consultarStatusSefazNfe) | **GET** /nfe/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora
*NfeApi* | [**criarCartaCorrecaoNfe**](docs/Apis/NfeApi.md#criarCartaCorrecaoNfe) | **POST** /nfe/{id}/carta-correcao | Solicitar correção da NF-e
*NfeApi* | [**emitirLoteNfe**](docs/Apis/NfeApi.md#emitirLoteNfe) | **POST** /nfe/lotes | Emitir lote de NF-e
*NfeApi* | [**emitirNfe**](docs/Apis/NfeApi.md#emitirNfe) | **POST** /nfe | Emitir NF-e
*NfeApi* | [**enviarEmailNfe**](docs/Apis/NfeApi.md#enviarEmailNfe) | **POST** /nfe/{id}/email | Enviar e-mail
*NfeApi* | [**inutilizarNumeracaoNfe**](docs/Apis/NfeApi.md#inutilizarNumeracaoNfe) | **POST** /nfe/inutilizacoes | Inutilizar uma sequência de numeração de NF-e
*NfeApi* | [**listarEventosNfe**](docs/Apis/NfeApi.md#listarEventosNfe) | **GET** /nfe/eventos | Listar eventos
*NfeApi* | [**listarLotesNfe**](docs/Apis/NfeApi.md#listarLotesNfe) | **GET** /nfe/lotes | Listar lotes de NF-e
*NfeApi* | [**listarNfe**](docs/Apis/NfeApi.md#listarNfe) | **GET** /nfe | Listar NF-e
*NfeApi* | [**sincronizarNfe**](docs/Apis/NfeApi.md#sincronizarNfe) | **POST** /nfe/{id}/sincronizar | Sincroniza dados na NF-e a partir da SEFAZ
*NfseApi* | [**baixarPdfNfse**](docs/Apis/NfseApi.md#baixarPdfNfse) | **GET** /nfse/{id}/pdf | Baixar PDF do DANFSE
*NfseApi* | [**baixarXmlCancelamentoNfse**](docs/Apis/NfseApi.md#baixarXmlCancelamentoNfse) | **GET** /nfse/{Id}/cancelamento/xml | Baixar XML do evento de cancelamento
*NfseApi* | [**baixarXmlDps**](docs/Apis/NfseApi.md#baixarXmlDps) | **GET** /nfse/{id}/xml/dps | Baixar XML da DPS
*NfseApi* | [**baixarXmlNfse**](docs/Apis/NfseApi.md#baixarXmlNfse) | **GET** /nfse/{id}/xml | Baixar XML da NFS-e processada
*NfseApi* | [**cancelarNfse**](docs/Apis/NfseApi.md#cancelarNfse) | **POST** /nfse/{id}/cancelamento | Cancelar uma NFS-e autorizada
*NfseApi* | [**cidadesAtendidas**](docs/Apis/NfseApi.md#cidadesAtendidas) | **GET** /nfse/cidades | Cidades atendidas
*NfseApi* | [**consultarCancelamentoNfse**](docs/Apis/NfseApi.md#consultarCancelamentoNfse) | **GET** /nfse/{id}/cancelamento | Consultar o cancelamento da NFS-e
*NfseApi* | [**consultarLoteNfse**](docs/Apis/NfseApi.md#consultarLoteNfse) | **GET** /nfse/lotes/{id} | Consultar lote de NFS-e
*NfseApi* | [**consultarMetadados**](docs/Apis/NfseApi.md#consultarMetadados) | **GET** /nfse/cidades/{codigo_ibge} | Consultar metadados
*NfseApi* | [**consultarNfse**](docs/Apis/NfseApi.md#consultarNfse) | **GET** /nfse/{id} | Consultar NFS-e
*NfseApi* | [**emitirLoteNfse**](docs/Apis/NfseApi.md#emitirLoteNfse) | **POST** /nfse/lotes | Emitir lote de NFS-e
*NfseApi* | [**emitirLoteNfseDps**](docs/Apis/NfseApi.md#emitirLoteNfseDps) | **POST** /nfse/dps/lotes | Emitir lote de NFS-e
*NfseApi* | [**emitirNfse**](docs/Apis/NfseApi.md#emitirNfse) | **POST** /nfse | Emitir NFS-e
*NfseApi* | [**emitirNfseDps**](docs/Apis/NfseApi.md#emitirNfseDps) | **POST** /nfse/dps | Emitir NFS-e
*NfseApi* | [**listarLotesNfse**](docs/Apis/NfseApi.md#listarLotesNfse) | **GET** /nfse/lotes | Listar lotes de NFS-e
*NfseApi* | [**listarNfse**](docs/Apis/NfseApi.md#listarNfse) | **GET** /nfse | Listar NFS-e
*NfseApi* | [**sincronizarNfse**](docs/Apis/NfseApi.md#sincronizarNfse) | **POST** /nfse/{id}/sincronizar | Sincroniza dados na NFS-e a partir da Prefeitura


<a name="documentation-for-models"></a>
## Documentação dos DTOs

 - [AtvEvento](docs/Models/AtvEvento.md)
 - [BeneficioMunicipal](docs/Models/BeneficioMunicipal.md)
 - [CServ](docs/Models/CServ.md)
 - [CepEndereco](docs/Models/CepEndereco.md)
 - [CnpjCnae](docs/Models/CnpjCnae.md)
 - [CnpjCnaeSecundario](docs/Models/CnpjCnaeSecundario.md)
 - [CnpjEmpresa](docs/Models/CnpjEmpresa.md)
 - [CnpjEndereco](docs/Models/CnpjEndereco.md)
 - [CnpjFaixaEtaria](docs/Models/CnpjFaixaEtaria.md)
 - [CnpjIdentificadorSocio](docs/Models/CnpjIdentificadorSocio.md)
 - [CnpjListagem](docs/Models/CnpjListagem.md)
 - [CnpjMotivoSituacaoCadastral](docs/Models/CnpjMotivoSituacaoCadastral.md)
 - [CnpjMunicipio](docs/Models/CnpjMunicipio.md)
 - [CnpjNaturezaJuridica](docs/Models/CnpjNaturezaJuridica.md)
 - [CnpjOpcaoSimei](docs/Models/CnpjOpcaoSimei.md)
 - [CnpjOpcaoSimples](docs/Models/CnpjOpcaoSimples.md)
 - [CnpjPais](docs/Models/CnpjPais.md)
 - [CnpjPorteEmpresa](docs/Models/CnpjPorteEmpresa.md)
 - [CnpjQualificacaoSocio](docs/Models/CnpjQualificacaoSocio.md)
 - [CnpjRepresentanteLegal](docs/Models/CnpjRepresentanteLegal.md)
 - [CnpjSituacaoCadastral](docs/Models/CnpjSituacaoCadastral.md)
 - [CnpjSituacaoEspecial](docs/Models/CnpjSituacaoEspecial.md)
 - [CnpjSocio](docs/Models/CnpjSocio.md)
 - [CnpjTelefone](docs/Models/CnpjTelefone.md)
 - [ComExterior](docs/Models/ComExterior.md)
 - [ContaCota](docs/Models/ContaCota.md)
 - [ContaCotaListagem](docs/Models/ContaCotaListagem.md)
 - [ContaCotaPrePago](docs/Models/ContaCotaPrePago.md)
 - [ContaExtratoCredito](docs/Models/ContaExtratoCredito.md)
 - [ContaExtratoCreditoListagem](docs/Models/ContaExtratoCreditoListagem.md)
 - [CteCartaCorrecao](docs/Models/CteCartaCorrecao.md)
 - [CteInfCorrecao](docs/Models/CteInfCorrecao.md)
 - [CteOsCartaCorrecao](docs/Models/CteOsCartaCorrecao.md)
 - [CteOsInfCorrecao](docs/Models/CteOsInfCorrecao.md)
 - [CteOsPedidoCancelamento](docs/Models/CteOsPedidoCancelamento.md)
 - [CteOsPedidoCartaCorrecao](docs/Models/CteOsPedidoCartaCorrecao.md)
 - [CteOsPedidoEmissao](docs/Models/CteOsPedidoEmissao.md)
 - [CteOsSefazALCZFMCBSOS](docs/Models/CteOsSefazALCZFMCBSOS.md)
 - [CteOsSefazAutXMLOS](docs/Models/CteOsSefazAutXMLOS.md)
 - [CteOsSefazCIBSOS](docs/Models/CteOsSefazCIBSOS.md)
 - [CteOsSefazCobrOS](docs/Models/CteOsSefazCobrOS.md)
 - [CteOsSefazCompOS](docs/Models/CteOsSefazCompOS.md)
 - [CteOsSefazComplOS](docs/Models/CteOsSefazComplOS.md)
 - [CteOsSefazCompraGovReduzidoOS](docs/Models/CteOsSefazCompraGovReduzidoOS.md)
 - [CteOsSefazDevTribOS](docs/Models/CteOsSefazDevTribOS.md)
 - [CteOsSefazDifOS](docs/Models/CteOsSefazDifOS.md)
 - [CteOsSefazDupOS](docs/Models/CteOsSefazDupOS.md)
 - [CteOsSefazEmitOS](docs/Models/CteOsSefazEmitOS.md)
 - [CteOsSefazEndeEmiOS](docs/Models/CteOsSefazEndeEmiOS.md)
 - [CteOsSefazEnderecoOS](docs/Models/CteOsSefazEnderecoOS.md)
 - [CteOsSefazEstornoCredOS](docs/Models/CteOsSefazEstornoCredOS.md)
 - [CteOsSefazFatOS](docs/Models/CteOsSefazFatOS.md)
 - [CteOsSefazGCBSOS](docs/Models/CteOsSefazGCBSOS.md)
 - [CteOsSefazGIBSMunOS](docs/Models/CteOsSefazGIBSMunOS.md)
 - [CteOsSefazGIBSUFOS](docs/Models/CteOsSefazGIBSUFOS.md)
 - [CteOsSefazGPagAntecipadoOS](docs/Models/CteOsSefazGPagAntecipadoOS.md)
 - [CteOsSefazICMS00OS](docs/Models/CteOsSefazICMS00OS.md)
 - [CteOsSefazICMS20OS](docs/Models/CteOsSefazICMS20OS.md)
 - [CteOsSefazICMS45OS](docs/Models/CteOsSefazICMS45OS.md)
 - [CteOsSefazICMS90OS](docs/Models/CteOsSefazICMS90OS.md)
 - [CteOsSefazICMSOutraUFOS](docs/Models/CteOsSefazICMSOutraUFOS.md)
 - [CteOsSefazICMSSNOS](docs/Models/CteOsSefazICMSSNOS.md)
 - [CteOsSefazICMSUFFimOS](docs/Models/CteOsSefazICMSUFFimOS.md)
 - [CteOsSefazIdeOS](docs/Models/CteOsSefazIdeOS.md)
 - [CteOsSefazImpOS](docs/Models/CteOsSefazImpOS.md)
 - [CteOsSefazInfCTeNormOS](docs/Models/CteOsSefazInfCTeNormOS.md)
 - [CteOsSefazInfCTeSuplOS](docs/Models/CteOsSefazInfCTeSuplOS.md)
 - [CteOsSefazInfCteCompOS](docs/Models/CteOsSefazInfCteCompOS.md)
 - [CteOsSefazInfCteImpOS](docs/Models/CteOsSefazInfCte_ImpOS.md)
 - [CteOsSefazInfCteOS](docs/Models/CteOsSefazInfCteOS.md)
 - [CteOsSefazInfCteSubOS](docs/Models/CteOsSefazInfCteSubOS.md)
 - [CteOsSefazInfDocRefOS](docs/Models/CteOsSefazInfDocRefOS.md)
 - [CteOsSefazInfFretamentoOS](docs/Models/CteOsSefazInfFretamentoOS.md)
 - [CteOsSefazInfGTVeCompOS](docs/Models/CteOsSefazInfGTVe_CompOS.md)
 - [CteOsSefazInfGTVeOS](docs/Models/CteOsSefazInfGTVeOS.md)
 - [CteOsSefazInfModalOS](docs/Models/CteOsSefazInfModalOS.md)
 - [CteOsSefazInfPercursoOS](docs/Models/CteOsSefazInfPercursoOS.md)
 - [CteOsSefazInfQOS](docs/Models/CteOsSefazInfQOS.md)
 - [CteOsSefazInfServicoOS](docs/Models/CteOsSefazInfServicoOS.md)
 - [CteOsSefazInfTribFedOS](docs/Models/CteOsSefazInfTribFedOS.md)
 - [CteOsSefazObsContOS](docs/Models/CteOsSefazObsContOS.md)
 - [CteOsSefazObsFiscoOS](docs/Models/CteOsSefazObsFiscoOS.md)
 - [CteOsSefazPagamentoRTCOS](docs/Models/CteOsSefazPagamentoRTCOS.md)
 - [CteOsSefazPgtoVincOS](docs/Models/CteOsSefazPgtoVincOS.md)
 - [CteOsSefazPropOS](docs/Models/CteOsSefazPropOS.md)
 - [CteOsSefazRedOS](docs/Models/CteOsSefazRedOS.md)
 - [CteOsSefazRespTecOS](docs/Models/CteOsSefazRespTecOS.md)
 - [CteOsSefazRodoOS](docs/Models/CteOsSefazRodoOS.md)
 - [CteOsSefazSegOS](docs/Models/CteOsSefazSegOS.md)
 - [CteOsSefazTomaOS](docs/Models/CteOsSefazTomaOS.md)
 - [CteOsSefazTribCTeOS](docs/Models/CteOsSefazTribCTeOS.md)
 - [CteOsSefazTribCompraGovOS](docs/Models/CteOsSefazTribCompraGovOS.md)
 - [CteOsSefazTribRegularOS](docs/Models/CteOsSefazTribRegularOS.md)
 - [CteOsSefazVPrestOS](docs/Models/CteOsSefazVPrestOS.md)
 - [CteOsSefazVeicOS](docs/Models/CteOsSefazVeicOS.md)
 - [CtePedidoCancelamento](docs/Models/CtePedidoCancelamento.md)
 - [CtePedidoCartaCorrecao](docs/Models/CtePedidoCartaCorrecao.md)
 - [CtePedidoEmissao](docs/Models/CtePedidoEmissao.md)
 - [CteSefazALCZFMCBS](docs/Models/CteSefazALCZFMCBS.md)
 - [CteSefazAereo](docs/Models/CteSefazAereo.md)
 - [CteSefazAquav](docs/Models/CteSefazAquav.md)
 - [CteSefazAutXML](docs/Models/CteSefazAutXML.md)
 - [CteSefazBalsa](docs/Models/CteSefazBalsa.md)
 - [CteSefazCIBS](docs/Models/CteSefazCIBS.md)
 - [CteSefazCobr](docs/Models/CteSefazCobr.md)
 - [CteSefazComData](docs/Models/CteSefazComData.md)
 - [CteSefazComHora](docs/Models/CteSefazComHora.md)
 - [CteSefazComp](docs/Models/CteSefazComp.md)
 - [CteSefazCompl](docs/Models/CteSefazCompl.md)
 - [CteSefazCompraGovReduzido](docs/Models/CteSefazCompraGovReduzido.md)
 - [CteSefazDest](docs/Models/CteSefazDest.md)
 - [CteSefazDetCont](docs/Models/CteSefazDetCont.md)
 - [CteSefazDetContInfDoc](docs/Models/CteSefazDetCont_InfDoc.md)
 - [CteSefazDetContInfDocInfNF](docs/Models/CteSefazDetCont_InfDoc_InfNF.md)
 - [CteSefazDetContInfDocInfNFe](docs/Models/CteSefazDetCont_InfDoc_InfNFe.md)
 - [CteSefazDevTrib](docs/Models/CteSefazDevTrib.md)
 - [CteSefazDif](docs/Models/CteSefazDif.md)
 - [CteSefazDocAnt](docs/Models/CteSefazDocAnt.md)
 - [CteSefazDup](docs/Models/CteSefazDup.md)
 - [CteSefazDuto](docs/Models/CteSefazDuto.md)
 - [CteSefazEmiDocAnt](docs/Models/CteSefazEmiDocAnt.md)
 - [CteSefazEmiOcc](docs/Models/CteSefazEmiOcc.md)
 - [CteSefazEmit](docs/Models/CteSefazEmit.md)
 - [CteSefazEndeEmi](docs/Models/CteSefazEndeEmi.md)
 - [CteSefazEnderFer](docs/Models/CteSefazEnderFer.md)
 - [CteSefazEndereco](docs/Models/CteSefazEndereco.md)
 - [CteSefazEntrega](docs/Models/CteSefazEntrega.md)
 - [CteSefazEstornoCred](docs/Models/CteSefazEstornoCred.md)
 - [CteSefazExped](docs/Models/CteSefazExped.md)
 - [CteSefazFat](docs/Models/CteSefazFat.md)
 - [CteSefazFerroEnv](docs/Models/CteSefazFerroEnv.md)
 - [CteSefazFerrov](docs/Models/CteSefazFerrov.md)
 - [CteSefazFluxo](docs/Models/CteSefazFluxo.md)
 - [CteSefazGCBS](docs/Models/CteSefazGCBS.md)
 - [CteSefazGIBSMun](docs/Models/CteSefazGIBSMun.md)
 - [CteSefazGIBSUF](docs/Models/CteSefazGIBSUF.md)
 - [CteSefazGPagAntecipado](docs/Models/CteSefazGPagAntecipado.md)
 - [CteSefazICMS00](docs/Models/CteSefazICMS00.md)
 - [CteSefazICMS20](docs/Models/CteSefazICMS20.md)
 - [CteSefazICMS45](docs/Models/CteSefazICMS45.md)
 - [CteSefazICMS60](docs/Models/CteSefazICMS60.md)
 - [CteSefazICMS90](docs/Models/CteSefazICMS90.md)
 - [CteSefazICMSOutraUF](docs/Models/CteSefazICMSOutraUF.md)
 - [CteSefazICMSSN](docs/Models/CteSefazICMSSN.md)
 - [CteSefazICMSUFFim](docs/Models/CteSefazICMSUFFim.md)
 - [CteSefazIdDocAnt](docs/Models/CteSefazIdDocAnt.md)
 - [CteSefazIdDocAntEle](docs/Models/CteSefazIdDocAntEle.md)
 - [CteSefazIdDocAntPap](docs/Models/CteSefazIdDocAntPap.md)
 - [CteSefazIde](docs/Models/CteSefazIde.md)
 - [CteSefazImp](docs/Models/CteSefazImp.md)
 - [CteSefazInfCTeMultimodal](docs/Models/CteSefazInfCTeMultimodal.md)
 - [CteSefazInfCTeNorm](docs/Models/CteSefazInfCTeNorm.md)
 - [CteSefazInfCTeSupl](docs/Models/CteSefazInfCTeSupl.md)
 - [CteSefazInfCarga](docs/Models/CteSefazInfCarga.md)
 - [CteSefazInfCte](docs/Models/CteSefazInfCte.md)
 - [CteSefazInfCteComp](docs/Models/CteSefazInfCteComp.md)
 - [CteSefazInfCteImp](docs/Models/CteSefazInfCte_Imp.md)
 - [CteSefazInfCteSub](docs/Models/CteSefazInfCteSub.md)
 - [CteSefazInfDCe](docs/Models/CteSefazInfDCe.md)
 - [CteSefazInfDoc](docs/Models/CteSefazInfDoc.md)
 - [CteSefazInfGlobalizado](docs/Models/CteSefazInfGlobalizado.md)
 - [CteSefazInfModal](docs/Models/CteSefazInfModal.md)
 - [CteSefazInfNF](docs/Models/CteSefazInfNF.md)
 - [CteSefazInfNFe](docs/Models/CteSefazInfNFe.md)
 - [CteSefazInfOutros](docs/Models/CteSefazInfOutros.md)
 - [CteSefazInfQ](docs/Models/CteSefazInfQ.md)
 - [CteSefazInfSeg](docs/Models/CteSefazInfSeg.md)
 - [CteSefazInfServVinc](docs/Models/CteSefazInfServVinc.md)
 - [CteSefazInfSolicNFF](docs/Models/CteSefazInfSolicNFF.md)
 - [CteSefazInfTotAP](docs/Models/CteSefazInfTotAP.md)
 - [CteSefazLacUnidCarga](docs/Models/CteSefazLacUnidCarga.md)
 - [CteSefazLacUnidTransp](docs/Models/CteSefazLacUnidTransp.md)
 - [CteSefazLacre](docs/Models/CteSefazLacre.md)
 - [CteSefazMultimodal](docs/Models/CteSefazMultimodal.md)
 - [CteSefazNatCarga](docs/Models/CteSefazNatCarga.md)
 - [CteSefazNoInter](docs/Models/CteSefazNoInter.md)
 - [CteSefazNoPeriodo](docs/Models/CteSefazNoPeriodo.md)
 - [CteSefazObsCont](docs/Models/CteSefazObsCont.md)
 - [CteSefazObsFisco](docs/Models/CteSefazObsFisco.md)
 - [CteSefazOcc](docs/Models/CteSefazOcc.md)
 - [CteSefazPagamentoRTC](docs/Models/CteSefazPagamentoRTC.md)
 - [CteSefazPass](docs/Models/CteSefazPass.md)
 - [CteSefazPeri](docs/Models/CteSefazPeri.md)
 - [CteSefazPgtoVinc](docs/Models/CteSefazPgtoVinc.md)
 - [CteSefazReceb](docs/Models/CteSefazReceb.md)
 - [CteSefazRed](docs/Models/CteSefazRed.md)
 - [CteSefazRem](docs/Models/CteSefazRem.md)
 - [CteSefazRespTec](docs/Models/CteSefazRespTec.md)
 - [CteSefazRodo](docs/Models/CteSefazRodo.md)
 - [CteSefazSeg](docs/Models/CteSefazSeg.md)
 - [CteSefazSemData](docs/Models/CteSefazSemData.md)
 - [CteSefazSemHora](docs/Models/CteSefazSemHora.md)
 - [CteSefazTarifa](docs/Models/CteSefazTarifa.md)
 - [CteSefazToma3](docs/Models/CteSefazToma3.md)
 - [CteSefazToma4](docs/Models/CteSefazToma4.md)
 - [CteSefazTrafMut](docs/Models/CteSefazTrafMut.md)
 - [CteSefazTribCTe](docs/Models/CteSefazTribCTe.md)
 - [CteSefazTribCompraGov](docs/Models/CteSefazTribCompraGov.md)
 - [CteSefazTribRegular](docs/Models/CteSefazTribRegular.md)
 - [CteSefazUnidCarga](docs/Models/CteSefazUnidCarga.md)
 - [CteSefazUnidadeTransp](docs/Models/CteSefazUnidadeTransp.md)
 - [CteSefazVPrest](docs/Models/CteSefazVPrest.md)
 - [CteSefazVeicNovos](docs/Models/CteSefazVeicNovos.md)
 - [CteSimpPedidoEmissao](docs/Models/CteSimpPedidoEmissao.md)
 - [CteSimpSefazALCZFMCBSSimp](docs/Models/CteSimpSefazALCZFMCBSSimp.md)
 - [CteSimpSefazAereoSimp](docs/Models/CteSimpSefazAereoSimp.md)
 - [CteSimpSefazAquavSimp](docs/Models/CteSimpSefazAquavSimp.md)
 - [CteSimpSefazAutXMLSimp](docs/Models/CteSimpSefazAutXMLSimp.md)
 - [CteSimpSefazBalsaSimp](docs/Models/CteSimpSefazBalsaSimp.md)
 - [CteSimpSefazCIBSSimp](docs/Models/CteSimpSefazCIBSSimp.md)
 - [CteSimpSefazCobrSimp](docs/Models/CteSimpSefazCobrSimp.md)
 - [CteSimpSefazCompSimp](docs/Models/CteSimpSefazCompSimp.md)
 - [CteSimpSefazComplSimp](docs/Models/CteSimpSefazComplSimp.md)
 - [CteSimpSefazCompraGovReduzidoSimp](docs/Models/CteSimpSefazCompraGovReduzidoSimp.md)
 - [CteSimpSefazDetContSimp](docs/Models/CteSimpSefazDetContSimp.md)
 - [CteSimpSefazDetSimp](docs/Models/CteSimpSefazDetSimp.md)
 - [CteSimpSefazDevTribSimp](docs/Models/CteSimpSefazDevTribSimp.md)
 - [CteSimpSefazDifSimp](docs/Models/CteSimpSefazDifSimp.md)
 - [CteSimpSefazDupSimp](docs/Models/CteSimpSefazDupSimp.md)
 - [CteSimpSefazDutoSimp](docs/Models/CteSimpSefazDutoSimp.md)
 - [CteSimpSefazEmiOccSimp](docs/Models/CteSimpSefazEmiOccSimp.md)
 - [CteSimpSefazEmitSimp](docs/Models/CteSimpSefazEmitSimp.md)
 - [CteSimpSefazEndeEmiSimp](docs/Models/CteSimpSefazEndeEmiSimp.md)
 - [CteSimpSefazEnderFerSimp](docs/Models/CteSimpSefazEnderFerSimp.md)
 - [CteSimpSefazEnderecoSimp](docs/Models/CteSimpSefazEnderecoSimp.md)
 - [CteSimpSefazEstornoCredSimp](docs/Models/CteSimpSefazEstornoCredSimp.md)
 - [CteSimpSefazFatSimp](docs/Models/CteSimpSefazFatSimp.md)
 - [CteSimpSefazFerroEnvSimp](docs/Models/CteSimpSefazFerroEnvSimp.md)
 - [CteSimpSefazFerrovSimp](docs/Models/CteSimpSefazFerrovSimp.md)
 - [CteSimpSefazFluxoSimp](docs/Models/CteSimpSefazFluxoSimp.md)
 - [CteSimpSefazGCBSSimp](docs/Models/CteSimpSefazGCBSSimp.md)
 - [CteSimpSefazGIBSMunSimp](docs/Models/CteSimpSefazGIBSMunSimp.md)
 - [CteSimpSefazGIBSUFSimp](docs/Models/CteSimpSefazGIBSUFSimp.md)
 - [CteSimpSefazGPagAntecipadoSimp](docs/Models/CteSimpSefazGPagAntecipadoSimp.md)
 - [CteSimpSefazICMS00Simp](docs/Models/CteSimpSefazICMS00Simp.md)
 - [CteSimpSefazICMS20Simp](docs/Models/CteSimpSefazICMS20Simp.md)
 - [CteSimpSefazICMS45Simp](docs/Models/CteSimpSefazICMS45Simp.md)
 - [CteSimpSefazICMS60Simp](docs/Models/CteSimpSefazICMS60Simp.md)
 - [CteSimpSefazICMS90Simp](docs/Models/CteSimpSefazICMS90Simp.md)
 - [CteSimpSefazICMSOutraUFSimp](docs/Models/CteSimpSefazICMSOutraUFSimp.md)
 - [CteSimpSefazICMSSNSimp](docs/Models/CteSimpSefazICMSSNSimp.md)
 - [CteSimpSefazICMSUFFimSimp](docs/Models/CteSimpSefazICMSUFFimSimp.md)
 - [CteSimpSefazIdeSimp](docs/Models/CteSimpSefazIdeSimp.md)
 - [CteSimpSefazImpSimp](docs/Models/CteSimpSefazImpSimp.md)
 - [CteSimpSefazInfCTeSuplSimp](docs/Models/CteSimpSefazInfCTeSuplSimp.md)
 - [CteSimpSefazInfCargaSimp](docs/Models/CteSimpSefazInfCargaSimp.md)
 - [CteSimpSefazInfCteImpSimp](docs/Models/CteSimpSefazInfCte_ImpSimp.md)
 - [CteSimpSefazInfCteSimp](docs/Models/CteSimpSefazInfCteSimp.md)
 - [CteSimpSefazInfCteSubSimp](docs/Models/CteSimpSefazInfCteSubSimp.md)
 - [CteSimpSefazInfDocAntSimp](docs/Models/CteSimpSefazInfDocAntSimp.md)
 - [CteSimpSefazInfDocInfNFeSimp](docs/Models/CteSimpSefazInfDoc_InfNFeSimp.md)
 - [CteSimpSefazInfDocSimp](docs/Models/CteSimpSefazInfDocSimp.md)
 - [CteSimpSefazInfModalSimp](docs/Models/CteSimpSefazInfModalSimp.md)
 - [CteSimpSefazInfNFSimp](docs/Models/CteSimpSefazInfNFSimp.md)
 - [CteSimpSefazInfNFeSimp](docs/Models/CteSimpSefazInfNFeSimp.md)
 - [CteSimpSefazInfNFeTranspParcialSimp](docs/Models/CteSimpSefazInfNFeTranspParcialSimp.md)
 - [CteSimpSefazInfQSimp](docs/Models/CteSimpSefazInfQSimp.md)
 - [CteSimpSefazInfSegSimp](docs/Models/CteSimpSefazInfSegSimp.md)
 - [CteSimpSefazInfSolicNFFSimp](docs/Models/CteSimpSefazInfSolicNFFSimp.md)
 - [CteSimpSefazInfTotAPSimp](docs/Models/CteSimpSefazInfTotAPSimp.md)
 - [CteSimpSefazLacUnidCargaSimp](docs/Models/CteSimpSefazLacUnidCargaSimp.md)
 - [CteSimpSefazLacUnidTranspSimp](docs/Models/CteSimpSefazLacUnidTranspSimp.md)
 - [CteSimpSefazLacreSimp](docs/Models/CteSimpSefazLacreSimp.md)
 - [CteSimpSefazMultimodalSimp](docs/Models/CteSimpSefazMultimodalSimp.md)
 - [CteSimpSefazNatCargaSimp](docs/Models/CteSimpSefazNatCargaSimp.md)
 - [CteSimpSefazObsContSimp](docs/Models/CteSimpSefazObsContSimp.md)
 - [CteSimpSefazObsFiscoSimp](docs/Models/CteSimpSefazObsFiscoSimp.md)
 - [CteSimpSefazOccSimp](docs/Models/CteSimpSefazOccSimp.md)
 - [CteSimpSefazPagamentoRTCSimp](docs/Models/CteSimpSefazPagamentoRTCSimp.md)
 - [CteSimpSefazPassSimp](docs/Models/CteSimpSefazPassSimp.md)
 - [CteSimpSefazPeriSimp](docs/Models/CteSimpSefazPeriSimp.md)
 - [CteSimpSefazPgtoVincSimp](docs/Models/CteSimpSefazPgtoVincSimp.md)
 - [CteSimpSefazRedSimp](docs/Models/CteSimpSefazRedSimp.md)
 - [CteSimpSefazRespTecSimp](docs/Models/CteSimpSefazRespTecSimp.md)
 - [CteSimpSefazRodoSimp](docs/Models/CteSimpSefazRodoSimp.md)
 - [CteSimpSefazSegSimp](docs/Models/CteSimpSefazSegSimp.md)
 - [CteSimpSefazTarifaSimp](docs/Models/CteSimpSefazTarifaSimp.md)
 - [CteSimpSefazTomaSimp](docs/Models/CteSimpSefazTomaSimp.md)
 - [CteSimpSefazTotalSimp](docs/Models/CteSimpSefazTotalSimp.md)
 - [CteSimpSefazTrafMutSimp](docs/Models/CteSimpSefazTrafMutSimp.md)
 - [CteSimpSefazTribCTeSimp](docs/Models/CteSimpSefazTribCTeSimp.md)
 - [CteSimpSefazTribCompraGovSimp](docs/Models/CteSimpSefazTribCompraGovSimp.md)
 - [CteSimpSefazTribRegularSimp](docs/Models/CteSimpSefazTribRegularSimp.md)
 - [CteSimpSefazUnidCargaSimp](docs/Models/CteSimpSefazUnidCargaSimp.md)
 - [CteSimpSefazUnidadeTranspSimp](docs/Models/CteSimpSefazUnidadeTranspSimp.md)
 - [DPS](docs/Models/DPS.md)
 - [DcePedidoCancelamento](docs/Models/DcePedidoCancelamento.md)
 - [DcePedidoEmissao](docs/Models/DcePedidoEmissao.md)
 - [DceSefazAutXML](docs/Models/DceSefazAutXML.md)
 - [DceSefazDest](docs/Models/DceSefazDest.md)
 - [DceSefazDet](docs/Models/DceSefazDet.md)
 - [DceSefazECT](docs/Models/DceSefazECT.md)
 - [DceSefazEmit](docs/Models/DceSefazEmit.md)
 - [DceSefazEndeDest](docs/Models/DceSefazEndeDest.md)
 - [DceSefazEndeEmi](docs/Models/DceSefazEndeEmi.md)
 - [DceSefazFisco](docs/Models/DceSefazFisco.md)
 - [DceSefazIde](docs/Models/DceSefazIde.md)
 - [DceSefazInfAdic](docs/Models/DceSefazInfAdic.md)
 - [DceSefazInfDCe](docs/Models/DceSefazInfDCe.md)
 - [DceSefazInfDec](docs/Models/DceSefazInfDec.md)
 - [DceSefazInfSolicDCe](docs/Models/DceSefazInfSolicDCe.md)
 - [DceSefazMarketplace](docs/Models/DceSefazMarketplace.md)
 - [DceSefazObsECT](docs/Models/DceSefazObsECT.md)
 - [DceSefazObsEmit](docs/Models/DceSefazObsEmit.md)
 - [DceSefazObsFisco](docs/Models/DceSefazObsFisco.md)
 - [DceSefazObsMarketplace](docs/Models/DceSefazObsMarketplace.md)
 - [DceSefazProd](docs/Models/DceSefazProd.md)
 - [DceSefazTotal](docs/Models/DceSefazTotal.md)
 - [DceSefazTransp](docs/Models/DceSefazTransp.md)
 - [DceSefazTransportadora](docs/Models/DceSefazTransportadora.md)
 - [Dfe](docs/Models/Dfe.md)
 - [DfeAutorEvento](docs/Models/DfeAutorEvento.md)
 - [DfeAutorizacao](docs/Models/DfeAutorizacao.md)
 - [DfeCancelamento](docs/Models/DfeCancelamento.md)
 - [DfeCartaCorrecao](docs/Models/DfeCartaCorrecao.md)
 - [DfeContribuinteEndereco](docs/Models/DfeContribuinteEndereco.md)
 - [DfeContribuinteInfCad](docs/Models/DfeContribuinteInfCad.md)
 - [DfeContribuinteInfCons](docs/Models/DfeContribuinteInfCons.md)
 - [DfeDebug](docs/Models/DfeDebug.md)
 - [DfeEvento](docs/Models/DfeEvento.md)
 - [DfeEventoListagem](docs/Models/DfeEventoListagem.md)
 - [DfeInutilizacao](docs/Models/DfeInutilizacao.md)
 - [DfeListagem](docs/Models/DfeListagem.md)
 - [DfeLote](docs/Models/DfeLote.md)
 - [DfeLoteListagem](docs/Models/DfeLoteListagem.md)
 - [DfePedidoEnvioEmail](docs/Models/DfePedidoEnvioEmail.md)
 - [DfePedidoInutilizacao](docs/Models/DfePedidoInutilizacao.md)
 - [DfeRecibo](docs/Models/DfeRecibo.md)
 - [DfeRequisicaoDebug](docs/Models/DfeRequisicaoDebug.md)
 - [DfeSefazStatus](docs/Models/DfeSefazStatus.md)
 - [DfeSincronizacao](docs/Models/DfeSincronizacao.md)
 - [DistribuicaoNfe](docs/Models/DistribuicaoNfe.md)
 - [DistribuicaoNfeDocumento](docs/Models/DistribuicaoNfeDocumento.md)
 - [DistribuicaoNfeDocumentoListagem](docs/Models/DistribuicaoNfeDocumentoListagem.md)
 - [DistribuicaoNfeEvento](docs/Models/DistribuicaoNfeEvento.md)
 - [DistribuicaoNfeListagem](docs/Models/DistribuicaoNfeListagem.md)
 - [DistribuicaoNfeNota](docs/Models/DistribuicaoNfeNota.md)
 - [DistribuicaoNfeNotaListagem](docs/Models/DistribuicaoNfeNotaListagem.md)
 - [DistribuicaoNfePedido](docs/Models/DistribuicaoNfePedido.md)
 - [DistribuicaoNfePedidoManifestacao](docs/Models/DistribuicaoNfePedidoManifestacao.md)
 - [DocDedRed](docs/Models/DocDedRed.md)
 - [DocNFNFS](docs/Models/DocNFNFS.md)
 - [DocOutNFSe](docs/Models/DocOutNFSe.md)
 - [Email](docs/Models/Email.md)
 - [EmailAttachment](docs/Models/EmailAttachment.md)
 - [EmailEvent](docs/Models/EmailEvent.md)
 - [EmailListagem](docs/Models/EmailListagem.md)
 - [EmailResumo](docs/Models/EmailResumo.md)
 - [EmailStatusResponse](docs/Models/EmailStatusResponse.md)
 - [Empresa](docs/Models/Empresa.md)
 - [EmpresaCertificado](docs/Models/EmpresaCertificado.md)
 - [EmpresaCertificadoListagem](docs/Models/EmpresaCertificadoListagem.md)
 - [EmpresaConfigCte](docs/Models/EmpresaConfigCte.md)
 - [EmpresaConfigCteOs](docs/Models/EmpresaConfigCteOs.md)
 - [EmpresaConfigDce](docs/Models/EmpresaConfigDce.md)
 - [EmpresaConfigDistribuicaoNfe](docs/Models/EmpresaConfigDistribuicaoNfe.md)
 - [EmpresaConfigMdfe](docs/Models/EmpresaConfigMdfe.md)
 - [EmpresaConfigNfce](docs/Models/EmpresaConfigNfce.md)
 - [EmpresaConfigNfceSefaz](docs/Models/EmpresaConfigNfceSefaz.md)
 - [EmpresaConfigNfcom](docs/Models/EmpresaConfigNfcom.md)
 - [EmpresaConfigNfe](docs/Models/EmpresaConfigNfe.md)
 - [EmpresaConfigNfse](docs/Models/EmpresaConfigNfse.md)
 - [EmpresaConfigNfseRegTrib](docs/Models/EmpresaConfigNfseRegTrib.md)
 - [EmpresaConfigPrefeitura](docs/Models/EmpresaConfigPrefeitura.md)
 - [EmpresaConfigRps](docs/Models/EmpresaConfigRps.md)
 - [EmpresaEndereco](docs/Models/EmpresaEndereco.md)
 - [EmpresaListagem](docs/Models/EmpresaListagem.md)
 - [EmpresaPedidoCadastroCertificado](docs/Models/EmpresaPedidoCadastroCertificado.md)
 - [EnderExt](docs/Models/EnderExt.md)
 - [EnderExtSimples](docs/Models/EnderExtSimples.md)
 - [EnderNac](docs/Models/EnderNac.md)
 - [EnderObraEvento](docs/Models/EnderObraEvento.md)
 - [Endereco](docs/Models/Endereco.md)
 - [EnderecoEmail](docs/Models/EnderecoEmail.md)
 - [EnderecoSimples](docs/Models/EnderecoSimples.md)
 - [ExigSuspensa](docs/Models/ExigSuspensa.md)
 - [HttpRequestDebug](docs/Models/HttpRequestDebug.md)
 - [InfDPS](docs/Models/InfDPS.md)
 - [InfoCompl](docs/Models/InfoCompl.md)
 - [InfoDedRed](docs/Models/InfoDedRed.md)
 - [InfoFornecDocDedRed](docs/Models/InfoFornecDocDedRed.md)
 - [InfoIntermediario](docs/Models/InfoIntermediario.md)
 - [InfoItemPed](docs/Models/InfoItemPed.md)
 - [InfoObra](docs/Models/InfoObra.md)
 - [InfoPrestador](docs/Models/InfoPrestador.md)
 - [InfoRefNFSe](docs/Models/InfoRefNFSe.md)
 - [InfoTomador](docs/Models/InfoTomador.md)
 - [InfoTributacao](docs/Models/InfoTributacao.md)
 - [InfoValores](docs/Models/InfoValores.md)
 - [ListaDocDedRed](docs/Models/ListaDocDedRed.md)
 - [LocPrest](docs/Models/LocPrest.md)
 - [ManifestacaoNfeListagem](docs/Models/ManifestacaoNfeListagem.md)
 - [MdfeDocumentoVinculado](docs/Models/MdfeDocumentoVinculado.md)
 - [MdfeEncerramento](docs/Models/MdfeEncerramento.md)
 - [MdfeInclusaoCondutor](docs/Models/MdfeInclusaoCondutor.md)
 - [MdfeInclusaoDfe](docs/Models/MdfeInclusaoDfe.md)
 - [MdfeNaoEncerrado](docs/Models/MdfeNaoEncerrado.md)
 - [MdfeNaoEncerrados](docs/Models/MdfeNaoEncerrados.md)
 - [MdfePedidoCancelamento](docs/Models/MdfePedidoCancelamento.md)
 - [MdfePedidoEmissao](docs/Models/MdfePedidoEmissao.md)
 - [MdfePedidoEmissaoLote](docs/Models/MdfePedidoEmissaoLote.md)
 - [MdfePedidoEncerramento](docs/Models/MdfePedidoEncerramento.md)
 - [MdfePedidoInclusaoCondutor](docs/Models/MdfePedidoInclusaoCondutor.md)
 - [MdfePedidoInclusaoDfe](docs/Models/MdfePedidoInclusaoDfe.md)
 - [MdfeSefazAereo](docs/Models/MdfeSefazAereo.md)
 - [MdfeSefazAquav](docs/Models/MdfeSefazAquav.md)
 - [MdfeSefazAutXML](docs/Models/MdfeSefazAutXML.md)
 - [MdfeSefazComp](docs/Models/MdfeSefazComp.md)
 - [MdfeSefazCondutor](docs/Models/MdfeSefazCondutor.md)
 - [MdfeSefazDisp](docs/Models/MdfeSefazDisp.md)
 - [MdfeSefazEmit](docs/Models/MdfeSefazEmit.md)
 - [MdfeSefazEndeEmi](docs/Models/MdfeSefazEndeEmi.md)
 - [MdfeSefazFerrov](docs/Models/MdfeSefazFerrov.md)
 - [MdfeSefazIde](docs/Models/MdfeSefazIde.md)
 - [MdfeSefazInfANTT](docs/Models/MdfeSefazInfANTT.md)
 - [MdfeSefazInfAdic](docs/Models/MdfeSefazInfAdic.md)
 - [MdfeSefazInfBanc](docs/Models/MdfeSefazInfBanc.md)
 - [MdfeSefazInfCIOT](docs/Models/MdfeSefazInfCIOT.md)
 - [MdfeSefazInfCTe](docs/Models/MdfeSefazInfCTe.md)
 - [MdfeSefazInfContratante](docs/Models/MdfeSefazInfContratante.md)
 - [MdfeSefazInfContrato](docs/Models/MdfeSefazInfContrato.md)
 - [MdfeSefazInfDoc](docs/Models/MdfeSefazInfDoc.md)
 - [MdfeSefazInfEmbComb](docs/Models/MdfeSefazInfEmbComb.md)
 - [MdfeSefazInfEntregaParcial](docs/Models/MdfeSefazInfEntregaParcial.md)
 - [MdfeSefazInfLocalCarrega](docs/Models/MdfeSefazInfLocalCarrega.md)
 - [MdfeSefazInfLocalDescarrega](docs/Models/MdfeSefazInfLocalDescarrega.md)
 - [MdfeSefazInfLotacao](docs/Models/MdfeSefazInfLotacao.md)
 - [MdfeSefazInfMDFe](docs/Models/MdfeSefazInfMDFe.md)
 - [MdfeSefazInfMDFeSupl](docs/Models/MdfeSefazInfMDFeSupl.md)
 - [MdfeSefazInfMDFeTransp](docs/Models/MdfeSefazInfMDFeTransp.md)
 - [MdfeSefazInfMDFeTranspPeri](docs/Models/MdfeSefazInfMDFeTransp_Peri.md)
 - [MdfeSefazInfModal](docs/Models/MdfeSefazInfModal.md)
 - [MdfeSefazInfMunCarrega](docs/Models/MdfeSefazInfMunCarrega.md)
 - [MdfeSefazInfMunDescarga](docs/Models/MdfeSefazInfMunDescarga.md)
 - [MdfeSefazInfNFe](docs/Models/MdfeSefazInfNFe.md)
 - [MdfeSefazInfNFePeri](docs/Models/MdfeSefazInfNFe_Peri.md)
 - [MdfeSefazInfNFePrestParcial](docs/Models/MdfeSefazInfNFePrestParcial.md)
 - [MdfeSefazInfPag](docs/Models/MdfeSefazInfPag.md)
 - [MdfeSefazInfPercurso](docs/Models/MdfeSefazInfPercurso.md)
 - [MdfeSefazInfPrazo](docs/Models/MdfeSefazInfPrazo.md)
 - [MdfeSefazInfResp](docs/Models/MdfeSefazInfResp.md)
 - [MdfeSefazInfSeg](docs/Models/MdfeSefazInfSeg.md)
 - [MdfeSefazInfSolicNFF](docs/Models/MdfeSefazInfSolicNFF.md)
 - [MdfeSefazInfTermCarreg](docs/Models/MdfeSefazInfTermCarreg.md)
 - [MdfeSefazInfTermDescarreg](docs/Models/MdfeSefazInfTermDescarreg.md)
 - [MdfeSefazInfUnidCargaVazia](docs/Models/MdfeSefazInfUnidCargaVazia.md)
 - [MdfeSefazInfUnidTranspVazia](docs/Models/MdfeSefazInfUnidTranspVazia.md)
 - [MdfeSefazLacRodo](docs/Models/MdfeSefazLacRodo.md)
 - [MdfeSefazLacUnidCarga](docs/Models/MdfeSefazLacUnidCarga.md)
 - [MdfeSefazLacUnidTransp](docs/Models/MdfeSefazLacUnidTransp.md)
 - [MdfeSefazLacres](docs/Models/MdfeSefazLacres.md)
 - [MdfeSefazPeri](docs/Models/MdfeSefazPeri.md)
 - [MdfeSefazProdPred](docs/Models/MdfeSefazProdPred.md)
 - [MdfeSefazProp](docs/Models/MdfeSefazProp.md)
 - [MdfeSefazRespTec](docs/Models/MdfeSefazRespTec.md)
 - [MdfeSefazRodo](docs/Models/MdfeSefazRodo.md)
 - [MdfeSefazSeg](docs/Models/MdfeSefazSeg.md)
 - [MdfeSefazTot](docs/Models/MdfeSefazTot.md)
 - [MdfeSefazTrem](docs/Models/MdfeSefazTrem.md)
 - [MdfeSefazUnidCarga](docs/Models/MdfeSefazUnidCarga.md)
 - [MdfeSefazUnidadeTransp](docs/Models/MdfeSefazUnidadeTransp.md)
 - [MdfeSefazVag](docs/Models/MdfeSefazVag.md)
 - [MdfeSefazValePed](docs/Models/MdfeSefazValePed.md)
 - [MdfeSefazVeicReboque](docs/Models/MdfeSefazVeicReboque.md)
 - [MdfeSefazVeicReboqueProp](docs/Models/MdfeSefazVeicReboque_Prop.md)
 - [MdfeSefazVeicTracao](docs/Models/MdfeSefazVeicTracao.md)
 - [NfcomPedidoCancelamento](docs/Models/NfcomPedidoCancelamento.md)
 - [NfcomPedidoEmissao](docs/Models/NfcomPedidoEmissao.md)
 - [NfcomSefazALCZFMCBS](docs/Models/NfcomSefazALCZFMCBS.md)
 - [NfcomSefazAssinante](docs/Models/NfcomSefazAssinante.md)
 - [NfcomSefazAutXML](docs/Models/NfcomSefazAutXML.md)
 - [NfcomSefazCIBS](docs/Models/NfcomSefazCIBS.md)
 - [NfcomSefazCOFINS](docs/Models/NfcomSefazCOFINS.md)
 - [NfcomSefazCompraGovReduzido](docs/Models/NfcomSefazCompraGovReduzido.md)
 - [NfcomSefazDest](docs/Models/NfcomSefazDest.md)
 - [NfcomSefazDet](docs/Models/NfcomSefazDet.md)
 - [NfcomSefazDevTrib](docs/Models/NfcomSefazDevTrib.md)
 - [NfcomSefazDif](docs/Models/NfcomSefazDif.md)
 - [NfcomSefazEmit](docs/Models/NfcomSefazEmit.md)
 - [NfcomSefazEndeDest](docs/Models/NfcomSefazEndeDest.md)
 - [NfcomSefazEndeEmi](docs/Models/NfcomSefazEndeEmi.md)
 - [NfcomSefazEstornoCred](docs/Models/NfcomSefazEstornoCred.md)
 - [NfcomSefazFUNTTEL](docs/Models/NfcomSefazFUNTTEL.md)
 - [NfcomSefazFUST](docs/Models/NfcomSefazFUST.md)
 - [NfcomSefazGCBS](docs/Models/NfcomSefazGCBS.md)
 - [NfcomSefazGCofat](docs/Models/NfcomSefazGCofat.md)
 - [NfcomSefazGCofatGNF](docs/Models/NfcomSefazGCofat_GNF.md)
 - [NfcomSefazGEstornoCred](docs/Models/NfcomSefazGEstornoCred.md)
 - [NfcomSefazGFat](docs/Models/NfcomSefazGFat.md)
 - [NfcomSefazGFatCentral](docs/Models/NfcomSefazGFatCentral.md)
 - [NfcomSefazGFidelidade](docs/Models/NfcomSefazGFidelidade.md)
 - [NfcomSefazGIBS](docs/Models/NfcomSefazGIBS.md)
 - [NfcomSefazGIBSGIBSMun](docs/Models/NfcomSefazGIBS_GIBSMun.md)
 - [NfcomSefazGIBSGIBSUF](docs/Models/NfcomSefazGIBS_GIBSUF.md)
 - [NfcomSefazGIBSMun](docs/Models/NfcomSefazGIBSMun.md)
 - [NfcomSefazGIBSUF](docs/Models/NfcomSefazGIBSUF.md)
 - [NfcomSefazGNF](docs/Models/NfcomSefazGNF.md)
 - [NfcomSefazGPIX](docs/Models/NfcomSefazGPIX.md)
 - [NfcomSefazGPagAntecipado](docs/Models/NfcomSefazGPagAntecipado.md)
 - [NfcomSefazGProc](docs/Models/NfcomSefazGProc.md)
 - [NfcomSefazGProcRef](docs/Models/NfcomSefazGProcRef.md)
 - [NfcomSefazGRessarc](docs/Models/NfcomSefazGRessarc.md)
 - [NfcomSefazGSub](docs/Models/NfcomSefazGSub.md)
 - [NfcomSefazIBSCBSTot](docs/Models/NfcomSefazIBSCBSTot.md)
 - [NfcomSefazIBSCBSTotGCBS](docs/Models/NfcomSefazIBSCBSTot_GCBS.md)
 - [NfcomSefazICMS00](docs/Models/NfcomSefazICMS00.md)
 - [NfcomSefazICMS20](docs/Models/NfcomSefazICMS20.md)
 - [NfcomSefazICMS40](docs/Models/NfcomSefazICMS40.md)
 - [NfcomSefazICMS51](docs/Models/NfcomSefazICMS51.md)
 - [NfcomSefazICMS90](docs/Models/NfcomSefazICMS90.md)
 - [NfcomSefazICMSSN](docs/Models/NfcomSefazICMSSN.md)
 - [NfcomSefazICMSTot](docs/Models/NfcomSefazICMSTot.md)
 - [NfcomSefazICMSUFDest](docs/Models/NfcomSefazICMSUFDest.md)
 - [NfcomSefazIde](docs/Models/NfcomSefazIde.md)
 - [NfcomSefazImposto](docs/Models/NfcomSefazImposto.md)
 - [NfcomSefazInfAdic](docs/Models/NfcomSefazInfAdic.md)
 - [NfcomSefazInfNFCom](docs/Models/NfcomSefazInfNFCom.md)
 - [NfcomSefazPIS](docs/Models/NfcomSefazPIS.md)
 - [NfcomSefazPagamentoRTC](docs/Models/NfcomSefazPagamentoRTC.md)
 - [NfcomSefazPgtoVinc](docs/Models/NfcomSefazPgtoVinc.md)
 - [NfcomSefazProd](docs/Models/NfcomSefazProd.md)
 - [NfcomSefazRed](docs/Models/NfcomSefazRed.md)
 - [NfcomSefazRespTec](docs/Models/NfcomSefazRespTec.md)
 - [NfcomSefazRetTrib](docs/Models/NfcomSefazRetTrib.md)
 - [NfcomSefazTotal](docs/Models/NfcomSefazTotal.md)
 - [NfcomSefazTribCompraGov](docs/Models/NfcomSefazTribCompraGov.md)
 - [NfcomSefazTribNFCom](docs/Models/NfcomSefazTribNFCom.md)
 - [NfcomSefazTribRegular](docs/Models/NfcomSefazTribRegular.md)
 - [NfcomSefazVRetTribTot](docs/Models/NfcomSefazVRetTribTot.md)
 - [NfePedidoCancelamento](docs/Models/NfePedidoCancelamento.md)
 - [NfePedidoCartaCorrecao](docs/Models/NfePedidoCartaCorrecao.md)
 - [NfePedidoEmissao](docs/Models/NfePedidoEmissao.md)
 - [NfePedidoEmissaoLote](docs/Models/NfePedidoEmissaoLote.md)
 - [NfeSefazAdi](docs/Models/NfeSefazAdi.md)
 - [NfeSefazAgropecuario](docs/Models/NfeSefazAgropecuario.md)
 - [NfeSefazAjusteCompet](docs/Models/NfeSefazAjusteCompet.md)
 - [NfeSefazArma](docs/Models/NfeSefazArma.md)
 - [NfeSefazAutXML](docs/Models/NfeSefazAutXML.md)
 - [NfeSefazAvulsa](docs/Models/NfeSefazAvulsa.md)
 - [NfeSefazCIBS](docs/Models/NfeSefazCIBS.md)
 - [NfeSefazCIDE](docs/Models/NfeSefazCIDE.md)
 - [NfeSefazCOFINS](docs/Models/NfeSefazCOFINS.md)
 - [NfeSefazCOFINSAliq](docs/Models/NfeSefazCOFINSAliq.md)
 - [NfeSefazCOFINSNT](docs/Models/NfeSefazCOFINSNT.md)
 - [NfeSefazCOFINSOutr](docs/Models/NfeSefazCOFINSOutr.md)
 - [NfeSefazCOFINSQtde](docs/Models/NfeSefazCOFINSQtde.md)
 - [NfeSefazCOFINSST](docs/Models/NfeSefazCOFINSST.md)
 - [NfeSefazCana](docs/Models/NfeSefazCana.md)
 - [NfeSefazCard](docs/Models/NfeSefazCard.md)
 - [NfeSefazCobr](docs/Models/NfeSefazCobr.md)
 - [NfeSefazComb](docs/Models/NfeSefazComb.md)
 - [NfeSefazCompra](docs/Models/NfeSefazCompra.md)
 - [NfeSefazCompraGov](docs/Models/NfeSefazCompraGov.md)
 - [NfeSefazCredPres](docs/Models/NfeSefazCredPres.md)
 - [NfeSefazCredPresIBSZFM](docs/Models/NfeSefazCredPresIBSZFM.md)
 - [NfeSefazCredPresOper](docs/Models/NfeSefazCredPresOper.md)
 - [NfeSefazDFeReferenciado](docs/Models/NfeSefazDFeReferenciado.md)
 - [NfeSefazDI](docs/Models/NfeSefazDI.md)
 - [NfeSefazDeduc](docs/Models/NfeSefazDeduc.md)
 - [NfeSefazDefensivo](docs/Models/NfeSefazDefensivo.md)
 - [NfeSefazDest](docs/Models/NfeSefazDest.md)
 - [NfeSefazDet](docs/Models/NfeSefazDet.md)
 - [NfeSefazDetExport](docs/Models/NfeSefazDetExport.md)
 - [NfeSefazDetPag](docs/Models/NfeSefazDetPag.md)
 - [NfeSefazDevTrib](docs/Models/NfeSefazDevTrib.md)
 - [NfeSefazDif](docs/Models/NfeSefazDif.md)
 - [NfeSefazDup](docs/Models/NfeSefazDup.md)
 - [NfeSefazEmit](docs/Models/NfeSefazEmit.md)
 - [NfeSefazEncerrante](docs/Models/NfeSefazEncerrante.md)
 - [NfeSefazEnderEmi](docs/Models/NfeSefazEnderEmi.md)
 - [NfeSefazEndereco](docs/Models/NfeSefazEndereco.md)
 - [NfeSefazEstornoCred](docs/Models/NfeSefazEstornoCred.md)
 - [NfeSefazExportInd](docs/Models/NfeSefazExportInd.md)
 - [NfeSefazExporta](docs/Models/NfeSefazExporta.md)
 - [NfeSefazFat](docs/Models/NfeSefazFat.md)
 - [NfeSefazForDia](docs/Models/NfeSefazForDia.md)
 - [NfeSefazGCBS](docs/Models/NfeSefazGCBS.md)
 - [NfeSefazGCred](docs/Models/NfeSefazGCred.md)
 - [NfeSefazGEstornoCred](docs/Models/NfeSefazGEstornoCred.md)
 - [NfeSefazGIBS](docs/Models/NfeSefazGIBS.md)
 - [NfeSefazGIBSGIBSMun](docs/Models/NfeSefazGIBS_GIBSMun.md)
 - [NfeSefazGIBSGIBSUF](docs/Models/NfeSefazGIBS_GIBSUF.md)
 - [NfeSefazGIBSMun](docs/Models/NfeSefazGIBSMun.md)
 - [NfeSefazGIBSUF](docs/Models/NfeSefazGIBSUF.md)
 - [NfeSefazGMono](docs/Models/NfeSefazGMono.md)
 - [NfeSefazGMonoDif](docs/Models/NfeSefazGMonoDif.md)
 - [NfeSefazGMonoPadrao](docs/Models/NfeSefazGMonoPadrao.md)
 - [NfeSefazGMonoRet](docs/Models/NfeSefazGMonoRet.md)
 - [NfeSefazGMonoReten](docs/Models/NfeSefazGMonoReten.md)
 - [NfeSefazGPagAntecipado](docs/Models/NfeSefazGPagAntecipado.md)
 - [NfeSefazGuiaTransito](docs/Models/NfeSefazGuiaTransito.md)
 - [NfeSefazIBSCBSMonoTot](docs/Models/NfeSefazIBSCBSMonoTot.md)
 - [NfeSefazIBSCBSMonoTotGCBS](docs/Models/NfeSefazIBSCBSMonoTot_GCBS.md)
 - [NfeSefazICMS](docs/Models/NfeSefazICMS.md)
 - [NfeSefazICMS00](docs/Models/NfeSefazICMS00.md)
 - [NfeSefazICMS02](docs/Models/NfeSefazICMS02.md)
 - [NfeSefazICMS10](docs/Models/NfeSefazICMS10.md)
 - [NfeSefazICMS15](docs/Models/NfeSefazICMS15.md)
 - [NfeSefazICMS20](docs/Models/NfeSefazICMS20.md)
 - [NfeSefazICMS30](docs/Models/NfeSefazICMS30.md)
 - [NfeSefazICMS40](docs/Models/NfeSefazICMS40.md)
 - [NfeSefazICMS51](docs/Models/NfeSefazICMS51.md)
 - [NfeSefazICMS53](docs/Models/NfeSefazICMS53.md)
 - [NfeSefazICMS60](docs/Models/NfeSefazICMS60.md)
 - [NfeSefazICMS61](docs/Models/NfeSefazICMS61.md)
 - [NfeSefazICMS70](docs/Models/NfeSefazICMS70.md)
 - [NfeSefazICMS90](docs/Models/NfeSefazICMS90.md)
 - [NfeSefazICMSPart](docs/Models/NfeSefazICMSPart.md)
 - [NfeSefazICMSSN101](docs/Models/NfeSefazICMSSN101.md)
 - [NfeSefazICMSSN102](docs/Models/NfeSefazICMSSN102.md)
 - [NfeSefazICMSSN201](docs/Models/NfeSefazICMSSN201.md)
 - [NfeSefazICMSSN202](docs/Models/NfeSefazICMSSN202.md)
 - [NfeSefazICMSSN500](docs/Models/NfeSefazICMSSN500.md)
 - [NfeSefazICMSSN900](docs/Models/NfeSefazICMSSN900.md)
 - [NfeSefazICMSST](docs/Models/NfeSefazICMSST.md)
 - [NfeSefazICMSTot](docs/Models/NfeSefazICMSTot.md)
 - [NfeSefazICMSUFDest](docs/Models/NfeSefazICMSUFDest.md)
 - [NfeSefazII](docs/Models/NfeSefazII.md)
 - [NfeSefazIPINT](docs/Models/NfeSefazIPINT.md)
 - [NfeSefazIPITrib](docs/Models/NfeSefazIPITrib.md)
 - [NfeSefazIS](docs/Models/NfeSefazIS.md)
 - [NfeSefazISSQN](docs/Models/NfeSefazISSQN.md)
 - [NfeSefazISSQNtot](docs/Models/NfeSefazISSQNtot.md)
 - [NfeSefazISTot](docs/Models/NfeSefazISTot.md)
 - [NfeSefazIde](docs/Models/NfeSefazIde.md)
 - [NfeSefazImposto](docs/Models/NfeSefazImposto.md)
 - [NfeSefazImpostoDevol](docs/Models/NfeSefazImpostoDevol.md)
 - [NfeSefazImpostoDevolIPI](docs/Models/NfeSefazImpostoDevol_IPI.md)
 - [NfeSefazInfAdic](docs/Models/NfeSefazInfAdic.md)
 - [NfeSefazInfAdicObsCont](docs/Models/NfeSefazInfAdic_ObsCont.md)
 - [NfeSefazInfAdicObsFisco](docs/Models/NfeSefazInfAdic_ObsFisco.md)
 - [NfeSefazInfIntermed](docs/Models/NfeSefazInfIntermed.md)
 - [NfeSefazInfNFe](docs/Models/NfeSefazInfNFe.md)
 - [NfeSefazInfNFeSupl](docs/Models/NfeSefazInfNFeSupl.md)
 - [NfeSefazInfPAA](docs/Models/NfeSefazInfPAA.md)
 - [NfeSefazInfProdEmb](docs/Models/NfeSefazInfProdEmb.md)
 - [NfeSefazInfProdNFF](docs/Models/NfeSefazInfProdNFF.md)
 - [NfeSefazInfRespTec](docs/Models/NfeSefazInfRespTec.md)
 - [NfeSefazInfSolicNFF](docs/Models/NfeSefazInfSolicNFF.md)
 - [NfeSefazIpi](docs/Models/NfeSefazIpi.md)
 - [NfeSefazLacres](docs/Models/NfeSefazLacres.md)
 - [NfeSefazLocal](docs/Models/NfeSefazLocal.md)
 - [NfeSefazMed](docs/Models/NfeSefazMed.md)
 - [NfeSefazMonofasia](docs/Models/NfeSefazMonofasia.md)
 - [NfeSefazNFref](docs/Models/NfeSefazNFref.md)
 - [NfeSefazObsCont](docs/Models/NfeSefazObsCont.md)
 - [NfeSefazObsFisco](docs/Models/NfeSefazObsFisco.md)
 - [NfeSefazObsItem](docs/Models/NfeSefazObsItem.md)
 - [NfeSefazOrigComb](docs/Models/NfeSefazOrigComb.md)
 - [NfeSefazPAASignature](docs/Models/NfeSefazPAASignature.md)
 - [NfeSefazPIS](docs/Models/NfeSefazPIS.md)
 - [NfeSefazPISAliq](docs/Models/NfeSefazPISAliq.md)
 - [NfeSefazPISNT](docs/Models/NfeSefazPISNT.md)
 - [NfeSefazPISOutr](docs/Models/NfeSefazPISOutr.md)
 - [NfeSefazPISQtde](docs/Models/NfeSefazPISQtde.md)
 - [NfeSefazPISST](docs/Models/NfeSefazPISST.md)
 - [NfeSefazPag](docs/Models/NfeSefazPag.md)
 - [NfeSefazProcRef](docs/Models/NfeSefazProcRef.md)
 - [NfeSefazProd](docs/Models/NfeSefazProd.md)
 - [NfeSefazRSAKeyValueType](docs/Models/NfeSefazRSAKeyValueType.md)
 - [NfeSefazRastro](docs/Models/NfeSefazRastro.md)
 - [NfeSefazRed](docs/Models/NfeSefazRed.md)
 - [NfeSefazRefECF](docs/Models/NfeSefazRefECF.md)
 - [NfeSefazRefNF](docs/Models/NfeSefazRefNF.md)
 - [NfeSefazRefNFP](docs/Models/NfeSefazRefNFP.md)
 - [NfeSefazRetTransp](docs/Models/NfeSefazRetTransp.md)
 - [NfeSefazRetTrib](docs/Models/NfeSefazRetTrib.md)
 - [NfeSefazTotal](docs/Models/NfeSefazTotal.md)
 - [NfeSefazTransfCred](docs/Models/NfeSefazTransfCred.md)
 - [NfeSefazTransp](docs/Models/NfeSefazTransp.md)
 - [NfeSefazTransporta](docs/Models/NfeSefazTransporta.md)
 - [NfeSefazTribCompraGov](docs/Models/NfeSefazTribCompraGov.md)
 - [NfeSefazTribNFe](docs/Models/NfeSefazTribNFe.md)
 - [NfeSefazTribRegular](docs/Models/NfeSefazTribRegular.md)
 - [NfeSefazVeicProd](docs/Models/NfeSefazVeicProd.md)
 - [NfeSefazVeiculo](docs/Models/NfeSefazVeiculo.md)
 - [NfeSefazVol](docs/Models/NfeSefazVol.md)
 - [Nfse](docs/Models/Nfse.md)
 - [NfseCancelamento](docs/Models/NfseCancelamento.md)
 - [NfseCidadeMetadados](docs/Models/NfseCidadeMetadados.md)
 - [NfseCidadesAtendidas](docs/Models/NfseCidadesAtendidas.md)
 - [NfseDpsPedidoEmissao](docs/Models/NfseDpsPedidoEmissao.md)
 - [NfseListagem](docs/Models/NfseListagem.md)
 - [NfseLoteDpsPedidoEmissao](docs/Models/NfseLoteDpsPedidoEmissao.md)
 - [NfseMensagemRetorno](docs/Models/NfseMensagemRetorno.md)
 - [NfsePedidoCancelamento](docs/Models/NfsePedidoCancelamento.md)
 - [NfsePedidoEmissao](docs/Models/NfsePedidoEmissao.md)
 - [NfsePedidoSincronizacao](docs/Models/NfsePedidoSincronizacao.md)
 - [NfseSincronizacao](docs/Models/NfseSincronizacao.md)
 - [RTCInfoDest](docs/Models/RTCInfoDest.md)
 - [RTCInfoIBSCBS](docs/Models/RTCInfoIBSCBS.md)
 - [RTCInfoImovel](docs/Models/RTCInfoImovel.md)
 - [RTCInfoReeRepRes](docs/Models/RTCInfoReeRepRes.md)
 - [RTCInfoTributosDif](docs/Models/RTCInfoTributosDif.md)
 - [RTCInfoTributosIBSCBS](docs/Models/RTCInfoTributosIBSCBS.md)
 - [RTCInfoTributosSitClas](docs/Models/RTCInfoTributosSitClas.md)
 - [RTCInfoTributosTribRegular](docs/Models/RTCInfoTributosTribRegular.md)
 - [RTCInfoValoresIBSCBS](docs/Models/RTCInfoValoresIBSCBS.md)
 - [RTCListaDoc](docs/Models/RTCListaDoc.md)
 - [RTCListaDocDFe](docs/Models/RTCListaDocDFe.md)
 - [RTCListaDocFiscalOutro](docs/Models/RTCListaDocFiscalOutro.md)
 - [RTCListaDocFornec](docs/Models/RTCListaDocFornec.md)
 - [RTCListaDocOutro](docs/Models/RTCListaDocOutro.md)
 - [RegTrib](docs/Models/RegTrib.md)
 - [Rps](docs/Models/Rps.md)
 - [RpsDados](docs/Models/RpsDados.md)
 - [RpsDadosConstrucaoCivil](docs/Models/RpsDadosConstrucaoCivil.md)
 - [RpsDadosIntermediario](docs/Models/RpsDadosIntermediario.md)
 - [RpsDadosPrestador](docs/Models/RpsDadosPrestador.md)
 - [RpsDadosServico](docs/Models/RpsDadosServico.md)
 - [RpsDadosTomador](docs/Models/RpsDadosTomador.md)
 - [RpsDadosTomadorEndereco](docs/Models/RpsDadosTomadorEndereco.md)
 - [RpsIdentificacao](docs/Models/RpsIdentificacao.md)
 - [RpsIdentificacaoPrestador](docs/Models/RpsIdentificacaoPrestador.md)
 - [RpsLote](docs/Models/RpsLote.md)
 - [RpsLoteListagem](docs/Models/RpsLoteListagem.md)
 - [RpsPedidoEmissao](docs/Models/RpsPedidoEmissao.md)
 - [RpsPedidoEmissaoLote](docs/Models/RpsPedidoEmissaoLote.md)
 - [RpsServicoValores](docs/Models/RpsServicoValores.md)
 - [Serv](docs/Models/Serv.md)
 - [Substituicao](docs/Models/Substituicao.md)
 - [TribFederal](docs/Models/TribFederal.md)
 - [TribMunicipal](docs/Models/TribMunicipal.md)
 - [TribOutrosPisCofins](docs/Models/TribOutrosPisCofins.md)
 - [TribTotal](docs/Models/TribTotal.md)
 - [TribTotalMonet](docs/Models/TribTotalMonet.md)
 - [TribTotalPercent](docs/Models/TribTotalPercent.md)
 - [VDescCondIncond](docs/Models/VDescCondIncond.md)
 - [VServPrest](docs/Models/VServPrest.md)


<a name="documentation-for-authorization"></a>
## Autorização

- **oauth2**: OAuth 2.0, fluxo `application`
  - URL do token: https://auth.acbr.api.br/realms/ACBrAPI/protocol/openid-connect/token
  - Escopo: `conta`
  - Escopo: `empresa`
  - Escopo: `cep`
  - Escopo: `cnpj`
  - Escopo: `mdfe`
  - Escopo: `cte`
  - Escopo: `nfse`
  - Escopo: `nfe`

