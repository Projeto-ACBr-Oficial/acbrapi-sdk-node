# Documentação da ACBr API

Referência dos endpoints e DTOs do SDK Node.js da ACBr API.
Consultar também a [documentação oficial da ACBr API](https://dev.acbr.api.br/docs)
e o [README do SDK](../README.md).

<a name="documentation-for-api-endpoints"></a>
## Documentação dos endpoints

Todas as URIs relativas a *https://prod.acbr.api.br*

| Classe | Método | Endpoint | Descrição |
|------------ | ------------- | ------------- | -------------|
| *CepApi* | [**consultarCep**](Apis/CepApi.md#consultarcep) | **GET** /cep/{Cep} | Consultar endereço através do CEP |
| *CnpjApi* | [**consultarCnpj**](Apis/CnpjApi.md#consultarcnpj) | **GET** /cnpj/{Cnpj} | Consultar dados do CNPJ |
*CnpjApi* | [**listarCnpj**](Apis/CnpjApi.md#listarcnpj) | **GET** /cnpj | Listar estabelecimentos ativos a partir da base de CNPJ |
| *ContaApi* | [**consultarCotaConta**](Apis/ContaApi.md#consultarcotaconta) | **GET** /conta/cotas/{nome} | Consultar o limite de uso e o consumo de uma cota específica. |
*ContaApi* | [**consultarCotaPrePago**](Apis/ContaApi.md#consultarcotaprepago) | **GET** /conta/cotas/prepago | Consultar o resumo da cota de créditos pré-pagos. |
*ContaApi* | [**listarCotasConta**](Apis/ContaApi.md#listarcotasconta) | **GET** /conta/cotas | Consultar os limites de uso e consumo das cotas disponíveis, exceto a cota de créditos pré-pagos. |
*ContaApi* | [**listarExtratoCreditosConta**](Apis/ContaApi.md#listarextratocreditosconta) | **GET** /conta/extrato | Consultar o extrato de movimentação de créditos do tenant atual. |
| *CteApi* | [**baixarPdfCancelamentoCte**](Apis/CteApi.md#baixarpdfcancelamentocte) | **GET** /cte/{id}/cancelamento/pdf | Baixar PDF do cancelamento |
*CteApi* | [**baixarPdfCartaCorrecaoCte**](Apis/CteApi.md#baixarpdfcartacorrecaocte) | **GET** /cte/{id}/carta-correcao/pdf | Baixar PDF da carta de correção |
*CteApi* | [**baixarPdfCte**](Apis/CteApi.md#baixarpdfcte) | **GET** /cte/{id}/pdf | Baixar PDF do DACTE |
*CteApi* | [**baixarPdfEventoCte**](Apis/CteApi.md#baixarpdfeventocte) | **GET** /cte/eventos/{id}/pdf | Baixar PDF do evento |
*CteApi* | [**baixarXmlCancelamentoCte**](Apis/CteApi.md#baixarxmlcancelamentocte) | **GET** /cte/{id}/cancelamento/xml | Baixar XML do cancelamento |
*CteApi* | [**baixarXmlCartaCorrecaoCte**](Apis/CteApi.md#baixarxmlcartacorrecaocte) | **GET** /cte/{id}/carta-correcao/xml | Baixar XML da carta de correção |
*CteApi* | [**baixarXmlCte**](Apis/CteApi.md#baixarxmlcte) | **GET** /cte/{id}/xml | Baixar XML do CT-e processado |
*CteApi* | [**baixarXmlCteConhecimento**](Apis/CteApi.md#baixarxmlcteconhecimento) | **GET** /cte/{id}/xml/conhecimento | Baixar XML do CT-e |
*CteApi* | [**baixarXmlCteProtocolo**](Apis/CteApi.md#baixarxmlcteprotocolo) | **GET** /cte/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ |
*CteApi* | [**baixarXmlEventoCte**](Apis/CteApi.md#baixarxmleventocte) | **GET** /cte/eventos/{id}/xml | Baixar XML do evento |
*CteApi* | [**cancelarCte**](Apis/CteApi.md#cancelarcte) | **POST** /cte/{id}/cancelamento | Cancelar um CT-e autorizado |
*CteApi* | [**consultarCancelamentoCte**](Apis/CteApi.md#consultarcancelamentocte) | **GET** /cte/{id}/cancelamento | Consultar o cancelamento do CT-e |
*CteApi* | [**consultarCartaCorrecaoCte**](Apis/CteApi.md#consultarcartacorrecaocte) | **GET** /cte/{id}/carta-correcao | Consultar a solicitação de correção do CT-e |
*CteApi* | [**consultarCte**](Apis/CteApi.md#consultarcte) | **GET** /cte/{id} | Consultar CT-e |
*CteApi* | [**consultarEventoCte**](Apis/CteApi.md#consultareventocte) | **GET** /cte/eventos/{id} | Consultar evento |
*CteApi* | [**consultarStatusSefazCte**](Apis/CteApi.md#consultarstatussefazcte) | **GET** /cte/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora |
*CteApi* | [**criarCartaCorrecaoCte**](Apis/CteApi.md#criarcartacorrecaocte) | **POST** /cte/{id}/carta-correcao | Solicitar correção do CT-e |
*CteApi* | [**emitirCte**](Apis/CteApi.md#emitircte) | **POST** /cte | Emitir CT-e |
*CteApi* | [**emitirCteSimp**](Apis/CteApi.md#emitirctesimp) | **POST** /cte/simp | Emitir CT-e Simplificado |
*CteApi* | [**listarCte**](Apis/CteApi.md#listarcte) | **GET** /cte | Listar CT-e |
*CteApi* | [**sincronizarCte**](Apis/CteApi.md#sincronizarcte) | **POST** /cte/{id}/sincronizar | Sincroniza dados no CT-e a partir da SEFAZ |
| *CteOsApi* | [**baixarPdfCancelamentoCteOs**](Apis/CteOsApi.md#baixarpdfcancelamentocteos) | **GET** /cteos/{id}/cancelamento/pdf | Baixar PDF do cancelamento |
*CteOsApi* | [**baixarPdfCartaCorrecaoCteOs**](Apis/CteOsApi.md#baixarpdfcartacorrecaocteos) | **GET** /cteos/{id}/carta-correcao/pdf | Baixar PDF da carta de correção |
*CteOsApi* | [**baixarPdfCteOs**](Apis/CteOsApi.md#baixarpdfcteos) | **GET** /cteos/{id}/pdf | Baixar PDF do DACTE |
*CteOsApi* | [**baixarPdfEventoCteOs**](Apis/CteOsApi.md#baixarpdfeventocteos) | **GET** /cteos/eventos/{id}/pdf | Baixar PDF do evento |
*CteOsApi* | [**baixarXmlCancelamentoCteOs**](Apis/CteOsApi.md#baixarxmlcancelamentocteos) | **GET** /cteos/{id}/cancelamento/xml | Baixar XML do cancelamento |
*CteOsApi* | [**baixarXmlCartaCorrecaoCteOs**](Apis/CteOsApi.md#baixarxmlcartacorrecaocteos) | **GET** /cteos/{id}/carta-correcao/xml | Baixar XML da carta de correção |
*CteOsApi* | [**baixarXmlCteOs**](Apis/CteOsApi.md#baixarxmlcteos) | **GET** /cteos/{id}/xml | Baixar XML do CT-e OS processado |
*CteOsApi* | [**baixarXmlCteOsConhecimento**](Apis/CteOsApi.md#baixarxmlcteosconhecimento) | **GET** /cteos/{id}/xml/conhecimento | Baixar XML do CT-e OS |
*CteOsApi* | [**baixarXmlCteOsProtocolo**](Apis/CteOsApi.md#baixarxmlcteosprotocolo) | **GET** /cteos/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ |
*CteOsApi* | [**baixarXmlEventoCteOs**](Apis/CteOsApi.md#baixarxmleventocteos) | **GET** /cteos/eventos/{id}/xml | Baixar XML do evento |
*CteOsApi* | [**cancelarCteOs**](Apis/CteOsApi.md#cancelarcteos) | **POST** /cteos/{id}/cancelamento | Cancelar um CT-e OS autorizado |
*CteOsApi* | [**consultarCancelamentoCteOs**](Apis/CteOsApi.md#consultarcancelamentocteos) | **GET** /cteos/{id}/cancelamento | Consultar o cancelamento do CT-e OS |
*CteOsApi* | [**consultarCartaCorrecaoCteOs**](Apis/CteOsApi.md#consultarcartacorrecaocteos) | **GET** /cteos/{id}/carta-correcao | Consultar a solicitação de correção do CT-e OS |
*CteOsApi* | [**consultarCteOs**](Apis/CteOsApi.md#consultarcteos) | **GET** /cteos/{id} | Consultar CT-e OS |
*CteOsApi* | [**consultarEventoCteOs**](Apis/CteOsApi.md#consultareventocteos) | **GET** /cteos/eventos/{id} | Consultar evento |
*CteOsApi* | [**consultarStatusSefazCteOs**](Apis/CteOsApi.md#consultarstatussefazcteos) | **GET** /cteos/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora |
*CteOsApi* | [**criarCartaCorrecaoCteOs**](Apis/CteOsApi.md#criarcartacorrecaocteos) | **POST** /cteos/{id}/carta-correcao | Solicitar correção do CT-e OS |
*CteOsApi* | [**emitirCteOs**](Apis/CteOsApi.md#emitircteos) | **POST** /cteos | Emitir CT-e OS |
*CteOsApi* | [**listarCteOs**](Apis/CteOsApi.md#listarcteos) | **GET** /cteos | Listar CT-e OS |
*CteOsApi* | [**sincronizarCteOs**](Apis/CteOsApi.md#sincronizarcteos) | **POST** /cteos/{id}/sincronizar | Sincroniza dados no CT-e OS a partir da SEFAZ |
| *DceApi* | [**baixarPdfDce**](Apis/DceApi.md#baixarpdfdce) | **GET** /dce/{id}/pdf | Baixar PDF do DACE |
*DceApi* | [**baixarXmlCancelamentoDce**](Apis/DceApi.md#baixarxmlcancelamentodce) | **GET** /dce/{id}/cancelamento/xml | Baixar XML do cancelamento |
*DceApi* | [**baixarXmlDce**](Apis/DceApi.md#baixarxmldce) | **GET** /dce/{id}/xml | Baixar XML da DC-e processada |
*DceApi* | [**baixarXmlDceDeclaracao**](Apis/DceApi.md#baixarxmldcedeclaracao) | **GET** /dce/{id}/xml/declaracao | Baixar XML da DC-e |
*DceApi* | [**baixarXmlDceProtocolo**](Apis/DceApi.md#baixarxmldceprotocolo) | **GET** /dce/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ |
*DceApi* | [**cancelarDce**](Apis/DceApi.md#cancelardce) | **POST** /dce/{id}/cancelamento | Cancelar uma DC-e autorizada |
*DceApi* | [**consultarCancelamentoDce**](Apis/DceApi.md#consultarcancelamentodce) | **GET** /dce/{id}/cancelamento | Consultar o cancelamento da DC-e |
*DceApi* | [**consultarDce**](Apis/DceApi.md#consultardce) | **GET** /dce/{id} | Consultar DC-e |
*DceApi* | [**consultarStatusSefazDce**](Apis/DceApi.md#consultarstatussefazdce) | **GET** /dce/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora |
*DceApi* | [**emitirDce**](Apis/DceApi.md#emitirdce) | **POST** /dce | Emitir DC-e |
*DceApi* | [**listarDce**](Apis/DceApi.md#listardce) | **GET** /dce | Listar DC-e |
| *DebugApi* | [**debugDfe**](Apis/DebugApi.md#debugdfe) | **GET** /debug/{id} | Debug de DF-e |
*DebugApi* | [**debugDfeOriginalPayload**](Apis/DebugApi.md#debugdfeoriginalpayload) | **GET** /debug/{id}/original-payload | Payload original recebido |
*DebugApi* | [**debugHttpRequestContent**](Apis/DebugApi.md#debughttprequestcontent) | **GET** /debug/http-requests/{id}/request-content | Corpo da requisição HTTP |
*DebugApi* | [**debugHttpResponseContent**](Apis/DebugApi.md#debughttpresponsecontent) | **GET** /debug/http-requests/{id}/response-content | Corpo da resposta HTTP |
| *DistribuioNFEApi* | [**baixarPdfDocumentoDistribuicaoNfe**](Apis/DistribuioNFEApi.md#baixarpdfdocumentodistribuicaonfe) | **GET** /distribuicao/nfe/documentos/{id}/pdf | Baixar PDF do documento |
*DistribuioNFEApi* | [**baixarXmlDocumentoDistribuicaoNfe**](Apis/DistribuioNFEApi.md#baixarxmldocumentodistribuicaonfe) | **GET** /distribuicao/nfe/documentos/{id}/xml | Baixar XML do documento |
*DistribuioNFEApi* | [**consultarDistribuicaoNfe**](Apis/DistribuioNFEApi.md#consultardistribuicaonfe) | **GET** /distribuicao/nfe/{id} | Consultar distribuição |
*DistribuioNFEApi* | [**consultarDocumentoDistribuicaoNfe**](Apis/DistribuioNFEApi.md#consultardocumentodistribuicaonfe) | **GET** /distribuicao/nfe/documentos/{id} | Consultar documento |
*DistribuioNFEApi* | [**consultarManifestacaoNfe**](Apis/DistribuioNFEApi.md#consultarmanifestacaonfe) | **GET** /distribuicao/nfe/manifestacoes/{id} | Consultar manifestação |
*DistribuioNFEApi* | [**gerarDistribuicaoNfe**](Apis/DistribuioNFEApi.md#gerardistribuicaonfe) | **POST** /distribuicao/nfe | Distribuir documentos |
*DistribuioNFEApi* | [**listarDistribuicaoNfe**](Apis/DistribuioNFEApi.md#listardistribuicaonfe) | **GET** /distribuicao/nfe | Listar distribuições |
*DistribuioNFEApi* | [**listarDocumentoDistribuicaoNfe**](Apis/DistribuioNFEApi.md#listardocumentodistribuicaonfe) | **GET** /distribuicao/nfe/documentos | Listar documentos |
*DistribuioNFEApi* | [**listarManifestacaoNfe**](Apis/DistribuioNFEApi.md#listarmanifestacaonfe) | **GET** /distribuicao/nfe/manifestacoes | Listar Manifestações |
*DistribuioNFEApi* | [**listarNfeSemManifestacao**](Apis/DistribuioNFEApi.md#listarnfesemmanifestacao) | **GET** /distribuicao/nfe/notas-sem-manifestacao | Listar notas sem manifestação |
*DistribuioNFEApi* | [**manifestarNfe**](Apis/DistribuioNFEApi.md#manifestarnfe) | **POST** /distribuicao/nfe/manifestacoes | Manifestar nota |
| *EmailApi* | [**consultarEmail**](Apis/EmailApi.md#consultaremail) | **GET** /emails/{id} | Consultar e-mail |
*EmailApi* | [**listarEmails**](Apis/EmailApi.md#listaremails) | **GET** /emails | Listar e-mails |
| *EmpresaApi* | [**alterarConfigCte**](Apis/EmpresaApi.md#alterarconfigcte) | **PUT** /empresas/{cpf_cnpj}/cte | Alterar configuração de CT-e |
*EmpresaApi* | [**alterarConfigCteOs**](Apis/EmpresaApi.md#alterarconfigcteos) | **PUT** /empresas/{cpf_cnpj}/cteos | Alterar configuração de CT-e OS |
*EmpresaApi* | [**alterarConfigDce**](Apis/EmpresaApi.md#alterarconfigdce) | **PUT** /empresas/{cpf_cnpj}/dce | Alterar configuração de DC-e |
*EmpresaApi* | [**alterarConfigDistribuicaoNfe**](Apis/EmpresaApi.md#alterarconfigdistribuicaonfe) | **PUT** /empresas/{cpf_cnpj}/distnfe | Alterar configuração de Distribuição de NF-e |
*EmpresaApi* | [**alterarConfigMdfe**](Apis/EmpresaApi.md#alterarconfigmdfe) | **PUT** /empresas/{cpf_cnpj}/mdfe | Alterar configuração de MDF-e |
*EmpresaApi* | [**alterarConfigNfce**](Apis/EmpresaApi.md#alterarconfignfce) | **PUT** /empresas/{cpf_cnpj}/nfce | Alterar configuração de NFC-e |
*EmpresaApi* | [**alterarConfigNfcom**](Apis/EmpresaApi.md#alterarconfignfcom) | **PUT** /empresas/{cpf_cnpj}/nfcom | Alterar configuração de NFCom |
*EmpresaApi* | [**alterarConfigNfe**](Apis/EmpresaApi.md#alterarconfignfe) | **PUT** /empresas/{cpf_cnpj}/nfe | Alterar configuração de NF-e |
*EmpresaApi* | [**alterarConfigNfse**](Apis/EmpresaApi.md#alterarconfignfse) | **PUT** /empresas/{cpf_cnpj}/nfse | Alterar configuração de NFS-e |
*EmpresaApi* | [**atualizarEmpresa**](Apis/EmpresaApi.md#atualizarempresa) | **PUT** /empresas/{cpf_cnpj} | Alterar empresa |
*EmpresaApi* | [**baixarLogotipoEmpresa**](Apis/EmpresaApi.md#baixarlogotipoempresa) | **GET** /empresas/{cpf_cnpj}/logotipo | Baixar logotipo |
*EmpresaApi* | [**cadastrarCertificadoEmpresa**](Apis/EmpresaApi.md#cadastrarcertificadoempresa) | **PUT** /empresas/{cpf_cnpj}/certificado | Cadastrar certificado |
*EmpresaApi* | [**consultarCertificadoEmpresa**](Apis/EmpresaApi.md#consultarcertificadoempresa) | **GET** /empresas/{cpf_cnpj}/certificado | Consultar certificado |
*EmpresaApi* | [**consultarConfigCte**](Apis/EmpresaApi.md#consultarconfigcte) | **GET** /empresas/{cpf_cnpj}/cte | Consultar configuração de CT-e |
*EmpresaApi* | [**consultarConfigCteOs**](Apis/EmpresaApi.md#consultarconfigcteos) | **GET** /empresas/{cpf_cnpj}/cteos | Consultar configuração de CT-e OS |
*EmpresaApi* | [**consultarConfigDce**](Apis/EmpresaApi.md#consultarconfigdce) | **GET** /empresas/{cpf_cnpj}/dce | Consultar configuração de DC-e |
*EmpresaApi* | [**consultarConfigDistribuicaoNfe**](Apis/EmpresaApi.md#consultarconfigdistribuicaonfe) | **GET** /empresas/{cpf_cnpj}/distnfe | Consultar configuração de Distribuição de NF-e |
*EmpresaApi* | [**consultarConfigMdfe**](Apis/EmpresaApi.md#consultarconfigmdfe) | **GET** /empresas/{cpf_cnpj}/mdfe | Consultar configuração de MDF-e |
*EmpresaApi* | [**consultarConfigNfce**](Apis/EmpresaApi.md#consultarconfignfce) | **GET** /empresas/{cpf_cnpj}/nfce | Consultar configuração de NFC-e |
*EmpresaApi* | [**consultarConfigNfcom**](Apis/EmpresaApi.md#consultarconfignfcom) | **GET** /empresas/{cpf_cnpj}/nfcom | Consultar configuração de NFCom |
*EmpresaApi* | [**consultarConfigNfe**](Apis/EmpresaApi.md#consultarconfignfe) | **GET** /empresas/{cpf_cnpj}/nfe | Consultar configuração de NF-e |
*EmpresaApi* | [**consultarConfigNfse**](Apis/EmpresaApi.md#consultarconfignfse) | **GET** /empresas/{cpf_cnpj}/nfse | Consultar configuração de NFS-e |
*EmpresaApi* | [**consultarEmpresa**](Apis/EmpresaApi.md#consultarempresa) | **GET** /empresas/{cpf_cnpj} | Consultar empresa |
*EmpresaApi* | [**criarEmpresa**](Apis/EmpresaApi.md#criarempresa) | **POST** /empresas | Cadastrar empresa |
*EmpresaApi* | [**enviarCertificadoEmpresa**](Apis/EmpresaApi.md#enviarcertificadoempresa) | **PUT** /empresas/{cpf_cnpj}/certificado/upload | Upload de certificado |
*EmpresaApi* | [**enviarLogotipoEmpresa**](Apis/EmpresaApi.md#enviarlogotipoempresa) | **PUT** /empresas/{cpf_cnpj}/logotipo | Enviar logotipo |
*EmpresaApi* | [**excluirCertificadoEmpresa**](Apis/EmpresaApi.md#excluircertificadoempresa) | **DELETE** /empresas/{cpf_cnpj}/certificado | Deletar certificado |
*EmpresaApi* | [**excluirEmpresa**](Apis/EmpresaApi.md#excluirempresa) | **DELETE** /empresas/{cpf_cnpj} | Deletar empresa |
*EmpresaApi* | [**excluirLogotipoEmpresa**](Apis/EmpresaApi.md#excluirlogotipoempresa) | **DELETE** /empresas/{cpf_cnpj}/logotipo | Deletar logotipo |
*EmpresaApi* | [**listarCertificados**](Apis/EmpresaApi.md#listarcertificados) | **GET** /empresas/certificados | Listar certificados |
*EmpresaApi* | [**listarEmpresas**](Apis/EmpresaApi.md#listarempresas) | **GET** /empresas | Listar empresas |
| *MdfeApi* | [**baixarPdfCancelamentoMdfe**](Apis/MdfeApi.md#baixarpdfcancelamentomdfe) | **GET** /mdfe/{id}/cancelamento/pdf | Baixar PDF do cancelamento |
*MdfeApi* | [**baixarPdfEncerramentoMdfe**](Apis/MdfeApi.md#baixarpdfencerramentomdfe) | **GET** /mdfe/{id}/encerramento/pdf | Baixar PDF do encerramento |
*MdfeApi* | [**baixarPdfEventoMdfe**](Apis/MdfeApi.md#baixarpdfeventomdfe) | **GET** /mdfe/eventos/{id}/pdf | Baixar PDF do evento |
*MdfeApi* | [**baixarPdfMdfe**](Apis/MdfeApi.md#baixarpdfmdfe) | **GET** /mdfe/{id}/pdf | Baixar PDF do DAMDFE |
*MdfeApi* | [**baixarXmlCancelamentoMdfe**](Apis/MdfeApi.md#baixarxmlcancelamentomdfe) | **GET** /mdfe/{id}/cancelamento/xml | Baixar XML do cancelamento |
*MdfeApi* | [**baixarXmlEncerramentoMdfe**](Apis/MdfeApi.md#baixarxmlencerramentomdfe) | **GET** /mdfe/{id}/encerramento/xml | Baixar XML do encerramento |
*MdfeApi* | [**baixarXmlEventoMdfe**](Apis/MdfeApi.md#baixarxmleventomdfe) | **GET** /mdfe/eventos/{id}/xml | Baixar XML do evento |
*MdfeApi* | [**baixarXmlMdfe**](Apis/MdfeApi.md#baixarxmlmdfe) | **GET** /mdfe/{id}/xml | Baixar XML do MDF-e processado |
*MdfeApi* | [**baixarXmlMdfeManifesto**](Apis/MdfeApi.md#baixarxmlmdfemanifesto) | **GET** /mdfe/{id}/xml/manifesto | Baixar XML do MDF-e |
*MdfeApi* | [**baixarXmlMdfeProtocolo**](Apis/MdfeApi.md#baixarxmlmdfeprotocolo) | **GET** /mdfe/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ |
*MdfeApi* | [**cancelarMdfe**](Apis/MdfeApi.md#cancelarmdfe) | **POST** /mdfe/{id}/cancelamento | Cancelar um MDF-e autorizado |
*MdfeApi* | [**consultarCancelamentoMdfe**](Apis/MdfeApi.md#consultarcancelamentomdfe) | **GET** /mdfe/{id}/cancelamento | Consultar o cancelamento do MDF-e |
*MdfeApi* | [**consultarEncerramentoMdfe**](Apis/MdfeApi.md#consultarencerramentomdfe) | **GET** /mdfe/{id}/encerramento | Consultar encerramento do MDF-e |
*MdfeApi* | [**consultarEventoMdfe**](Apis/MdfeApi.md#consultareventomdfe) | **GET** /mdfe/eventos/{id} | Consultar evento do MDF-e |
*MdfeApi* | [**consultarLoteMdfe**](Apis/MdfeApi.md#consultarlotemdfe) | **GET** /mdfe/lotes/{id} | Consultar lote de MDF-e |
*MdfeApi* | [**consultarMdfe**](Apis/MdfeApi.md#consultarmdfe) | **GET** /mdfe/{id} | Consultar manifesto |
*MdfeApi* | [**consultarMdfeNaoEncerrados**](Apis/MdfeApi.md#consultarmdfenaoencerrados) | **GET** /mdfe/nao-encerrados | Consulta MDF-e não encerrados |
*MdfeApi* | [**consultarStatusSefazMdfe**](Apis/MdfeApi.md#consultarstatussefazmdfe) | **GET** /mdfe/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora |
*MdfeApi* | [**emitirLoteMdfe**](Apis/MdfeApi.md#emitirlotemdfe) | **POST** /mdfe/lotes | Emitir lote de MDF-e |
*MdfeApi* | [**emitirMdfe**](Apis/MdfeApi.md#emitirmdfe) | **POST** /mdfe | Emitir MDF-e |
*MdfeApi* | [**encerrarMdfe**](Apis/MdfeApi.md#encerrarmdfe) | **POST** /mdfe/{id}/encerramento | Encerrar um MDF-e autorizado |
*MdfeApi* | [**incluirCondutorMdfe**](Apis/MdfeApi.md#incluircondutormdfe) | **POST** /mdfe/{id}/inclusao-condutor | Incluir um condutor em um MDF-e autorizado |
*MdfeApi* | [**incluirDfeMdfe**](Apis/MdfeApi.md#incluirdfemdfe) | **POST** /mdfe/{id}/inclusao-dfe | Incluir um DF-e em um MDF-e autorizado |
*MdfeApi* | [**listarLotesMdfe**](Apis/MdfeApi.md#listarlotesmdfe) | **GET** /mdfe/lotes | Listar lotes de MDF-e |
*MdfeApi* | [**listarMdfe**](Apis/MdfeApi.md#listarmdfe) | **GET** /mdfe | Listar MDF-e |
*MdfeApi* | [**sincronizarMdfe**](Apis/MdfeApi.md#sincronizarmdfe) | **POST** /mdfe/{id}/sincronizar | Sincroniza dados no MDF-e a partir da SEFAZ |
| *NfceApi* | [**baixarEscPosNfce**](Apis/NfceApi.md#baixarescposnfce) | **GET** /nfce/{id}/escpos | Comandos ESC/POS para impressão do DANFCE |
*NfceApi* | [**baixarPdfCancelamentoNfce**](Apis/NfceApi.md#baixarpdfcancelamentonfce) | **GET** /nfce/{id}/cancelamento/pdf | Baixar PDF do cancelamento |
*NfceApi* | [**baixarPdfEventoNfce**](Apis/NfceApi.md#baixarpdfeventonfce) | **GET** /nfce/eventos/{id}/pdf | Baixar PDF do evento |
*NfceApi* | [**baixarPdfInutilizacaoNfce**](Apis/NfceApi.md#baixarpdfinutilizacaonfce) | **GET** /nfce/inutilizacoes/{id}/pdf | Baixar PDF da inutilização |
*NfceApi* | [**baixarPdfNfce**](Apis/NfceApi.md#baixarpdfnfce) | **GET** /nfce/{id}/pdf | Baixar PDF do DANFCE |
*NfceApi* | [**baixarPreviaPdfNfce**](Apis/NfceApi.md#baixarpreviapdfnfce) | **POST** /nfce/previa/pdf | Prévia do PDF do DANFCE |
*NfceApi* | [**baixarPreviaXmlNfce**](Apis/NfceApi.md#baixarpreviaxmlnfce) | **POST** /nfce/previa/xml | Prévia do XML da NFC-e |
*NfceApi* | [**baixarXmlCancelamentoNfce**](Apis/NfceApi.md#baixarxmlcancelamentonfce) | **GET** /nfce/{id}/cancelamento/xml | Baixar XML do cancelamento |
*NfceApi* | [**baixarXmlEventoNfce**](Apis/NfceApi.md#baixarxmleventonfce) | **GET** /nfce/eventos/{id}/xml | Baixar XML do evento |
*NfceApi* | [**baixarXmlInutilizacaoNfce**](Apis/NfceApi.md#baixarxmlinutilizacaonfce) | **GET** /nfce/inutilizacoes/{id}/xml | Baixar XML da inutilização |
*NfceApi* | [**baixarXmlNfce**](Apis/NfceApi.md#baixarxmlnfce) | **GET** /nfce/{id}/xml | Baixar XML da NFC-e processada |
*NfceApi* | [**baixarXmlNfceNota**](Apis/NfceApi.md#baixarxmlnfcenota) | **GET** /nfce/{id}/xml/nota | Baixar XML da NFC-e |
*NfceApi* | [**baixarXmlNfceProtocolo**](Apis/NfceApi.md#baixarxmlnfceprotocolo) | **GET** /nfce/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ |
*NfceApi* | [**cancelarNfce**](Apis/NfceApi.md#cancelarnfce) | **POST** /nfce/{id}/cancelamento | Cancelar uma NFC-e autorizada |
*NfceApi* | [**consultarCancelamentoNfce**](Apis/NfceApi.md#consultarcancelamentonfce) | **GET** /nfce/{id}/cancelamento | Consultar o cancelamento da NFC-e |
*NfceApi* | [**consultarEventoNfce**](Apis/NfceApi.md#consultareventonfce) | **GET** /nfce/eventos/{id} | Consultar evento |
*NfceApi* | [**consultarInutilizacaoNfce**](Apis/NfceApi.md#consultarinutilizacaonfce) | **GET** /nfce/inutilizacoes/{id} | Consultar a inutilização de sequência de numeração |
*NfceApi* | [**consultarLoteNfce**](Apis/NfceApi.md#consultarlotenfce) | **GET** /nfce/lotes/{id} | Consultar lote de NFC-e |
*NfceApi* | [**consultarNfce**](Apis/NfceApi.md#consultarnfce) | **GET** /nfce/{id} | Consultar NFC-e |
*NfceApi* | [**consultarStatusSefazNfce**](Apis/NfceApi.md#consultarstatussefaznfce) | **GET** /nfce/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora |
*NfceApi* | [**emitirLoteNfce**](Apis/NfceApi.md#emitirlotenfce) | **POST** /nfce/lotes | Emitir lote de NFC-e |
*NfceApi* | [**emitirNfce**](Apis/NfceApi.md#emitirnfce) | **POST** /nfce | Emitir NFC-e |
*NfceApi* | [**enviarEmailNfce**](Apis/NfceApi.md#enviaremailnfce) | **POST** /nfce/{id}/email | Enviar e-mail |
*NfceApi* | [**inutilizarNumeracaoNfce**](Apis/NfceApi.md#inutilizarnumeracaonfce) | **POST** /nfce/inutilizacoes | Inutilizar uma sequência de numeração de NFC-e |
*NfceApi* | [**listarEventosNfce**](Apis/NfceApi.md#listareventosnfce) | **GET** /nfce/eventos | Listar eventos |
*NfceApi* | [**listarLotesNfce**](Apis/NfceApi.md#listarlotesnfce) | **GET** /nfce/lotes | Listar lotes de NFC-e |
*NfceApi* | [**listarNfce**](Apis/NfceApi.md#listarnfce) | **GET** /nfce | Listar NFC-e |
*NfceApi* | [**sincronizarNfce**](Apis/NfceApi.md#sincronizarnfce) | **POST** /nfce/{id}/sincronizar | Sincroniza dados na NFC-e a partir da SEFAZ |
| *NfcomApi* | [**baixarPdfNfcom**](Apis/NfcomApi.md#baixarpdfnfcom) | **GET** /nfcom/{id}/pdf | Baixar PDF do DANFE-COM |
*NfcomApi* | [**baixarXmlCancelamentoNfcom**](Apis/NfcomApi.md#baixarxmlcancelamentonfcom) | **GET** /nfcom/{id}/cancelamento/xml | Baixar XML do cancelamento |
*NfcomApi* | [**baixarXmlNfcom**](Apis/NfcomApi.md#baixarxmlnfcom) | **GET** /nfcom/{id}/xml | Baixar XML da NFCom processada |
*NfcomApi* | [**baixarXmlNfcomNota**](Apis/NfcomApi.md#baixarxmlnfcomnota) | **GET** /nfcom/{id}/xml/nota | Baixar XML da NFCom |
*NfcomApi* | [**baixarXmlNfcomProtocolo**](Apis/NfcomApi.md#baixarxmlnfcomprotocolo) | **GET** /nfcom/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ |
*NfcomApi* | [**cancelarNfcom**](Apis/NfcomApi.md#cancelarnfcom) | **POST** /nfcom/{id}/cancelamento | Cancelar uma NFCom autorizada |
*NfcomApi* | [**consultarCancelamentoNfcom**](Apis/NfcomApi.md#consultarcancelamentonfcom) | **GET** /nfcom/{id}/cancelamento | Consultar o cancelamento da NFCom |
*NfcomApi* | [**consultarNfcom**](Apis/NfcomApi.md#consultarnfcom) | **GET** /nfcom/{id} | Consultar NFCom |
*NfcomApi* | [**consultarStatusSefazNfcom**](Apis/NfcomApi.md#consultarstatussefaznfcom) | **GET** /nfcom/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora |
*NfcomApi* | [**emitirNfcom**](Apis/NfcomApi.md#emitirnfcom) | **POST** /nfcom | Emitir NFCom |
*NfcomApi* | [**listarNfcom**](Apis/NfcomApi.md#listarnfcom) | **GET** /nfcom | Listar NFCom |
| *NfeApi* | [**baixarPdfCancelamentoNfe**](Apis/NfeApi.md#baixarpdfcancelamentonfe) | **GET** /nfe/{id}/cancelamento/pdf | Baixar PDF do cancelamento |
*NfeApi* | [**baixarPdfCartaCorrecaoNfe**](Apis/NfeApi.md#baixarpdfcartacorrecaonfe) | **GET** /nfe/{id}/carta-correcao/pdf | Baixar PDF da carta de correção |
*NfeApi* | [**baixarPdfEventoNfe**](Apis/NfeApi.md#baixarpdfeventonfe) | **GET** /nfe/eventos/{id}/pdf | Baixar PDF do evento |
*NfeApi* | [**baixarPdfInutilizacaoNfe**](Apis/NfeApi.md#baixarpdfinutilizacaonfe) | **GET** /nfe/inutilizacoes/{id}/pdf | Baixar PDF da inutilização |
*NfeApi* | [**baixarPdfNfe**](Apis/NfeApi.md#baixarpdfnfe) | **GET** /nfe/{id}/pdf | Baixar PDF do DANFE |
*NfeApi* | [**baixarPreviaPdfNfe**](Apis/NfeApi.md#baixarpreviapdfnfe) | **POST** /nfe/previa/pdf | Prévia do PDF do DANFE |
*NfeApi* | [**baixarPreviaXmlNfe**](Apis/NfeApi.md#baixarpreviaxmlnfe) | **POST** /nfe/previa/xml | Prévia do XML da NF-e |
*NfeApi* | [**baixarXmlCancelamentoNfe**](Apis/NfeApi.md#baixarxmlcancelamentonfe) | **GET** /nfe/{id}/cancelamento/xml | Baixar XML do cancelamento |
*NfeApi* | [**baixarXmlCartaCorrecaoNfe**](Apis/NfeApi.md#baixarxmlcartacorrecaonfe) | **GET** /nfe/{id}/carta-correcao/xml | Baixar XML da carta de correção |
*NfeApi* | [**baixarXmlEventoNfe**](Apis/NfeApi.md#baixarxmleventonfe) | **GET** /nfe/eventos/{id}/xml | Baixar XML do evento |
*NfeApi* | [**baixarXmlInutilizacaoNfe**](Apis/NfeApi.md#baixarxmlinutilizacaonfe) | **GET** /nfe/inutilizacoes/{id}/xml | Baixar XML da inutilização |
*NfeApi* | [**baixarXmlNfe**](Apis/NfeApi.md#baixarxmlnfe) | **GET** /nfe/{id}/xml | Baixar XML da NF-e processada |
*NfeApi* | [**baixarXmlNfeNota**](Apis/NfeApi.md#baixarxmlnfenota) | **GET** /nfe/{id}/xml/nota | Baixar XML da NF-e |
*NfeApi* | [**baixarXmlNfeProtocolo**](Apis/NfeApi.md#baixarxmlnfeprotocolo) | **GET** /nfe/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ |
*NfeApi* | [**cancelarNfe**](Apis/NfeApi.md#cancelarnfe) | **POST** /nfe/{id}/cancelamento | Cancelar uma NF-e autorizada |
*NfeApi* | [**consultarCancelamentoNfe**](Apis/NfeApi.md#consultarcancelamentonfe) | **GET** /nfe/{id}/cancelamento | Consultar o cancelamento da NF-e |
*NfeApi* | [**consultarCartaCorrecaoNfe**](Apis/NfeApi.md#consultarcartacorrecaonfe) | **GET** /nfe/{id}/carta-correcao | Consultar a solicitação de correção da NF-e |
*NfeApi* | [**consultarContribuinteNfe**](Apis/NfeApi.md#consultarcontribuintenfe) | **GET** /nfe/cadastro-contribuinte | Consultar contribuinte |
*NfeApi* | [**consultarEventoNfe**](Apis/NfeApi.md#consultareventonfe) | **GET** /nfe/eventos/{id} | Consultar evento |
*NfeApi* | [**consultarInutilizacaoNfe**](Apis/NfeApi.md#consultarinutilizacaonfe) | **GET** /nfe/inutilizacoes/{id} | Consultar a inutilização de sequência de numeração |
*NfeApi* | [**consultarLoteNfe**](Apis/NfeApi.md#consultarlotenfe) | **GET** /nfe/lotes/{id} | Consultar lote de NF-e |
*NfeApi* | [**consultarNfe**](Apis/NfeApi.md#consultarnfe) | **GET** /nfe/{id} | Consultar NF-e |
*NfeApi* | [**consultarStatusSefazNfe**](Apis/NfeApi.md#consultarstatussefaznfe) | **GET** /nfe/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora |
*NfeApi* | [**criarCartaCorrecaoNfe**](Apis/NfeApi.md#criarcartacorrecaonfe) | **POST** /nfe/{id}/carta-correcao | Solicitar correção da NF-e |
*NfeApi* | [**emitirLoteNfe**](Apis/NfeApi.md#emitirlotenfe) | **POST** /nfe/lotes | Emitir lote de NF-e |
*NfeApi* | [**emitirNfe**](Apis/NfeApi.md#emitirnfe) | **POST** /nfe | Emitir NF-e |
*NfeApi* | [**enviarEmailNfe**](Apis/NfeApi.md#enviaremailnfe) | **POST** /nfe/{id}/email | Enviar e-mail |
*NfeApi* | [**inutilizarNumeracaoNfe**](Apis/NfeApi.md#inutilizarnumeracaonfe) | **POST** /nfe/inutilizacoes | Inutilizar uma sequência de numeração de NF-e |
*NfeApi* | [**listarEventosNfe**](Apis/NfeApi.md#listareventosnfe) | **GET** /nfe/eventos | Listar eventos |
*NfeApi* | [**listarLotesNfe**](Apis/NfeApi.md#listarlotesnfe) | **GET** /nfe/lotes | Listar lotes de NF-e |
*NfeApi* | [**listarNfe**](Apis/NfeApi.md#listarnfe) | **GET** /nfe | Listar NF-e |
*NfeApi* | [**sincronizarNfe**](Apis/NfeApi.md#sincronizarnfe) | **POST** /nfe/{id}/sincronizar | Sincroniza dados na NF-e a partir da SEFAZ |
| *NfseApi* | [**baixarPdfNfse**](Apis/NfseApi.md#baixarpdfnfse) | **GET** /nfse/{id}/pdf | Baixar PDF do DANFSE |
*NfseApi* | [**baixarXmlCancelamentoNfse**](Apis/NfseApi.md#baixarxmlcancelamentonfse) | **GET** /nfse/{Id}/cancelamento/xml | Baixar XML do evento de cancelamento |
*NfseApi* | [**baixarXmlDps**](Apis/NfseApi.md#baixarxmldps) | **GET** /nfse/{id}/xml/dps | Baixar XML da DPS |
*NfseApi* | [**baixarXmlNfse**](Apis/NfseApi.md#baixarxmlnfse) | **GET** /nfse/{id}/xml | Baixar XML da NFS-e processada |
*NfseApi* | [**cancelarNfse**](Apis/NfseApi.md#cancelarnfse) | **POST** /nfse/{id}/cancelamento | Cancelar uma NFS-e autorizada |
*NfseApi* | [**cidadesAtendidas**](Apis/NfseApi.md#cidadesatendidas) | **GET** /nfse/cidades | Cidades atendidas |
*NfseApi* | [**consultarCancelamentoNfse**](Apis/NfseApi.md#consultarcancelamentonfse) | **GET** /nfse/{id}/cancelamento | Consultar o cancelamento da NFS-e |
*NfseApi* | [**consultarLoteNfse**](Apis/NfseApi.md#consultarlotenfse) | **GET** /nfse/lotes/{id} | Consultar lote de NFS-e |
*NfseApi* | [**consultarMetadados**](Apis/NfseApi.md#consultarmetadados) | **GET** /nfse/cidades/{codigo_ibge} | Consultar metadados |
*NfseApi* | [**consultarNfse**](Apis/NfseApi.md#consultarnfse) | **GET** /nfse/{id} | Consultar NFS-e |
*NfseApi* | [**emitirLoteNfse**](Apis/NfseApi.md#emitirlotenfse) | **POST** /nfse/lotes | Emitir lote de NFS-e |
*NfseApi* | [**emitirLoteNfseDps**](Apis/NfseApi.md#emitirlotenfsedps) | **POST** /nfse/dps/lotes | Emitir lote de NFS-e |
*NfseApi* | [**emitirNfse**](Apis/NfseApi.md#emitirnfse) | **POST** /nfse | Emitir NFS-e |
*NfseApi* | [**emitirNfseDps**](Apis/NfseApi.md#emitirnfsedps) | **POST** /nfse/dps | Emitir NFS-e |
*NfseApi* | [**listarLotesNfse**](Apis/NfseApi.md#listarlotesnfse) | **GET** /nfse/lotes | Listar lotes de NFS-e |
*NfseApi* | [**listarNfse**](Apis/NfseApi.md#listarnfse) | **GET** /nfse | Listar NFS-e |
*NfseApi* | [**sincronizarNfse**](Apis/NfseApi.md#sincronizarnfse) | **POST** /nfse/{id}/sincronizar | Sincroniza dados na NFS-e a partir da Prefeitura |


<a name="documentation-for-models"></a>
## Documentação dos DTOs

 - [AtvEvento](./Models/AtvEvento.md)
 - [BeneficioMunicipal](./Models/BeneficioMunicipal.md)
 - [CServ](./Models/CServ.md)
 - [CepEndereco](./Models/CepEndereco.md)
 - [CnpjCnae](./Models/CnpjCnae.md)
 - [CnpjCnaeSecundario](./Models/CnpjCnaeSecundario.md)
 - [CnpjEmpresa](./Models/CnpjEmpresa.md)
 - [CnpjEndereco](./Models/CnpjEndereco.md)
 - [CnpjFaixaEtaria](./Models/CnpjFaixaEtaria.md)
 - [CnpjIdentificadorSocio](./Models/CnpjIdentificadorSocio.md)
 - [CnpjListagem](./Models/CnpjListagem.md)
 - [CnpjMotivoSituacaoCadastral](./Models/CnpjMotivoSituacaoCadastral.md)
 - [CnpjMunicipio](./Models/CnpjMunicipio.md)
 - [CnpjNaturezaJuridica](./Models/CnpjNaturezaJuridica.md)
 - [CnpjOpcaoSimei](./Models/CnpjOpcaoSimei.md)
 - [CnpjOpcaoSimples](./Models/CnpjOpcaoSimples.md)
 - [CnpjPais](./Models/CnpjPais.md)
 - [CnpjPorteEmpresa](./Models/CnpjPorteEmpresa.md)
 - [CnpjQualificacaoSocio](./Models/CnpjQualificacaoSocio.md)
 - [CnpjRepresentanteLegal](./Models/CnpjRepresentanteLegal.md)
 - [CnpjSituacaoCadastral](./Models/CnpjSituacaoCadastral.md)
 - [CnpjSituacaoEspecial](./Models/CnpjSituacaoEspecial.md)
 - [CnpjSocio](./Models/CnpjSocio.md)
 - [CnpjTelefone](./Models/CnpjTelefone.md)
 - [ComExterior](./Models/ComExterior.md)
 - [ContaCota](./Models/ContaCota.md)
 - [ContaCotaListagem](./Models/ContaCotaListagem.md)
 - [ContaCotaPrePago](./Models/ContaCotaPrePago.md)
 - [ContaExtratoCredito](./Models/ContaExtratoCredito.md)
 - [ContaExtratoCreditoListagem](./Models/ContaExtratoCreditoListagem.md)
 - [CteCartaCorrecao](./Models/CteCartaCorrecao.md)
 - [CteInfCorrecao](./Models/CteInfCorrecao.md)
 - [CteOsCartaCorrecao](./Models/CteOsCartaCorrecao.md)
 - [CteOsInfCorrecao](./Models/CteOsInfCorrecao.md)
 - [CteOsPedidoCancelamento](./Models/CteOsPedidoCancelamento.md)
 - [CteOsPedidoCartaCorrecao](./Models/CteOsPedidoCartaCorrecao.md)
 - [CteOsPedidoEmissao](./Models/CteOsPedidoEmissao.md)
 - [CteOsSefazALCZFMCBSOS](./Models/CteOsSefazALCZFMCBSOS.md)
 - [CteOsSefazAutXMLOS](./Models/CteOsSefazAutXMLOS.md)
 - [CteOsSefazCIBSOS](./Models/CteOsSefazCIBSOS.md)
 - [CteOsSefazCobrOS](./Models/CteOsSefazCobrOS.md)
 - [CteOsSefazCompOS](./Models/CteOsSefazCompOS.md)
 - [CteOsSefazComplOS](./Models/CteOsSefazComplOS.md)
 - [CteOsSefazCompraGovReduzidoOS](./Models/CteOsSefazCompraGovReduzidoOS.md)
 - [CteOsSefazDevTribOS](./Models/CteOsSefazDevTribOS.md)
 - [CteOsSefazDifOS](./Models/CteOsSefazDifOS.md)
 - [CteOsSefazDupOS](./Models/CteOsSefazDupOS.md)
 - [CteOsSefazEmitOS](./Models/CteOsSefazEmitOS.md)
 - [CteOsSefazEndeEmiOS](./Models/CteOsSefazEndeEmiOS.md)
 - [CteOsSefazEnderecoOS](./Models/CteOsSefazEnderecoOS.md)
 - [CteOsSefazEstornoCredOS](./Models/CteOsSefazEstornoCredOS.md)
 - [CteOsSefazFatOS](./Models/CteOsSefazFatOS.md)
 - [CteOsSefazGCBSOS](./Models/CteOsSefazGCBSOS.md)
 - [CteOsSefazGIBSMunOS](./Models/CteOsSefazGIBSMunOS.md)
 - [CteOsSefazGIBSUFOS](./Models/CteOsSefazGIBSUFOS.md)
 - [CteOsSefazGPagAntecipadoOS](./Models/CteOsSefazGPagAntecipadoOS.md)
 - [CteOsSefazICMS00OS](./Models/CteOsSefazICMS00OS.md)
 - [CteOsSefazICMS20OS](./Models/CteOsSefazICMS20OS.md)
 - [CteOsSefazICMS45OS](./Models/CteOsSefazICMS45OS.md)
 - [CteOsSefazICMS90OS](./Models/CteOsSefazICMS90OS.md)
 - [CteOsSefazICMSOutraUFOS](./Models/CteOsSefazICMSOutraUFOS.md)
 - [CteOsSefazICMSSNOS](./Models/CteOsSefazICMSSNOS.md)
 - [CteOsSefazICMSUFFimOS](./Models/CteOsSefazICMSUFFimOS.md)
 - [CteOsSefazIdeOS](./Models/CteOsSefazIdeOS.md)
 - [CteOsSefazImpOS](./Models/CteOsSefazImpOS.md)
 - [CteOsSefazInfCTeNormOS](./Models/CteOsSefazInfCTeNormOS.md)
 - [CteOsSefazInfCTeSuplOS](./Models/CteOsSefazInfCTeSuplOS.md)
 - [CteOsSefazInfCteCompOS](./Models/CteOsSefazInfCteCompOS.md)
 - [CteOsSefazInfCteOS](./Models/CteOsSefazInfCteOS.md)
 - [CteOsSefazInfCteSubOS](./Models/CteOsSefazInfCteSubOS.md)
 - [CteOsSefazInfCte_ImpOS](./Models/CteOsSefazInfCte_ImpOS.md)
 - [CteOsSefazInfDocRefOS](./Models/CteOsSefazInfDocRefOS.md)
 - [CteOsSefazInfFretamentoOS](./Models/CteOsSefazInfFretamentoOS.md)
 - [CteOsSefazInfGTVeOS](./Models/CteOsSefazInfGTVeOS.md)
 - [CteOsSefazInfGTVe_CompOS](./Models/CteOsSefazInfGTVe_CompOS.md)
 - [CteOsSefazInfModalOS](./Models/CteOsSefazInfModalOS.md)
 - [CteOsSefazInfPercursoOS](./Models/CteOsSefazInfPercursoOS.md)
 - [CteOsSefazInfQOS](./Models/CteOsSefazInfQOS.md)
 - [CteOsSefazInfServicoOS](./Models/CteOsSefazInfServicoOS.md)
 - [CteOsSefazInfTribFedOS](./Models/CteOsSefazInfTribFedOS.md)
 - [CteOsSefazObsContOS](./Models/CteOsSefazObsContOS.md)
 - [CteOsSefazObsFiscoOS](./Models/CteOsSefazObsFiscoOS.md)
 - [CteOsSefazPagamentoRTCOS](./Models/CteOsSefazPagamentoRTCOS.md)
 - [CteOsSefazPgtoVincOS](./Models/CteOsSefazPgtoVincOS.md)
 - [CteOsSefazPropOS](./Models/CteOsSefazPropOS.md)
 - [CteOsSefazRedOS](./Models/CteOsSefazRedOS.md)
 - [CteOsSefazRespTecOS](./Models/CteOsSefazRespTecOS.md)
 - [CteOsSefazRodoOS](./Models/CteOsSefazRodoOS.md)
 - [CteOsSefazSegOS](./Models/CteOsSefazSegOS.md)
 - [CteOsSefazTomaOS](./Models/CteOsSefazTomaOS.md)
 - [CteOsSefazTribCTeOS](./Models/CteOsSefazTribCTeOS.md)
 - [CteOsSefazTribCompraGovOS](./Models/CteOsSefazTribCompraGovOS.md)
 - [CteOsSefazTribRegularOS](./Models/CteOsSefazTribRegularOS.md)
 - [CteOsSefazVPrestOS](./Models/CteOsSefazVPrestOS.md)
 - [CteOsSefazVeicOS](./Models/CteOsSefazVeicOS.md)
 - [CtePedidoCancelamento](./Models/CtePedidoCancelamento.md)
 - [CtePedidoCartaCorrecao](./Models/CtePedidoCartaCorrecao.md)
 - [CtePedidoEmissao](./Models/CtePedidoEmissao.md)
 - [CteSefazALCZFMCBS](./Models/CteSefazALCZFMCBS.md)
 - [CteSefazAereo](./Models/CteSefazAereo.md)
 - [CteSefazAquav](./Models/CteSefazAquav.md)
 - [CteSefazAutXML](./Models/CteSefazAutXML.md)
 - [CteSefazBalsa](./Models/CteSefazBalsa.md)
 - [CteSefazCIBS](./Models/CteSefazCIBS.md)
 - [CteSefazCobr](./Models/CteSefazCobr.md)
 - [CteSefazComData](./Models/CteSefazComData.md)
 - [CteSefazComHora](./Models/CteSefazComHora.md)
 - [CteSefazComp](./Models/CteSefazComp.md)
 - [CteSefazCompl](./Models/CteSefazCompl.md)
 - [CteSefazCompraGovReduzido](./Models/CteSefazCompraGovReduzido.md)
 - [CteSefazDest](./Models/CteSefazDest.md)
 - [CteSefazDetCont](./Models/CteSefazDetCont.md)
 - [CteSefazDetCont_InfDoc](./Models/CteSefazDetCont_InfDoc.md)
 - [CteSefazDetCont_InfDoc_InfNF](./Models/CteSefazDetCont_InfDoc_InfNF.md)
 - [CteSefazDetCont_InfDoc_InfNFe](./Models/CteSefazDetCont_InfDoc_InfNFe.md)
 - [CteSefazDevTrib](./Models/CteSefazDevTrib.md)
 - [CteSefazDif](./Models/CteSefazDif.md)
 - [CteSefazDocAnt](./Models/CteSefazDocAnt.md)
 - [CteSefazDup](./Models/CteSefazDup.md)
 - [CteSefazDuto](./Models/CteSefazDuto.md)
 - [CteSefazEmiDocAnt](./Models/CteSefazEmiDocAnt.md)
 - [CteSefazEmiOcc](./Models/CteSefazEmiOcc.md)
 - [CteSefazEmit](./Models/CteSefazEmit.md)
 - [CteSefazEndeEmi](./Models/CteSefazEndeEmi.md)
 - [CteSefazEnderFer](./Models/CteSefazEnderFer.md)
 - [CteSefazEndereco](./Models/CteSefazEndereco.md)
 - [CteSefazEntrega](./Models/CteSefazEntrega.md)
 - [CteSefazEstornoCred](./Models/CteSefazEstornoCred.md)
 - [CteSefazExped](./Models/CteSefazExped.md)
 - [CteSefazFat](./Models/CteSefazFat.md)
 - [CteSefazFerroEnv](./Models/CteSefazFerroEnv.md)
 - [CteSefazFerrov](./Models/CteSefazFerrov.md)
 - [CteSefazFluxo](./Models/CteSefazFluxo.md)
 - [CteSefazGCBS](./Models/CteSefazGCBS.md)
 - [CteSefazGIBSMun](./Models/CteSefazGIBSMun.md)
 - [CteSefazGIBSUF](./Models/CteSefazGIBSUF.md)
 - [CteSefazGPagAntecipado](./Models/CteSefazGPagAntecipado.md)
 - [CteSefazICMS00](./Models/CteSefazICMS00.md)
 - [CteSefazICMS20](./Models/CteSefazICMS20.md)
 - [CteSefazICMS45](./Models/CteSefazICMS45.md)
 - [CteSefazICMS60](./Models/CteSefazICMS60.md)
 - [CteSefazICMS90](./Models/CteSefazICMS90.md)
 - [CteSefazICMSOutraUF](./Models/CteSefazICMSOutraUF.md)
 - [CteSefazICMSSN](./Models/CteSefazICMSSN.md)
 - [CteSefazICMSUFFim](./Models/CteSefazICMSUFFim.md)
 - [CteSefazIdDocAnt](./Models/CteSefazIdDocAnt.md)
 - [CteSefazIdDocAntEle](./Models/CteSefazIdDocAntEle.md)
 - [CteSefazIdDocAntPap](./Models/CteSefazIdDocAntPap.md)
 - [CteSefazIde](./Models/CteSefazIde.md)
 - [CteSefazImp](./Models/CteSefazImp.md)
 - [CteSefazInfCTeMultimodal](./Models/CteSefazInfCTeMultimodal.md)
 - [CteSefazInfCTeNorm](./Models/CteSefazInfCTeNorm.md)
 - [CteSefazInfCTeSupl](./Models/CteSefazInfCTeSupl.md)
 - [CteSefazInfCarga](./Models/CteSefazInfCarga.md)
 - [CteSefazInfCte](./Models/CteSefazInfCte.md)
 - [CteSefazInfCteComp](./Models/CteSefazInfCteComp.md)
 - [CteSefazInfCteSub](./Models/CteSefazInfCteSub.md)
 - [CteSefazInfCte_Imp](./Models/CteSefazInfCte_Imp.md)
 - [CteSefazInfDCe](./Models/CteSefazInfDCe.md)
 - [CteSefazInfDoc](./Models/CteSefazInfDoc.md)
 - [CteSefazInfGlobalizado](./Models/CteSefazInfGlobalizado.md)
 - [CteSefazInfModal](./Models/CteSefazInfModal.md)
 - [CteSefazInfNF](./Models/CteSefazInfNF.md)
 - [CteSefazInfNFe](./Models/CteSefazInfNFe.md)
 - [CteSefazInfOutros](./Models/CteSefazInfOutros.md)
 - [CteSefazInfQ](./Models/CteSefazInfQ.md)
 - [CteSefazInfSeg](./Models/CteSefazInfSeg.md)
 - [CteSefazInfServVinc](./Models/CteSefazInfServVinc.md)
 - [CteSefazInfSolicNFF](./Models/CteSefazInfSolicNFF.md)
 - [CteSefazInfTotAP](./Models/CteSefazInfTotAP.md)
 - [CteSefazLacUnidCarga](./Models/CteSefazLacUnidCarga.md)
 - [CteSefazLacUnidTransp](./Models/CteSefazLacUnidTransp.md)
 - [CteSefazLacre](./Models/CteSefazLacre.md)
 - [CteSefazMultimodal](./Models/CteSefazMultimodal.md)
 - [CteSefazNatCarga](./Models/CteSefazNatCarga.md)
 - [CteSefazNoInter](./Models/CteSefazNoInter.md)
 - [CteSefazNoPeriodo](./Models/CteSefazNoPeriodo.md)
 - [CteSefazObsCont](./Models/CteSefazObsCont.md)
 - [CteSefazObsFisco](./Models/CteSefazObsFisco.md)
 - [CteSefazOcc](./Models/CteSefazOcc.md)
 - [CteSefazPagamentoRTC](./Models/CteSefazPagamentoRTC.md)
 - [CteSefazPass](./Models/CteSefazPass.md)
 - [CteSefazPeri](./Models/CteSefazPeri.md)
 - [CteSefazPgtoVinc](./Models/CteSefazPgtoVinc.md)
 - [CteSefazReceb](./Models/CteSefazReceb.md)
 - [CteSefazRed](./Models/CteSefazRed.md)
 - [CteSefazRem](./Models/CteSefazRem.md)
 - [CteSefazRespTec](./Models/CteSefazRespTec.md)
 - [CteSefazRodo](./Models/CteSefazRodo.md)
 - [CteSefazSeg](./Models/CteSefazSeg.md)
 - [CteSefazSemData](./Models/CteSefazSemData.md)
 - [CteSefazSemHora](./Models/CteSefazSemHora.md)
 - [CteSefazTarifa](./Models/CteSefazTarifa.md)
 - [CteSefazToma3](./Models/CteSefazToma3.md)
 - [CteSefazToma4](./Models/CteSefazToma4.md)
 - [CteSefazTrafMut](./Models/CteSefazTrafMut.md)
 - [CteSefazTribCTe](./Models/CteSefazTribCTe.md)
 - [CteSefazTribCompraGov](./Models/CteSefazTribCompraGov.md)
 - [CteSefazTribRegular](./Models/CteSefazTribRegular.md)
 - [CteSefazUnidCarga](./Models/CteSefazUnidCarga.md)
 - [CteSefazUnidadeTransp](./Models/CteSefazUnidadeTransp.md)
 - [CteSefazVPrest](./Models/CteSefazVPrest.md)
 - [CteSefazVeicNovos](./Models/CteSefazVeicNovos.md)
 - [CteSimpPedidoEmissao](./Models/CteSimpPedidoEmissao.md)
 - [CteSimpSefazALCZFMCBSSimp](./Models/CteSimpSefazALCZFMCBSSimp.md)
 - [CteSimpSefazAereoSimp](./Models/CteSimpSefazAereoSimp.md)
 - [CteSimpSefazAquavSimp](./Models/CteSimpSefazAquavSimp.md)
 - [CteSimpSefazAutXMLSimp](./Models/CteSimpSefazAutXMLSimp.md)
 - [CteSimpSefazBalsaSimp](./Models/CteSimpSefazBalsaSimp.md)
 - [CteSimpSefazCIBSSimp](./Models/CteSimpSefazCIBSSimp.md)
 - [CteSimpSefazCobrSimp](./Models/CteSimpSefazCobrSimp.md)
 - [CteSimpSefazCompSimp](./Models/CteSimpSefazCompSimp.md)
 - [CteSimpSefazComplSimp](./Models/CteSimpSefazComplSimp.md)
 - [CteSimpSefazCompraGovReduzidoSimp](./Models/CteSimpSefazCompraGovReduzidoSimp.md)
 - [CteSimpSefazDetContSimp](./Models/CteSimpSefazDetContSimp.md)
 - [CteSimpSefazDetSimp](./Models/CteSimpSefazDetSimp.md)
 - [CteSimpSefazDevTribSimp](./Models/CteSimpSefazDevTribSimp.md)
 - [CteSimpSefazDifSimp](./Models/CteSimpSefazDifSimp.md)
 - [CteSimpSefazDupSimp](./Models/CteSimpSefazDupSimp.md)
 - [CteSimpSefazDutoSimp](./Models/CteSimpSefazDutoSimp.md)
 - [CteSimpSefazEmiOccSimp](./Models/CteSimpSefazEmiOccSimp.md)
 - [CteSimpSefazEmitSimp](./Models/CteSimpSefazEmitSimp.md)
 - [CteSimpSefazEndeEmiSimp](./Models/CteSimpSefazEndeEmiSimp.md)
 - [CteSimpSefazEnderFerSimp](./Models/CteSimpSefazEnderFerSimp.md)
 - [CteSimpSefazEnderecoSimp](./Models/CteSimpSefazEnderecoSimp.md)
 - [CteSimpSefazEstornoCredSimp](./Models/CteSimpSefazEstornoCredSimp.md)
 - [CteSimpSefazFatSimp](./Models/CteSimpSefazFatSimp.md)
 - [CteSimpSefazFerroEnvSimp](./Models/CteSimpSefazFerroEnvSimp.md)
 - [CteSimpSefazFerrovSimp](./Models/CteSimpSefazFerrovSimp.md)
 - [CteSimpSefazFluxoSimp](./Models/CteSimpSefazFluxoSimp.md)
 - [CteSimpSefazGCBSSimp](./Models/CteSimpSefazGCBSSimp.md)
 - [CteSimpSefazGIBSMunSimp](./Models/CteSimpSefazGIBSMunSimp.md)
 - [CteSimpSefazGIBSUFSimp](./Models/CteSimpSefazGIBSUFSimp.md)
 - [CteSimpSefazGPagAntecipadoSimp](./Models/CteSimpSefazGPagAntecipadoSimp.md)
 - [CteSimpSefazICMS00Simp](./Models/CteSimpSefazICMS00Simp.md)
 - [CteSimpSefazICMS20Simp](./Models/CteSimpSefazICMS20Simp.md)
 - [CteSimpSefazICMS45Simp](./Models/CteSimpSefazICMS45Simp.md)
 - [CteSimpSefazICMS60Simp](./Models/CteSimpSefazICMS60Simp.md)
 - [CteSimpSefazICMS90Simp](./Models/CteSimpSefazICMS90Simp.md)
 - [CteSimpSefazICMSOutraUFSimp](./Models/CteSimpSefazICMSOutraUFSimp.md)
 - [CteSimpSefazICMSSNSimp](./Models/CteSimpSefazICMSSNSimp.md)
 - [CteSimpSefazICMSUFFimSimp](./Models/CteSimpSefazICMSUFFimSimp.md)
 - [CteSimpSefazIdeSimp](./Models/CteSimpSefazIdeSimp.md)
 - [CteSimpSefazImpSimp](./Models/CteSimpSefazImpSimp.md)
 - [CteSimpSefazInfCTeSuplSimp](./Models/CteSimpSefazInfCTeSuplSimp.md)
 - [CteSimpSefazInfCargaSimp](./Models/CteSimpSefazInfCargaSimp.md)
 - [CteSimpSefazInfCteSimp](./Models/CteSimpSefazInfCteSimp.md)
 - [CteSimpSefazInfCteSubSimp](./Models/CteSimpSefazInfCteSubSimp.md)
 - [CteSimpSefazInfCte_ImpSimp](./Models/CteSimpSefazInfCte_ImpSimp.md)
 - [CteSimpSefazInfDocAntSimp](./Models/CteSimpSefazInfDocAntSimp.md)
 - [CteSimpSefazInfDocSimp](./Models/CteSimpSefazInfDocSimp.md)
 - [CteSimpSefazInfDoc_InfNFeSimp](./Models/CteSimpSefazInfDoc_InfNFeSimp.md)
 - [CteSimpSefazInfModalSimp](./Models/CteSimpSefazInfModalSimp.md)
 - [CteSimpSefazInfNFSimp](./Models/CteSimpSefazInfNFSimp.md)
 - [CteSimpSefazInfNFeSimp](./Models/CteSimpSefazInfNFeSimp.md)
 - [CteSimpSefazInfNFeTranspParcialSimp](./Models/CteSimpSefazInfNFeTranspParcialSimp.md)
 - [CteSimpSefazInfQSimp](./Models/CteSimpSefazInfQSimp.md)
 - [CteSimpSefazInfSegSimp](./Models/CteSimpSefazInfSegSimp.md)
 - [CteSimpSefazInfSolicNFFSimp](./Models/CteSimpSefazInfSolicNFFSimp.md)
 - [CteSimpSefazInfTotAPSimp](./Models/CteSimpSefazInfTotAPSimp.md)
 - [CteSimpSefazLacUnidCargaSimp](./Models/CteSimpSefazLacUnidCargaSimp.md)
 - [CteSimpSefazLacUnidTranspSimp](./Models/CteSimpSefazLacUnidTranspSimp.md)
 - [CteSimpSefazLacreSimp](./Models/CteSimpSefazLacreSimp.md)
 - [CteSimpSefazMultimodalSimp](./Models/CteSimpSefazMultimodalSimp.md)
 - [CteSimpSefazNatCargaSimp](./Models/CteSimpSefazNatCargaSimp.md)
 - [CteSimpSefazObsContSimp](./Models/CteSimpSefazObsContSimp.md)
 - [CteSimpSefazObsFiscoSimp](./Models/CteSimpSefazObsFiscoSimp.md)
 - [CteSimpSefazOccSimp](./Models/CteSimpSefazOccSimp.md)
 - [CteSimpSefazPagamentoRTCSimp](./Models/CteSimpSefazPagamentoRTCSimp.md)
 - [CteSimpSefazPassSimp](./Models/CteSimpSefazPassSimp.md)
 - [CteSimpSefazPeriSimp](./Models/CteSimpSefazPeriSimp.md)
 - [CteSimpSefazPgtoVincSimp](./Models/CteSimpSefazPgtoVincSimp.md)
 - [CteSimpSefazRedSimp](./Models/CteSimpSefazRedSimp.md)
 - [CteSimpSefazRespTecSimp](./Models/CteSimpSefazRespTecSimp.md)
 - [CteSimpSefazRodoSimp](./Models/CteSimpSefazRodoSimp.md)
 - [CteSimpSefazSegSimp](./Models/CteSimpSefazSegSimp.md)
 - [CteSimpSefazTarifaSimp](./Models/CteSimpSefazTarifaSimp.md)
 - [CteSimpSefazTomaSimp](./Models/CteSimpSefazTomaSimp.md)
 - [CteSimpSefazTotalSimp](./Models/CteSimpSefazTotalSimp.md)
 - [CteSimpSefazTrafMutSimp](./Models/CteSimpSefazTrafMutSimp.md)
 - [CteSimpSefazTribCTeSimp](./Models/CteSimpSefazTribCTeSimp.md)
 - [CteSimpSefazTribCompraGovSimp](./Models/CteSimpSefazTribCompraGovSimp.md)
 - [CteSimpSefazTribRegularSimp](./Models/CteSimpSefazTribRegularSimp.md)
 - [CteSimpSefazUnidCargaSimp](./Models/CteSimpSefazUnidCargaSimp.md)
 - [CteSimpSefazUnidadeTranspSimp](./Models/CteSimpSefazUnidadeTranspSimp.md)
 - [DPS](./Models/DPS.md)
 - [DcePedidoCancelamento](./Models/DcePedidoCancelamento.md)
 - [DcePedidoEmissao](./Models/DcePedidoEmissao.md)
 - [DceSefazAutXML](./Models/DceSefazAutXML.md)
 - [DceSefazDest](./Models/DceSefazDest.md)
 - [DceSefazDet](./Models/DceSefazDet.md)
 - [DceSefazECT](./Models/DceSefazECT.md)
 - [DceSefazEmit](./Models/DceSefazEmit.md)
 - [DceSefazEndeDest](./Models/DceSefazEndeDest.md)
 - [DceSefazEndeEmi](./Models/DceSefazEndeEmi.md)
 - [DceSefazFisco](./Models/DceSefazFisco.md)
 - [DceSefazIde](./Models/DceSefazIde.md)
 - [DceSefazInfAdic](./Models/DceSefazInfAdic.md)
 - [DceSefazInfDCe](./Models/DceSefazInfDCe.md)
 - [DceSefazInfDec](./Models/DceSefazInfDec.md)
 - [DceSefazInfSolicDCe](./Models/DceSefazInfSolicDCe.md)
 - [DceSefazMarketplace](./Models/DceSefazMarketplace.md)
 - [DceSefazObsECT](./Models/DceSefazObsECT.md)
 - [DceSefazObsEmit](./Models/DceSefazObsEmit.md)
 - [DceSefazObsFisco](./Models/DceSefazObsFisco.md)
 - [DceSefazObsMarketplace](./Models/DceSefazObsMarketplace.md)
 - [DceSefazProd](./Models/DceSefazProd.md)
 - [DceSefazTotal](./Models/DceSefazTotal.md)
 - [DceSefazTransp](./Models/DceSefazTransp.md)
 - [DceSefazTransportadora](./Models/DceSefazTransportadora.md)
 - [Dfe](./Models/Dfe.md)
 - [DfeAutorEvento](./Models/DfeAutorEvento.md)
 - [DfeAutorizacao](./Models/DfeAutorizacao.md)
 - [DfeCancelamento](./Models/DfeCancelamento.md)
 - [DfeCartaCorrecao](./Models/DfeCartaCorrecao.md)
 - [DfeContribuinteEndereco](./Models/DfeContribuinteEndereco.md)
 - [DfeContribuinteInfCad](./Models/DfeContribuinteInfCad.md)
 - [DfeContribuinteInfCons](./Models/DfeContribuinteInfCons.md)
 - [DfeDebug](./Models/DfeDebug.md)
 - [DfeEvento](./Models/DfeEvento.md)
 - [DfeEventoListagem](./Models/DfeEventoListagem.md)
 - [DfeInutilizacao](./Models/DfeInutilizacao.md)
 - [DfeListagem](./Models/DfeListagem.md)
 - [DfeLote](./Models/DfeLote.md)
 - [DfeLoteListagem](./Models/DfeLoteListagem.md)
 - [DfePedidoEnvioEmail](./Models/DfePedidoEnvioEmail.md)
 - [DfePedidoInutilizacao](./Models/DfePedidoInutilizacao.md)
 - [DfeRecibo](./Models/DfeRecibo.md)
 - [DfeRequisicaoDebug](./Models/DfeRequisicaoDebug.md)
 - [DfeSefazStatus](./Models/DfeSefazStatus.md)
 - [DfeSincronizacao](./Models/DfeSincronizacao.md)
 - [DistribuicaoNfe](./Models/DistribuicaoNfe.md)
 - [DistribuicaoNfeDocumento](./Models/DistribuicaoNfeDocumento.md)
 - [DistribuicaoNfeDocumentoListagem](./Models/DistribuicaoNfeDocumentoListagem.md)
 - [DistribuicaoNfeEvento](./Models/DistribuicaoNfeEvento.md)
 - [DistribuicaoNfeListagem](./Models/DistribuicaoNfeListagem.md)
 - [DistribuicaoNfeNota](./Models/DistribuicaoNfeNota.md)
 - [DistribuicaoNfeNotaListagem](./Models/DistribuicaoNfeNotaListagem.md)
 - [DistribuicaoNfePedido](./Models/DistribuicaoNfePedido.md)
 - [DistribuicaoNfePedidoManifestacao](./Models/DistribuicaoNfePedidoManifestacao.md)
 - [DocDedRed](./Models/DocDedRed.md)
 - [DocNFNFS](./Models/DocNFNFS.md)
 - [DocOutNFSe](./Models/DocOutNFSe.md)
 - [Email](./Models/Email.md)
 - [EmailAttachment](./Models/EmailAttachment.md)
 - [EmailEvent](./Models/EmailEvent.md)
 - [EmailListagem](./Models/EmailListagem.md)
 - [EmailResumo](./Models/EmailResumo.md)
 - [EmailStatusResponse](./Models/EmailStatusResponse.md)
 - [Empresa](./Models/Empresa.md)
 - [EmpresaCertificado](./Models/EmpresaCertificado.md)
 - [EmpresaCertificadoListagem](./Models/EmpresaCertificadoListagem.md)
 - [EmpresaConfigCte](./Models/EmpresaConfigCte.md)
 - [EmpresaConfigCteOs](./Models/EmpresaConfigCteOs.md)
 - [EmpresaConfigDce](./Models/EmpresaConfigDce.md)
 - [EmpresaConfigDistribuicaoNfe](./Models/EmpresaConfigDistribuicaoNfe.md)
 - [EmpresaConfigMdfe](./Models/EmpresaConfigMdfe.md)
 - [EmpresaConfigNfce](./Models/EmpresaConfigNfce.md)
 - [EmpresaConfigNfceSefaz](./Models/EmpresaConfigNfceSefaz.md)
 - [EmpresaConfigNfcom](./Models/EmpresaConfigNfcom.md)
 - [EmpresaConfigNfe](./Models/EmpresaConfigNfe.md)
 - [EmpresaConfigNfse](./Models/EmpresaConfigNfse.md)
 - [EmpresaConfigNfseRegTrib](./Models/EmpresaConfigNfseRegTrib.md)
 - [EmpresaConfigPrefeitura](./Models/EmpresaConfigPrefeitura.md)
 - [EmpresaConfigRps](./Models/EmpresaConfigRps.md)
 - [EmpresaEndereco](./Models/EmpresaEndereco.md)
 - [EmpresaListagem](./Models/EmpresaListagem.md)
 - [EmpresaPedidoCadastroCertificado](./Models/EmpresaPedidoCadastroCertificado.md)
 - [EnderExt](./Models/EnderExt.md)
 - [EnderExtSimples](./Models/EnderExtSimples.md)
 - [EnderNac](./Models/EnderNac.md)
 - [EnderObraEvento](./Models/EnderObraEvento.md)
 - [Endereco](./Models/Endereco.md)
 - [EnderecoEmail](./Models/EnderecoEmail.md)
 - [EnderecoSimples](./Models/EnderecoSimples.md)
 - [ExigSuspensa](./Models/ExigSuspensa.md)
 - [HttpRequestDebug](./Models/HttpRequestDebug.md)
 - [InfDPS](./Models/InfDPS.md)
 - [InfoCompl](./Models/InfoCompl.md)
 - [InfoDedRed](./Models/InfoDedRed.md)
 - [InfoFornecDocDedRed](./Models/InfoFornecDocDedRed.md)
 - [InfoIntermediario](./Models/InfoIntermediario.md)
 - [InfoItemPed](./Models/InfoItemPed.md)
 - [InfoObra](./Models/InfoObra.md)
 - [InfoPrestador](./Models/InfoPrestador.md)
 - [InfoRefNFSe](./Models/InfoRefNFSe.md)
 - [InfoTomador](./Models/InfoTomador.md)
 - [InfoTributacao](./Models/InfoTributacao.md)
 - [InfoValores](./Models/InfoValores.md)
 - [ListaDocDedRed](./Models/ListaDocDedRed.md)
 - [LocPrest](./Models/LocPrest.md)
 - [ManifestacaoNfeListagem](./Models/ManifestacaoNfeListagem.md)
 - [MdfeDocumentoVinculado](./Models/MdfeDocumentoVinculado.md)
 - [MdfeEncerramento](./Models/MdfeEncerramento.md)
 - [MdfeInclusaoCondutor](./Models/MdfeInclusaoCondutor.md)
 - [MdfeInclusaoDfe](./Models/MdfeInclusaoDfe.md)
 - [MdfeNaoEncerrado](./Models/MdfeNaoEncerrado.md)
 - [MdfeNaoEncerrados](./Models/MdfeNaoEncerrados.md)
 - [MdfePedidoCancelamento](./Models/MdfePedidoCancelamento.md)
 - [MdfePedidoEmissao](./Models/MdfePedidoEmissao.md)
 - [MdfePedidoEmissaoLote](./Models/MdfePedidoEmissaoLote.md)
 - [MdfePedidoEncerramento](./Models/MdfePedidoEncerramento.md)
 - [MdfePedidoInclusaoCondutor](./Models/MdfePedidoInclusaoCondutor.md)
 - [MdfePedidoInclusaoDfe](./Models/MdfePedidoInclusaoDfe.md)
 - [MdfeSefazAereo](./Models/MdfeSefazAereo.md)
 - [MdfeSefazAquav](./Models/MdfeSefazAquav.md)
 - [MdfeSefazAutXML](./Models/MdfeSefazAutXML.md)
 - [MdfeSefazComp](./Models/MdfeSefazComp.md)
 - [MdfeSefazCondutor](./Models/MdfeSefazCondutor.md)
 - [MdfeSefazDisp](./Models/MdfeSefazDisp.md)
 - [MdfeSefazEmit](./Models/MdfeSefazEmit.md)
 - [MdfeSefazEndeEmi](./Models/MdfeSefazEndeEmi.md)
 - [MdfeSefazFerrov](./Models/MdfeSefazFerrov.md)
 - [MdfeSefazIde](./Models/MdfeSefazIde.md)
 - [MdfeSefazInfANTT](./Models/MdfeSefazInfANTT.md)
 - [MdfeSefazInfAdic](./Models/MdfeSefazInfAdic.md)
 - [MdfeSefazInfBanc](./Models/MdfeSefazInfBanc.md)
 - [MdfeSefazInfCIOT](./Models/MdfeSefazInfCIOT.md)
 - [MdfeSefazInfCTe](./Models/MdfeSefazInfCTe.md)
 - [MdfeSefazInfContratante](./Models/MdfeSefazInfContratante.md)
 - [MdfeSefazInfContrato](./Models/MdfeSefazInfContrato.md)
 - [MdfeSefazInfDoc](./Models/MdfeSefazInfDoc.md)
 - [MdfeSefazInfEmbComb](./Models/MdfeSefazInfEmbComb.md)
 - [MdfeSefazInfEntregaParcial](./Models/MdfeSefazInfEntregaParcial.md)
 - [MdfeSefazInfLocalCarrega](./Models/MdfeSefazInfLocalCarrega.md)
 - [MdfeSefazInfLocalDescarrega](./Models/MdfeSefazInfLocalDescarrega.md)
 - [MdfeSefazInfLotacao](./Models/MdfeSefazInfLotacao.md)
 - [MdfeSefazInfMDFe](./Models/MdfeSefazInfMDFe.md)
 - [MdfeSefazInfMDFeSupl](./Models/MdfeSefazInfMDFeSupl.md)
 - [MdfeSefazInfMDFeTransp](./Models/MdfeSefazInfMDFeTransp.md)
 - [MdfeSefazInfMDFeTransp_Peri](./Models/MdfeSefazInfMDFeTransp_Peri.md)
 - [MdfeSefazInfModal](./Models/MdfeSefazInfModal.md)
 - [MdfeSefazInfMunCarrega](./Models/MdfeSefazInfMunCarrega.md)
 - [MdfeSefazInfMunDescarga](./Models/MdfeSefazInfMunDescarga.md)
 - [MdfeSefazInfNFe](./Models/MdfeSefazInfNFe.md)
 - [MdfeSefazInfNFePrestParcial](./Models/MdfeSefazInfNFePrestParcial.md)
 - [MdfeSefazInfNFe_Peri](./Models/MdfeSefazInfNFe_Peri.md)
 - [MdfeSefazInfPag](./Models/MdfeSefazInfPag.md)
 - [MdfeSefazInfPercurso](./Models/MdfeSefazInfPercurso.md)
 - [MdfeSefazInfPrazo](./Models/MdfeSefazInfPrazo.md)
 - [MdfeSefazInfResp](./Models/MdfeSefazInfResp.md)
 - [MdfeSefazInfSeg](./Models/MdfeSefazInfSeg.md)
 - [MdfeSefazInfSolicNFF](./Models/MdfeSefazInfSolicNFF.md)
 - [MdfeSefazInfTermCarreg](./Models/MdfeSefazInfTermCarreg.md)
 - [MdfeSefazInfTermDescarreg](./Models/MdfeSefazInfTermDescarreg.md)
 - [MdfeSefazInfUnidCargaVazia](./Models/MdfeSefazInfUnidCargaVazia.md)
 - [MdfeSefazInfUnidTranspVazia](./Models/MdfeSefazInfUnidTranspVazia.md)
 - [MdfeSefazLacRodo](./Models/MdfeSefazLacRodo.md)
 - [MdfeSefazLacUnidCarga](./Models/MdfeSefazLacUnidCarga.md)
 - [MdfeSefazLacUnidTransp](./Models/MdfeSefazLacUnidTransp.md)
 - [MdfeSefazLacres](./Models/MdfeSefazLacres.md)
 - [MdfeSefazPeri](./Models/MdfeSefazPeri.md)
 - [MdfeSefazProdPred](./Models/MdfeSefazProdPred.md)
 - [MdfeSefazProp](./Models/MdfeSefazProp.md)
 - [MdfeSefazRespTec](./Models/MdfeSefazRespTec.md)
 - [MdfeSefazRodo](./Models/MdfeSefazRodo.md)
 - [MdfeSefazSeg](./Models/MdfeSefazSeg.md)
 - [MdfeSefazTot](./Models/MdfeSefazTot.md)
 - [MdfeSefazTrem](./Models/MdfeSefazTrem.md)
 - [MdfeSefazUnidCarga](./Models/MdfeSefazUnidCarga.md)
 - [MdfeSefazUnidadeTransp](./Models/MdfeSefazUnidadeTransp.md)
 - [MdfeSefazVag](./Models/MdfeSefazVag.md)
 - [MdfeSefazValePed](./Models/MdfeSefazValePed.md)
 - [MdfeSefazVeicReboque](./Models/MdfeSefazVeicReboque.md)
 - [MdfeSefazVeicReboque_Prop](./Models/MdfeSefazVeicReboque_Prop.md)
 - [MdfeSefazVeicTracao](./Models/MdfeSefazVeicTracao.md)
 - [NfcomPedidoCancelamento](./Models/NfcomPedidoCancelamento.md)
 - [NfcomPedidoEmissao](./Models/NfcomPedidoEmissao.md)
 - [NfcomSefazALCZFMCBS](./Models/NfcomSefazALCZFMCBS.md)
 - [NfcomSefazAssinante](./Models/NfcomSefazAssinante.md)
 - [NfcomSefazAutXML](./Models/NfcomSefazAutXML.md)
 - [NfcomSefazCIBS](./Models/NfcomSefazCIBS.md)
 - [NfcomSefazCOFINS](./Models/NfcomSefazCOFINS.md)
 - [NfcomSefazCompraGovReduzido](./Models/NfcomSefazCompraGovReduzido.md)
 - [NfcomSefazDest](./Models/NfcomSefazDest.md)
 - [NfcomSefazDet](./Models/NfcomSefazDet.md)
 - [NfcomSefazDevTrib](./Models/NfcomSefazDevTrib.md)
 - [NfcomSefazDif](./Models/NfcomSefazDif.md)
 - [NfcomSefazEmit](./Models/NfcomSefazEmit.md)
 - [NfcomSefazEndeDest](./Models/NfcomSefazEndeDest.md)
 - [NfcomSefazEndeEmi](./Models/NfcomSefazEndeEmi.md)
 - [NfcomSefazEstornoCred](./Models/NfcomSefazEstornoCred.md)
 - [NfcomSefazFUNTTEL](./Models/NfcomSefazFUNTTEL.md)
 - [NfcomSefazFUST](./Models/NfcomSefazFUST.md)
 - [NfcomSefazGCBS](./Models/NfcomSefazGCBS.md)
 - [NfcomSefazGCofat](./Models/NfcomSefazGCofat.md)
 - [NfcomSefazGCofat_GNF](./Models/NfcomSefazGCofat_GNF.md)
 - [NfcomSefazGEstornoCred](./Models/NfcomSefazGEstornoCred.md)
 - [NfcomSefazGFat](./Models/NfcomSefazGFat.md)
 - [NfcomSefazGFatCentral](./Models/NfcomSefazGFatCentral.md)
 - [NfcomSefazGFidelidade](./Models/NfcomSefazGFidelidade.md)
 - [NfcomSefazGIBS](./Models/NfcomSefazGIBS.md)
 - [NfcomSefazGIBSMun](./Models/NfcomSefazGIBSMun.md)
 - [NfcomSefazGIBSUF](./Models/NfcomSefazGIBSUF.md)
 - [NfcomSefazGIBS_GIBSMun](./Models/NfcomSefazGIBS_GIBSMun.md)
 - [NfcomSefazGIBS_GIBSUF](./Models/NfcomSefazGIBS_GIBSUF.md)
 - [NfcomSefazGNF](./Models/NfcomSefazGNF.md)
 - [NfcomSefazGPIX](./Models/NfcomSefazGPIX.md)
 - [NfcomSefazGPagAntecipado](./Models/NfcomSefazGPagAntecipado.md)
 - [NfcomSefazGProc](./Models/NfcomSefazGProc.md)
 - [NfcomSefazGProcRef](./Models/NfcomSefazGProcRef.md)
 - [NfcomSefazGRessarc](./Models/NfcomSefazGRessarc.md)
 - [NfcomSefazGSub](./Models/NfcomSefazGSub.md)
 - [NfcomSefazIBSCBSTot](./Models/NfcomSefazIBSCBSTot.md)
 - [NfcomSefazIBSCBSTot_GCBS](./Models/NfcomSefazIBSCBSTot_GCBS.md)
 - [NfcomSefazICMS00](./Models/NfcomSefazICMS00.md)
 - [NfcomSefazICMS20](./Models/NfcomSefazICMS20.md)
 - [NfcomSefazICMS40](./Models/NfcomSefazICMS40.md)
 - [NfcomSefazICMS51](./Models/NfcomSefazICMS51.md)
 - [NfcomSefazICMS90](./Models/NfcomSefazICMS90.md)
 - [NfcomSefazICMSSN](./Models/NfcomSefazICMSSN.md)
 - [NfcomSefazICMSTot](./Models/NfcomSefazICMSTot.md)
 - [NfcomSefazICMSUFDest](./Models/NfcomSefazICMSUFDest.md)
 - [NfcomSefazIde](./Models/NfcomSefazIde.md)
 - [NfcomSefazImposto](./Models/NfcomSefazImposto.md)
 - [NfcomSefazInfAdic](./Models/NfcomSefazInfAdic.md)
 - [NfcomSefazInfNFCom](./Models/NfcomSefazInfNFCom.md)
 - [NfcomSefazPIS](./Models/NfcomSefazPIS.md)
 - [NfcomSefazPagamentoRTC](./Models/NfcomSefazPagamentoRTC.md)
 - [NfcomSefazPgtoVinc](./Models/NfcomSefazPgtoVinc.md)
 - [NfcomSefazProd](./Models/NfcomSefazProd.md)
 - [NfcomSefazRed](./Models/NfcomSefazRed.md)
 - [NfcomSefazRespTec](./Models/NfcomSefazRespTec.md)
 - [NfcomSefazRetTrib](./Models/NfcomSefazRetTrib.md)
 - [NfcomSefazTotal](./Models/NfcomSefazTotal.md)
 - [NfcomSefazTribCompraGov](./Models/NfcomSefazTribCompraGov.md)
 - [NfcomSefazTribNFCom](./Models/NfcomSefazTribNFCom.md)
 - [NfcomSefazTribRegular](./Models/NfcomSefazTribRegular.md)
 - [NfcomSefazVRetTribTot](./Models/NfcomSefazVRetTribTot.md)
 - [NfePedidoCancelamento](./Models/NfePedidoCancelamento.md)
 - [NfePedidoCartaCorrecao](./Models/NfePedidoCartaCorrecao.md)
 - [NfePedidoEmissao](./Models/NfePedidoEmissao.md)
 - [NfePedidoEmissaoLote](./Models/NfePedidoEmissaoLote.md)
 - [NfeSefazAdi](./Models/NfeSefazAdi.md)
 - [NfeSefazAgropecuario](./Models/NfeSefazAgropecuario.md)
 - [NfeSefazAjusteCompet](./Models/NfeSefazAjusteCompet.md)
 - [NfeSefazArma](./Models/NfeSefazArma.md)
 - [NfeSefazAutXML](./Models/NfeSefazAutXML.md)
 - [NfeSefazAvulsa](./Models/NfeSefazAvulsa.md)
 - [NfeSefazCIBS](./Models/NfeSefazCIBS.md)
 - [NfeSefazCIDE](./Models/NfeSefazCIDE.md)
 - [NfeSefazCOFINS](./Models/NfeSefazCOFINS.md)
 - [NfeSefazCOFINSAliq](./Models/NfeSefazCOFINSAliq.md)
 - [NfeSefazCOFINSNT](./Models/NfeSefazCOFINSNT.md)
 - [NfeSefazCOFINSOutr](./Models/NfeSefazCOFINSOutr.md)
 - [NfeSefazCOFINSQtde](./Models/NfeSefazCOFINSQtde.md)
 - [NfeSefazCOFINSST](./Models/NfeSefazCOFINSST.md)
 - [NfeSefazCana](./Models/NfeSefazCana.md)
 - [NfeSefazCard](./Models/NfeSefazCard.md)
 - [NfeSefazCobr](./Models/NfeSefazCobr.md)
 - [NfeSefazComb](./Models/NfeSefazComb.md)
 - [NfeSefazCompra](./Models/NfeSefazCompra.md)
 - [NfeSefazCompraGov](./Models/NfeSefazCompraGov.md)
 - [NfeSefazCredPres](./Models/NfeSefazCredPres.md)
 - [NfeSefazCredPresIBSZFM](./Models/NfeSefazCredPresIBSZFM.md)
 - [NfeSefazCredPresOper](./Models/NfeSefazCredPresOper.md)
 - [NfeSefazDFeReferenciado](./Models/NfeSefazDFeReferenciado.md)
 - [NfeSefazDI](./Models/NfeSefazDI.md)
 - [NfeSefazDeduc](./Models/NfeSefazDeduc.md)
 - [NfeSefazDefensivo](./Models/NfeSefazDefensivo.md)
 - [NfeSefazDest](./Models/NfeSefazDest.md)
 - [NfeSefazDet](./Models/NfeSefazDet.md)
 - [NfeSefazDetExport](./Models/NfeSefazDetExport.md)
 - [NfeSefazDetPag](./Models/NfeSefazDetPag.md)
 - [NfeSefazDevTrib](./Models/NfeSefazDevTrib.md)
 - [NfeSefazDif](./Models/NfeSefazDif.md)
 - [NfeSefazDup](./Models/NfeSefazDup.md)
 - [NfeSefazEmit](./Models/NfeSefazEmit.md)
 - [NfeSefazEncerrante](./Models/NfeSefazEncerrante.md)
 - [NfeSefazEnderEmi](./Models/NfeSefazEnderEmi.md)
 - [NfeSefazEndereco](./Models/NfeSefazEndereco.md)
 - [NfeSefazEstornoCred](./Models/NfeSefazEstornoCred.md)
 - [NfeSefazExportInd](./Models/NfeSefazExportInd.md)
 - [NfeSefazExporta](./Models/NfeSefazExporta.md)
 - [NfeSefazFat](./Models/NfeSefazFat.md)
 - [NfeSefazForDia](./Models/NfeSefazForDia.md)
 - [NfeSefazGCBS](./Models/NfeSefazGCBS.md)
 - [NfeSefazGCred](./Models/NfeSefazGCred.md)
 - [NfeSefazGEstornoCred](./Models/NfeSefazGEstornoCred.md)
 - [NfeSefazGIBS](./Models/NfeSefazGIBS.md)
 - [NfeSefazGIBSMun](./Models/NfeSefazGIBSMun.md)
 - [NfeSefazGIBSUF](./Models/NfeSefazGIBSUF.md)
 - [NfeSefazGIBS_GIBSMun](./Models/NfeSefazGIBS_GIBSMun.md)
 - [NfeSefazGIBS_GIBSUF](./Models/NfeSefazGIBS_GIBSUF.md)
 - [NfeSefazGMono](./Models/NfeSefazGMono.md)
 - [NfeSefazGMonoDif](./Models/NfeSefazGMonoDif.md)
 - [NfeSefazGMonoPadrao](./Models/NfeSefazGMonoPadrao.md)
 - [NfeSefazGMonoRet](./Models/NfeSefazGMonoRet.md)
 - [NfeSefazGMonoReten](./Models/NfeSefazGMonoReten.md)
 - [NfeSefazGPagAntecipado](./Models/NfeSefazGPagAntecipado.md)
 - [NfeSefazGuiaTransito](./Models/NfeSefazGuiaTransito.md)
 - [NfeSefazIBSCBSMonoTot](./Models/NfeSefazIBSCBSMonoTot.md)
 - [NfeSefazIBSCBSMonoTot_GCBS](./Models/NfeSefazIBSCBSMonoTot_GCBS.md)
 - [NfeSefazICMS](./Models/NfeSefazICMS.md)
 - [NfeSefazICMS00](./Models/NfeSefazICMS00.md)
 - [NfeSefazICMS02](./Models/NfeSefazICMS02.md)
 - [NfeSefazICMS10](./Models/NfeSefazICMS10.md)
 - [NfeSefazICMS15](./Models/NfeSefazICMS15.md)
 - [NfeSefazICMS20](./Models/NfeSefazICMS20.md)
 - [NfeSefazICMS30](./Models/NfeSefazICMS30.md)
 - [NfeSefazICMS40](./Models/NfeSefazICMS40.md)
 - [NfeSefazICMS51](./Models/NfeSefazICMS51.md)
 - [NfeSefazICMS53](./Models/NfeSefazICMS53.md)
 - [NfeSefazICMS60](./Models/NfeSefazICMS60.md)
 - [NfeSefazICMS61](./Models/NfeSefazICMS61.md)
 - [NfeSefazICMS70](./Models/NfeSefazICMS70.md)
 - [NfeSefazICMS90](./Models/NfeSefazICMS90.md)
 - [NfeSefazICMSPart](./Models/NfeSefazICMSPart.md)
 - [NfeSefazICMSSN101](./Models/NfeSefazICMSSN101.md)
 - [NfeSefazICMSSN102](./Models/NfeSefazICMSSN102.md)
 - [NfeSefazICMSSN201](./Models/NfeSefazICMSSN201.md)
 - [NfeSefazICMSSN202](./Models/NfeSefazICMSSN202.md)
 - [NfeSefazICMSSN500](./Models/NfeSefazICMSSN500.md)
 - [NfeSefazICMSSN900](./Models/NfeSefazICMSSN900.md)
 - [NfeSefazICMSST](./Models/NfeSefazICMSST.md)
 - [NfeSefazICMSTot](./Models/NfeSefazICMSTot.md)
 - [NfeSefazICMSUFDest](./Models/NfeSefazICMSUFDest.md)
 - [NfeSefazII](./Models/NfeSefazII.md)
 - [NfeSefazIPINT](./Models/NfeSefazIPINT.md)
 - [NfeSefazIPITrib](./Models/NfeSefazIPITrib.md)
 - [NfeSefazIS](./Models/NfeSefazIS.md)
 - [NfeSefazISSQN](./Models/NfeSefazISSQN.md)
 - [NfeSefazISSQNtot](./Models/NfeSefazISSQNtot.md)
 - [NfeSefazISTot](./Models/NfeSefazISTot.md)
 - [NfeSefazIde](./Models/NfeSefazIde.md)
 - [NfeSefazImposto](./Models/NfeSefazImposto.md)
 - [NfeSefazImpostoDevol](./Models/NfeSefazImpostoDevol.md)
 - [NfeSefazImpostoDevol_IPI](./Models/NfeSefazImpostoDevol_IPI.md)
 - [NfeSefazInfAdic](./Models/NfeSefazInfAdic.md)
 - [NfeSefazInfAdic_ObsCont](./Models/NfeSefazInfAdic_ObsCont.md)
 - [NfeSefazInfAdic_ObsFisco](./Models/NfeSefazInfAdic_ObsFisco.md)
 - [NfeSefazInfIntermed](./Models/NfeSefazInfIntermed.md)
 - [NfeSefazInfNFe](./Models/NfeSefazInfNFe.md)
 - [NfeSefazInfNFeSupl](./Models/NfeSefazInfNFeSupl.md)
 - [NfeSefazInfPAA](./Models/NfeSefazInfPAA.md)
 - [NfeSefazInfProdEmb](./Models/NfeSefazInfProdEmb.md)
 - [NfeSefazInfProdNFF](./Models/NfeSefazInfProdNFF.md)
 - [NfeSefazInfRespTec](./Models/NfeSefazInfRespTec.md)
 - [NfeSefazInfSolicNFF](./Models/NfeSefazInfSolicNFF.md)
 - [NfeSefazIpi](./Models/NfeSefazIpi.md)
 - [NfeSefazLacres](./Models/NfeSefazLacres.md)
 - [NfeSefazLocal](./Models/NfeSefazLocal.md)
 - [NfeSefazMed](./Models/NfeSefazMed.md)
 - [NfeSefazMonofasia](./Models/NfeSefazMonofasia.md)
 - [NfeSefazNFref](./Models/NfeSefazNFref.md)
 - [NfeSefazObsCont](./Models/NfeSefazObsCont.md)
 - [NfeSefazObsFisco](./Models/NfeSefazObsFisco.md)
 - [NfeSefazObsItem](./Models/NfeSefazObsItem.md)
 - [NfeSefazOrigComb](./Models/NfeSefazOrigComb.md)
 - [NfeSefazPAASignature](./Models/NfeSefazPAASignature.md)
 - [NfeSefazPIS](./Models/NfeSefazPIS.md)
 - [NfeSefazPISAliq](./Models/NfeSefazPISAliq.md)
 - [NfeSefazPISNT](./Models/NfeSefazPISNT.md)
 - [NfeSefazPISOutr](./Models/NfeSefazPISOutr.md)
 - [NfeSefazPISQtde](./Models/NfeSefazPISQtde.md)
 - [NfeSefazPISST](./Models/NfeSefazPISST.md)
 - [NfeSefazPag](./Models/NfeSefazPag.md)
 - [NfeSefazProcRef](./Models/NfeSefazProcRef.md)
 - [NfeSefazProd](./Models/NfeSefazProd.md)
 - [NfeSefazRSAKeyValueType](./Models/NfeSefazRSAKeyValueType.md)
 - [NfeSefazRastro](./Models/NfeSefazRastro.md)
 - [NfeSefazRed](./Models/NfeSefazRed.md)
 - [NfeSefazRefECF](./Models/NfeSefazRefECF.md)
 - [NfeSefazRefNF](./Models/NfeSefazRefNF.md)
 - [NfeSefazRefNFP](./Models/NfeSefazRefNFP.md)
 - [NfeSefazRetTransp](./Models/NfeSefazRetTransp.md)
 - [NfeSefazRetTrib](./Models/NfeSefazRetTrib.md)
 - [NfeSefazTotal](./Models/NfeSefazTotal.md)
 - [NfeSefazTransfCred](./Models/NfeSefazTransfCred.md)
 - [NfeSefazTransp](./Models/NfeSefazTransp.md)
 - [NfeSefazTransporta](./Models/NfeSefazTransporta.md)
 - [NfeSefazTribCompraGov](./Models/NfeSefazTribCompraGov.md)
 - [NfeSefazTribNFe](./Models/NfeSefazTribNFe.md)
 - [NfeSefazTribRegular](./Models/NfeSefazTribRegular.md)
 - [NfeSefazVeicProd](./Models/NfeSefazVeicProd.md)
 - [NfeSefazVeiculo](./Models/NfeSefazVeiculo.md)
 - [NfeSefazVol](./Models/NfeSefazVol.md)
 - [Nfse](./Models/Nfse.md)
 - [NfseCancelamento](./Models/NfseCancelamento.md)
 - [NfseCidadeMetadados](./Models/NfseCidadeMetadados.md)
 - [NfseCidadesAtendidas](./Models/NfseCidadesAtendidas.md)
 - [NfseDpsPedidoEmissao](./Models/NfseDpsPedidoEmissao.md)
 - [NfseListagem](./Models/NfseListagem.md)
 - [NfseLoteDpsPedidoEmissao](./Models/NfseLoteDpsPedidoEmissao.md)
 - [NfseMensagemRetorno](./Models/NfseMensagemRetorno.md)
 - [NfsePedidoCancelamento](./Models/NfsePedidoCancelamento.md)
 - [NfsePedidoEmissao](./Models/NfsePedidoEmissao.md)
 - [NfsePedidoSincronizacao](./Models/NfsePedidoSincronizacao.md)
 - [NfseSincronizacao](./Models/NfseSincronizacao.md)
 - [RTCInfoDest](./Models/RTCInfoDest.md)
 - [RTCInfoIBSCBS](./Models/RTCInfoIBSCBS.md)
 - [RTCInfoImovel](./Models/RTCInfoImovel.md)
 - [RTCInfoReeRepRes](./Models/RTCInfoReeRepRes.md)
 - [RTCInfoTributosDif](./Models/RTCInfoTributosDif.md)
 - [RTCInfoTributosIBSCBS](./Models/RTCInfoTributosIBSCBS.md)
 - [RTCInfoTributosSitClas](./Models/RTCInfoTributosSitClas.md)
 - [RTCInfoTributosTribRegular](./Models/RTCInfoTributosTribRegular.md)
 - [RTCInfoValoresIBSCBS](./Models/RTCInfoValoresIBSCBS.md)
 - [RTCListaDoc](./Models/RTCListaDoc.md)
 - [RTCListaDocDFe](./Models/RTCListaDocDFe.md)
 - [RTCListaDocFiscalOutro](./Models/RTCListaDocFiscalOutro.md)
 - [RTCListaDocFornec](./Models/RTCListaDocFornec.md)
 - [RTCListaDocOutro](./Models/RTCListaDocOutro.md)
 - [RegTrib](./Models/RegTrib.md)
 - [Rps](./Models/Rps.md)
 - [RpsDados](./Models/RpsDados.md)
 - [RpsDadosConstrucaoCivil](./Models/RpsDadosConstrucaoCivil.md)
 - [RpsDadosIntermediario](./Models/RpsDadosIntermediario.md)
 - [RpsDadosPrestador](./Models/RpsDadosPrestador.md)
 - [RpsDadosServico](./Models/RpsDadosServico.md)
 - [RpsDadosTomador](./Models/RpsDadosTomador.md)
 - [RpsDadosTomadorEndereco](./Models/RpsDadosTomadorEndereco.md)
 - [RpsIdentificacao](./Models/RpsIdentificacao.md)
 - [RpsIdentificacaoPrestador](./Models/RpsIdentificacaoPrestador.md)
 - [RpsLote](./Models/RpsLote.md)
 - [RpsLoteListagem](./Models/RpsLoteListagem.md)
 - [RpsPedidoEmissao](./Models/RpsPedidoEmissao.md)
 - [RpsPedidoEmissaoLote](./Models/RpsPedidoEmissaoLote.md)
 - [RpsServicoValores](./Models/RpsServicoValores.md)
 - [Serv](./Models/Serv.md)
 - [Substituicao](./Models/Substituicao.md)
 - [TribFederal](./Models/TribFederal.md)
 - [TribMunicipal](./Models/TribMunicipal.md)
 - [TribOutrosPisCofins](./Models/TribOutrosPisCofins.md)
 - [TribTotal](./Models/TribTotal.md)
 - [TribTotalMonet](./Models/TribTotalMonet.md)
 - [TribTotalPercent](./Models/TribTotalPercent.md)
 - [VDescCondIncond](./Models/VDescCondIncond.md)
 - [VServPrest](./Models/VServPrest.md)


<a name="documentation-for-authorization"></a>
## Documentação de autorização

<a name="oauth2"></a>
### oauth2

- **Tipo**: OAuth
- **Fluxo**: application
- **URL de autorização**: 
- **Escopos**: 
  - conta: 
  - empresa: 
  - cep: 
  - cnpj: 
  - mdfe: 
  - cte: 
  - nfse: 
  - nfe: 

