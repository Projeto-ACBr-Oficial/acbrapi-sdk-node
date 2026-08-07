# NfeSefazIde

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **cUF** | **number** | Código da UF do emitente do Documento Fiscal. Utilizar a Tabela do IBGE. |  |
| **cNF** | **string** | Código numérico que compõe a Chave de Acesso. Número aleatório gerado pelo emitente para cada NF-e.    *Geramos automaticamente quando nenhum valor é informado.* | [opcional]  |
| **natOp** | **string** | Descrição da Natureza da Operação. |  |
| **mod** | **number** | Código do modelo do Documento Fiscal:  * 55 - NF-e  * 65 - NFC-e | [opcional]  |
| **serie** | **number** | Série do Documento Fiscal:  * Série normal 0-889  * Avulsa Fisco 890-899  * SCAN 900-999 |  |
| **nNF** | **number** | Número do Documento Fiscal. |  |
| **dhEmi** | **Date** | Data e Hora de emissão do Documento Fiscal (AAAA-MM-DDThh:mm:ssTZD) ex.: 2012-09-01T13:00:00-03:00. |  |
| **dhSaiEnt** | **Date** | Data e Hora da saída ou de entrada da mercadoria / produto (AAAA-MM-DDTHH:mm:ssTZD). | [opcional]  |
| **dPrevEntrega** | **Date** | Data da previsão de entrega ou disponibilização do bem (AAAA-MM-DD). | [opcional]  |
| **tpNF** | **number** | Tipo do Documento Fiscal:  * 0 - Entrada  * 1 - Saída |  |
| **idDest** | **number** | Identificador de Local de destino da operação:  * 1 - Interna  * 2 - Interestadual  * 3 - Exterior |  |
| **cMunFG** | **string** | Código do Município de Ocorrência do Fato Gerador (utilizar a tabela do IBGE). |  |
| **cMunFGIBS** | **string** | Informar o município de ocorrência do fato gerador do fato gerador do IBS / CBS.  Campo preenchido somente quando “indPres &#x3D; 5 (Operação presencial, fora do estabelecimento) ”, e não tiver endereço do destinatário (Grupo: E05) ou local de entrega (Grupo: G01). | [opcional]  |
| **tpImp** | **number** | Formato de impressão do DANFE:  * 0 - Sem DANFE  * 1 - DANFe Retrato  * 2 - DANFe Paisagem  * 3 - DANFe Simplificado  * 4 - DANFe NFC-e  * 5 - DANFe NFC-e em mensagem eletrônica |  |
| **tpEmis** | **number** | Forma de emissão da NF-e  * 1 - Normal  * 2 - Contingência FS  * 3 - Regime Especial NFF (NT 2021.002)  * 4 - Contingência DPEC  * 5 - Contingência FSDA  * 6 - Contingência SVC - AN  * 7 - Contingência SVC - RS  * 9 - Contingência off-line NFC-e |  |
| **cDV** | **number** | Digito Verificador da Chave de Acesso da NF-e.    *Geramos automaticamente quando nenhum valor é informado.* | [opcional]  |
| **tpAmb** | **number** | Identificação do Ambiente:  * 1 - Produção  * 2 - Homologação | [opcional]  |
| **finNFe** | **number** | Finalidade da emissão da NF-e:  * 1 - NFe normal  * 2 - NFe complementar  * 3 - NFe de ajuste  * 4 - Devolução/Retorno  * 5 - Nota de crédito  * 6 - Nota de débito |  |
| **tpNFDebito** | **string** | Tipo de Nota de Débito:  * 01 - Transferência de créditos para Cooperativas  * 02 - Anulação de Crédito por Saídas Imunes/Isentas  * 03 - Débitos de notas fiscais não processadas na apuração  * 04 - Multa e juros  * 05 - Transferência de crédito de sucessão | [opcional]  |
| **tpNFCredito** | **string** | Tipo de Nota de Crédito. | [opcional]  |
| **indFinal** | **number** | Indica operação com consumidor final:  * 0 - Não  * 1 - Consumidor Final |  |
| **indPres** | **number** | Indicador de presença do comprador no estabelecimento comercial no momento da operação:  * 0 - Não se aplica (ex.: Nota Fiscal complementar ou de ajuste)  * 1 - Operação presencial  * 2 - Não presencial, internet  * 3 - Não presencial, teleatendimento  * 4 - NFC-e entrega em domicílio  * 5 - Operação presencial, fora do estabelecimento  * 9 - Não presencial, outros |  |
| **indIntermed** | **number** | Indicador de intermediador/marketplace  * 0 - Operação sem intermediador (em site ou plataforma própria)  * 1 - Operação em site ou plataforma de terceiros (intermediadores/marketplace) | [opcional]  |
| **procEmi** | **number** | Processo de emissão utilizado com a seguinte codificação:  * 0 - emissão de NF-e com aplicativo do contribuinte  * 1 - emissão de NF-e avulsa pelo Fisco  * 2 - emissão de NF-e avulsa, pelo contribuinte com seu certificado digital, através do site  do Fisco  * 3 - emissão de NF-e pelo contribuinte com aplicativo fornecido pelo Fisco  * 4 - emissão de NF-e por Provedor de Assinatura e Autorização - PAA |  |
| **verProc** | **string** | versão do aplicativo utilizado no processo de  emissão. |  |
| **dhCont** | **Date** | Informar a data e hora de entrada em contingência contingência no formato  (AAAA-MM-DDThh:mm:ssTZD) ex.: 2012-09-01T13:00:00-03:00. | [opcional]  |
| **xJust** | **string** | Informar a Justificativa da entrada. | [opcional]  |
| **NFref** | [**Array**](NfeSefazNFref.md) |  | [opcional]  |
| **gCompraGov** | [**NfeSefazCompraGov**](NfeSefazCompraGov.md) |  | [opcional]  |
| **gPagAntecipado** | [**NfeSefazGPagAntecipado**](NfeSefazGPagAntecipado.md) |  | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

