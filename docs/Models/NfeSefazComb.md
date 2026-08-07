# NfeSefazComb

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **cProdANP** | **number** | Código de produto da ANP. codificação de produtos do SIMP (http://www.anp.gov.br). |  |
| **descANP** | **string** | Descrição do Produto conforme ANP. Utilizar a descrição de produtos do Sistema de Informações de Movimentação de Produtos - SIMP (http://www.anp.gov.br/simp/). |  |
| **pGLP** | **number** | Percentual do GLP derivado do petróleo no produto GLP (cProdANP&#x3D;210203001). Informar em número decimal o percentual do GLP derivado de petróleo no produto GLP. Valores 0 a 100. | [opcional]  |
| **pGNn** | **number** | Percentual de gás natural nacional - GLGNn para o produto GLP (cProdANP&#x3D;210203001). Informar em número decimal o percentual do Gás Natural Nacional - GLGNn para o produto GLP. Valores de 0 a 100. | [opcional]  |
| **pGNi** | **number** | Percentual de gás natural importado GLGNi para o produto GLP (cProdANP&#x3D;210203001). Informar em número deciaml o percentual do Gás Natural Importado - GLGNi para o produto GLP. Valores de 0 a 100. | [opcional]  |
| **vPart** | **number** | Valor de partida (cProdANP&#x3D;210203001). Deve ser informado neste campo o valor por quilograma sem ICMS. | [opcional]  |
| **CODIF** | **string** | Código de autorização / registro do CODIF. Informar apenas quando a UF utilizar o CODIF (Sistema de Controle do    Diferimento do Imposto nas Operações com AEAC - Álcool Etílico Anidro Combustível). | [opcional]  |
| **qTemp** | **number** | Quantidade de combustível  faturada à temperatura ambiente.  Informar quando a quantidade  faturada informada no campo  qCom (I10) tiver sido ajustada para  uma temperatura diferente da  ambiente. | [opcional]  |
| **UFCons** | **string** | Sigla da UF de Consumo. |  |
| **CIDE** | [**NfeSefazCIDE**](NfeSefazCIDE.md) |  | [opcional]  |
| **encerrante** | [**NfeSefazEncerrante**](NfeSefazEncerrante.md) |  | [opcional]  |
| **pBio** | **number** | Percentual do índice de mistura do Biodiesel (B100) no Óleo Diesel B instituído pelo órgão regulamentador. | [opcional]  |
| **origComb** | [**Array**](NfeSefazOrigComb.md) |  | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

