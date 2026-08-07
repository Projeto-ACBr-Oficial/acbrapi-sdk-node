# ACBr API: SDK para Node.js

Biblioteca para uso da [ACBr API](https://www.acbr.api.br) com [Node.js](https://nodejs.org).
Consultar também a [documentação oficial da ACBr API](https://dev.acbr.api.br/docs).

A referência dos endpoints e DTOs deste SDK está em [docs/](docs/README.md).

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
