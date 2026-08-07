# DocDedRed

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **chNFSe** | **string** | Chave de Acesso da NFS-e (Padrão Nacional). | [opcional]  |
| **chNFe** | **string** | Chave de Acesso da NF-e. | [opcional]  |
| **NFSeMun** | [**DocOutNFSe**](DocOutNFSe.md) |  | [opcional]  |
| **NFNFS** | [**DocNFNFS**](DocNFNFS.md) |  | [opcional]  |
| **nDocFisc** | **string** | Número de documento fiscal. | [opcional]  |
| **nDoc** | **string** | Número de documento não fiscal. | [opcional]  |
| **tpDedRed** | **number** | Identificação da Dedução/Redução:  * 1 - Alimentação e bebidas/frigobar  * 2 - Materiais  * 3 - Produção Externa  * 4 - Reembolso de despesas  * 5 - Repasse consorciado  * 6 - Repasse plano de saúde  * 7 - Serviços  * 8 - Subempreitada de mão de obra  * 9 - Profissional parceiro  * 99 - Outras deduções |  |
| **xDescOutDed** | **string** | Descrição da Dedução/Redução quando a opção é \&quot;99 - Outras Deduções\&quot;. | [opcional]  |
| **dtEmiDoc** | **Date** | Data da emissão do documento dedutível. Ano, mês e dia (AAAA-MM-DD). |  |
| **vDedutivelRedutivel** | **number** | Valor monetário total dedutível/redutível no documento informado (R$).  Este é o valor total no documento informado que é passível de dedução/redução. |  |
| **vDeducaoReducao** | **number** | Valor monetário utilizado para dedução/redução do valor do serviço da NFS-e que está sendo emitida (R$).  Deve ser menor ou igual ao valor deduzível/redutível (vDedutivelRedutivel). |  |
| **fornec** | [**InfoFornecDocDedRed**](InfoFornecDocDedRed.md) |  | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

