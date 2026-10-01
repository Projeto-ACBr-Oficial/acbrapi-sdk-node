# RTCInfoTributosAbrasfMun

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **pIBSMun** | **number** | Alíquota do Município para IBS. | [opcional]  |
| **pRedAliqMun** | **number** | Percentual de redução de alíquota municipal. | [opcional]  |
| **pAliqEfetMun** | **number** | Alíquota efetiva do IBS municipal.  pAliqEfetMun &#x3D; pIBSMun x (1 - pRedAliqMun) x (1 - pRedutor) | [opcional]  |
| **vIBSMun** | **number** | Valor do IBS municipal (R$).  vIBSMun &#x3D; vBC x (pIBSMun ou pAliqEfetMun) | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

