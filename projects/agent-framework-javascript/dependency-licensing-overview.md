# Aries Framework JavaScript - Dependency Licenses

This document is aimed at providing insight about licensing for all **direct** dependencies of the repositories proposed to move. Each of the following sections is divided into sub sections. This is because all repositories are so called *mono-repos* and contains multiple packages. These packages are ultimately what ends up in the package manager repositories.

## Aries Framework JavaScript

### @aries-framework/action-menu

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| @aries-framework/core | 0.4.2 | Apache-2.0 | [@aries-framework/core](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| class-transformer | 0.5.1 | MIT | [class-transformer](git+https://github.com/typestack/class-transformer.git) |
| class-validator | 0.14.0 | MIT | [class-validator](git+https://github.com/typestack/class-validator.git) |
| rxjs | 7.8.0 | Apache-2.0 | [rxjs](git+https://github.com/reactivex/rxjs.git) |

### @aries-framework/anoncreds-rs

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| @aries-framework/anoncreds | 0.4.2 | Apache-2.0 | [@aries-framework/anoncreds](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| @aries-framework/core | 0.4.2 | Apache-2.0 | [@aries-framework/core](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| class-transformer | 0.5.1 | MIT | [class-transformer](git+https://github.com/typestack/class-transformer.git) |
| class-validator | 0.14.0 | MIT | [class-validator](git+https://github.com/typestack/class-validator.git) |
| rxjs | 7.8.0 | Apache-2.0 | [rxjs](git+https://github.com/reactivex/rxjs.git) |
| tsyringe | 4.8.0 | MIT | [tsyringe](git+https://github.com/Microsoft/tsyringe.git) |

### @aries-framework/anoncreds

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| @aries-framework/core | 0.4.2 | Apache-2.0 | [@aries-framework/core](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| bn.js | 5.2.1 | MIT | [bn.js](git+ssh://git@github.com/indutny/bn.js.git) |
| class-transformer | 0.5.1 | MIT | [class-transformer](git+https://github.com/typestack/class-transformer.git) |
| class-validator | 0.14.0 | MIT | [class-validator](git+https://github.com/typestack/class-validator.git) |
| reflect-metadata | 0.1.13 | Apache-2.0 | [reflect-metadata](git+https://github.com/rbuckton/reflect-metadata.git) |

### @aries-framework/askar

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| @aries-framework/core | 0.4.2 | Apache-2.0 | [@aries-framework/core](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| bn.js | 5.2.1 | MIT | [bn.js](git+ssh://git@github.com/indutny/bn.js.git) |
| class-transformer | 0.5.1 | MIT | [class-transformer](git+https://github.com/typestack/class-transformer.git) |
| class-validator | 0.14.0 | MIT | [class-validator](git+https://github.com/typestack/class-validator.git) |
| rxjs | 7.8.0 | Apache-2.0 | [rxjs](git+https://github.com/reactivex/rxjs.git) |
| tsyringe | 4.8.0 | MIT | [tsyringe](git+https://github.com/Microsoft/tsyringe.git) |

### @aries-framework/bbs-signatures

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| @aries-framework/core | 0.4.2 | Apache-2.0 | [@aries-framework/core](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| @mattrglobal/bbs-signatures | 1.3.1 | Apache-2.0 | [@mattrglobal/bbs-signatures](https://github.com/mattrglobal/bbs-signatures) |
| @mattrglobal/bls12381-key-pair | 1.0.0 | n/a | [@mattrglobal/bls12381-key-pair](git+https://github.com/mattrglobal/bls12381-key-pair) |
| @stablelib/random | 1.0.2 | MIT | [@stablelib/random](git+https://github.com/StableLib/stablelib.git) |

### @aries-framework/cheqd

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| @aries-framework/anoncreds | 0.4.2 | Apache-2.0 | [@aries-framework/anoncreds](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| @aries-framework/core | 0.4.2 | Apache-2.0 | [@aries-framework/core](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| @cheqd/sdk | 2.3.0 | Apache-2.0 | [@cheqd/sdk](git+https://github.com/cheqd/sdk.git) |
| @cheqd/ts-proto | 2.2.2 | Apache-2.0 | [@cheqd/ts-proto](git+https://github.com/cheqd/ts-proto.git) |
| @cosmjs/crypto | 0.29.5 | Apache-2.0 | [@cosmjs/crypto](https://github.com/cosmos/cosmjs/tree/main/packages/crypto) |
| @cosmjs/proto-signing | 0.31.1 | Apache-2.0 | [@cosmjs/proto-signing](https://github.com/cosmos/cosmjs/tree/main/packages/proto-signing) |
| @stablelib/ed25519 | 1.0.3 | MIT | [@stablelib/ed25519](git+https://github.com/StableLib/stablelib.git) |
| class-transformer | 0.5.1 | MIT | [class-transformer](git+https://github.com/typestack/class-transformer.git) |
| class-validator | 0.14.0 | MIT | [class-validator](git+https://github.com/typestack/class-validator.git) |
| rxjs | 7.8.0 | Apache-2.0 | [rxjs](git+https://github.com/reactivex/rxjs.git) |
| tsyringe | 4.8.0 | MIT | [tsyringe](git+https://github.com/Microsoft/tsyringe.git) |

### @aries-framework/core

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| @digitalcredentials/jsonld | 5.2.1 | BSD-3-Clause | [@digitalcredentials/jsonld](git+https://github.com/digitalcredentials/jsonld.js.git) |
| @digitalcredentials/jsonld-signatures | 9.3.2 | BSD-3-Clause | [@digitalcredentials/jsonld-signatures](git+https://github.com/digitalcredentials/jsonld-signatures.git) |
| @digitalcredentials/vc | 1.1.2 | BSD-3-Clause | [@digitalcredentials/vc](git+https://github.com/digitalcredentials/vc-js.git) |
| @multiformats/base-x | 4.0.1 | MIT | [@multiformats/base-x](https://github.com/gozala/@multiformats/base-x.git) |
| @stablelib/ed25519 | 1.0.3 | MIT | [@stablelib/ed25519](git+https://github.com/StableLib/stablelib.git) |
| @stablelib/random | 1.0.2 | MIT | [@stablelib/random](git+https://github.com/StableLib/stablelib.git) |
| @stablelib/sha256 | 1.0.1 | MIT | [@stablelib/sha256](git+https://github.com/StableLib/stablelib.git) |
| @types/ws | 8.5.5 | MIT | [@types/ws](https://github.com/DefinitelyTyped/DefinitelyTyped.git) |
| abort-controller | 3.0.0 | MIT | [abort-controller](git+https://github.com/mysticatea/abort-controller.git) |
| big-integer | 1.6.51 | Unlicense | [big-integer](git+ssh://git@github.com/peterolson/BigInteger.js.git) |
| borc | 3.0.0 | MIT | [borc](git+https://github.com/dignifiedquire/borc.git) |
| buffer | 6.0.3 | MIT | [buffer](git://github.com/feross/buffer.git) |
| class-transformer | 0.5.1 | MIT | [class-transformer](git+https://github.com/typestack/class-transformer.git) |
| class-validator | 0.14.0 | MIT | [class-validator](git+https://github.com/typestack/class-validator.git) |
| did-resolver | 4.1.0 | Apache-2.0 | [did-resolver](git+ssh://git@github.com/decentralized-identity/did-resolver.git) |
| lru_map | 0.4.1 | MIT | [lru_map](git+https://github.com/rsms/js-lru.git) |
| luxon | 3.3.0 | MIT | [luxon](git+https://github.com/moment/luxon.git) |
| make-error | 1.3.6 | ISC | [make-error](git://github.com/JsCommunity/make-error.git) |
| object-inspect | 1.12.3 | MIT | [object-inspect](git://github.com/inspect-js/object-inspect.git) |
| query-string | 7.1.3 | MIT | [query-string](git+https://github.com/sindresorhus/query-string.git) |
| reflect-metadata | 0.1.13 | Apache-2.0 | [reflect-metadata](git+https://github.com/rbuckton/reflect-metadata.git) |
| rxjs | 7.8.0 | Apache-2.0 | [rxjs](git+https://github.com/reactivex/rxjs.git) |
| tsyringe | 4.8.0 | MIT | [tsyringe](git+https://github.com/Microsoft/tsyringe.git) |
| uuid | 9.0.1 | MIT | [uuid](git+https://github.com/uuidjs/uuid.git) |
| varint | 6.0.0 | MIT | [varint](git://github.com/chrisdickinson/varint.git) |
| web-did-resolver | 2.0.27 | Apache-2.0 | [web-did-resolver](git+ssh://git@github.com/decentralized-identity/web-did-resolver.git) |

### @aries-framework/indy-sdk-to-askar-migration

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| @aries-framework/anoncreds | 0.4.2 | Apache-2.0 | [@aries-framework/anoncreds](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| @aries-framework/askar | 0.4.2 | Apache-2.0 | [@aries-framework/askar](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| @aries-framework/core | 0.4.2 | Apache-2.0 | [@aries-framework/core](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| @aries-framework/node | 0.4.2 | Apache-2.0 | [@aries-framework/node](git+https://github.com/hyperledger/aries-framework-javascript.git) |

### @aries-framework/indy-sdk

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| @aries-framework/anoncreds | 0.4.2 | Apache-2.0 | [@aries-framework/anoncreds](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| @aries-framework/core | 0.4.2 | Apache-2.0 | [@aries-framework/core](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| @stablelib/ed25519 | 1.0.3 | MIT | [@stablelib/ed25519](git+https://github.com/StableLib/stablelib.git) |
| @types/indy-sdk | 1.16.27 | MIT | [@types/indy-sdk](https://github.com/DefinitelyTyped/DefinitelyTyped.git) |
| class-transformer | 0.5.1 | MIT | [class-transformer](git+https://github.com/typestack/class-transformer.git) |
| class-validator | 0.14.0 | MIT | [class-validator](git+https://github.com/typestack/class-validator.git) |
| rxjs | 7.8.0 | Apache-2.0 | [rxjs](git+https://github.com/reactivex/rxjs.git) |
| tsyringe | 4.8.0 | MIT | [tsyringe](git+https://github.com/Microsoft/tsyringe.git) |

### @aries-framework/indy-vdr

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| @aries-framework/anoncreds | 0.4.2 | Apache-2.0 | [@aries-framework/anoncreds](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| @aries-framework/core | 0.4.2 | Apache-2.0 | [@aries-framework/core](git+https://github.com/hyperledger/aries-framework-javascript.git) |

### @aries-framework/node

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| @2060.io/ffi-napi | 4.0.8 | MIT | [@2060.io/ffi-napi](git+ssh://git@github.com/node-ffi-napi/node-ffi-napi.git) |
| @2060.io/ref-napi | 3.0.6 | MIT | [@2060.io/ref-napi](git://github.com/node-ffi-napi/ref-napi.git) |
| @aries-framework/core | 0.4.2 | Apache-2.0 | [@aries-framework/core](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| @types/express | 4.17.18 | MIT | [@types/express](https://github.com/DefinitelyTyped/DefinitelyTyped.git) |
| express | 4.18.2 | MIT | [express](git+https://github.com/expressjs/express.git) |
| ws | 8.13.0 | MIT | [ws](git+https://github.com/websockets/ws.git) |

### @aries-framework/openid4vc-client

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| @aries-framework/core | 0.4.2 | Apache-2.0 | [@aries-framework/core](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| @sphereon/openid4vci-client | 0.4.0 | Apache-2.0 | [@sphereon/openid4vci-client](https://registry.npmjs.org/@sphereon/openid4vci-client/-/openid4vci-client-0.4.0.tgz) |
| @stablelib/random | 1.0.2 | MIT | [@stablelib/random](git+https://github.com/StableLib/stablelib.git) |

### @aries-framework/question-answer

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| @aries-framework/core | 0.4.2 | Apache-2.0 | [@aries-framework/core](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| class-transformer | 0.5.1 | MIT | [class-transformer](git+https://github.com/typestack/class-transformer.git) |
| class-validator | 0.14.0 | MIT | [class-validator](git+https://github.com/typestack/class-validator.git) |
| rxjs | 7.8.0 | Apache-2.0 | [rxjs](git+https://github.com/reactivex/rxjs.git) |

### @aries-framework/react-native

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| @aries-framework/core | 0.4.2 | Apache-2.0 | [@aries-framework/core](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| @azure/core-asynciterator-polyfill | 1.0.2 | MIT | [@azure/core-asynciterator-polyfill](https://github.com/Azure/azure-sdk-for-js/tree/main/sdk/core/core-asynciterator-polyfill/README.md) |
| events | 3.3.0 | MIT | [events](git://github.com/Gozala/events.git) |

### @aries-framework/sd-jwt-vc

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| @aries-framework/askar | 0.4.2 | Apache-2.0 | [@aries-framework/askar](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| @aries-framework/core | 0.4.2 | Apache-2.0 | [@aries-framework/core](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| class-transformer | 0.5.1 | MIT | [class-transformer](git+https://github.com/typestack/class-transformer.git) |
| class-validator | 0.14.0 | MIT | [class-validator](git+https://github.com/typestack/class-validator.git) |
| jwt-sd | 0.1.2 | (MIT OR Apache-2.0) | [jwt-sd](git+https://github.com/berendsliedrecht/sd-jwt-ts.git) |

### @aries-framework/tenants

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| @aries-framework/core | 0.4.2 | Apache-2.0 | [@aries-framework/core](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| async-mutex | 0.4.0 | MIT | [async-mutex](git+https://github.com/DirtyHairy/async-mutex.git) |

## Aries Framework JavaScript Extensions

### @aries-framework/push-notifications

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| class-transformer | 0.5.1 | MIT | [class-transformer](git+https://github.com/typestack/class-transformer.git) |
| class-validator | 0.14.0 | MIT | [class-validator](git+https://github.com/typestack/class-validator.git) |
| reflect-metadata | 0.1.13 | Apache-2.0 | [reflect-metadata](git+https://github.com/rbuckton/reflect-metadata.git) |
| tsyringe | 4.7.0 | MIT | [tsyringe](git+https://github.com/Microsoft/tsyringe.git) |

### @aries-framework/react-hooks

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| rxjs | 7.5.6 | Apache-2.0 | [rxjs](git+https://github.com/reactivex/rxjs.git) |

### @aries-framework/redux-store

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| @reduxjs/toolkit | 1.8.3 | MIT | [@reduxjs/toolkit](git+https://github.com/reduxjs/redux-toolkit.git) |
| react-redux | 7.2.8 | MIT | [react-redux](git+https://github.com/reduxjs/react-redux.git) |

### @aries-framework/rest

| <div style="width:350px">Dependency</div> | <div style="width:60px">Version</div> | <div style="width:300px">License</div> | <div style="width:300px">Link</div> |
| ---------- | ------- | ------- | ---- |
| @aries-framework/core | 0.2.3 | Apache-2.0 | [@aries-framework/core](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| @aries-framework/node | 0.2.3 | Apache-2.0 | [@aries-framework/node](git+https://github.com/hyperledger/aries-framework-javascript.git) |
| @types/ws | 7.4.7 | MIT | [@types/ws](https://github.com/DefinitelyTyped/DefinitelyTyped.git) |
| body-parser | 1.20.0 | MIT | [body-parser](git+https://github.com/expressjs/body-parser.git) |
| cors | 2.8.5 | MIT | [cors](git+https://github.com/expressjs/cors.git) |
| express | 4.18.1 | MIT | [express](git+https://github.com/expressjs/express.git) |
| node-fetch | 2.6.7 | MIT | [node-fetch](git+https://github.com/bitinn/node-fetch.git) |
| reflect-metadata | 0.1.13 | Apache-2.0 | [reflect-metadata](git+https://github.com/rbuckton/reflect-metadata.git) |
| swagger-ui-express | 4.4.0 | MIT | [swagger-ui-express](git+ssh://git@github.com/scottie1984/swagger-ui-express.git) |
| tslog | 3.3.3 | MIT | [tslog](git+https://github.com/fullstack-build/tslog.git) |
| tsoa | 4.1.2 | MIT | [tsoa](git+https://github.com/lukeautry/tsoa.git) |
| tsyringe | 4.7.0 | MIT | [tsyringe](git+https://github.com/Microsoft/tsyringe.git) |
| ws | 7.5.8 | MIT | [ws](git+https://github.com/websockets/ws.git) |
| yargs | 17.5.1 | MIT | [yargs](git+https://github.com/yargs/yargs.git) |
