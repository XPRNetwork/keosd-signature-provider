# Keosd Signature Provider
# Installation

NPM
```
npm i @proton/keosd-signature-provider
```

YARN
```
yarn add @proton/keosd-signature-provider
```

# Usage
```
import { JsonRpc, Api } from '@proton/js'
import { KeosdSignatureProvider } from '@proton/keosd-signature-provider'
import fetch from 'node-fetch'

const rpc = new JsonRpc(['https://proton.eoscafeblock.com'], { fetch })
const api = new Api({ rpc, signatureProvider: new KeosdSignatureProvider() })
```