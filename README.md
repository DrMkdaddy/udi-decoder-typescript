# FDA & EU MDR Medical Device UDI Decoder (GS1, HIBCC, ICCBBA) — TypeScript / JavaScript Client

[![npm version](https://img.shields.io/npm/v/@noor-mkdad/udi-decoder-client.svg)](https://www.npmjs.com/package/@noor-mkdad/udi-decoder-client)
[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/57865358-8bafe64c-1441-4fe3-ba7a-2d60bdeb7dc5)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![RapidAPI Listing](https://img.shields.io/badge/RapidAPI-Dedicated%20Listing-blueviolet)](https://rapidapi.com/noor-mkdad-apis-noor-mkdad-apis-default/api/fda-eu-mdr-medical-device-udi-decoder-gs1-hibcc-iccbba)

Official zero-dependency, ultra-lightweight Node.js & browser client for **FDA & EU MDR Medical Device UDI Decoder (GS1, HIBCC, ICCBBA)**.

> Instant <5ms GS1-128, HIBCC Modulo-43 & ICCBBA ISBT 128 medical device barcode parser for FDA 21 CFR 801 & EU MDR compliance.

> 🔑 **Get your Dedicated API Key:** [Subscribe to FDA & EU MDR Medical Device UDI Decoder (GS1, HIBCC, ICCBBA) on RapidAPI](https://rapidapi.com/noor-mkdad-apis-noor-mkdad-apis-default/api/fda-eu-mdr-medical-device-udi-decoder-gs1-hibcc-iccbba)

---

## 🚀 Installation

```bash
npm install @noor-mkdad/udi-decoder-client
# or
pnpm add @noor-mkdad/udi-decoder-client
# or
yarn add @noor-mkdad/udi-decoder-client
```

---

## ⚡ Quickstart

```typescript
import { UdiDecoderClient } from '@noor-mkdad/udi-decoder-client';

// Pass your RapidAPI key for authenticated edge access
const client = new UdiDecoderClient({
  apiKey: process.env.RAPIDAPI_KEY // Get key from https://rapidapi.com/noor-mkdad-apis-noor-mkdad-apis-default/api/fda-eu-mdr-medical-device-udi-decoder-gs1-hibcc-iccbba
});

async function run() {
  const result = await client.validate({
    // Enter validation payload
  });

  if (result.success) {
    console.log('Result:', result.data);
  } else {
    console.error('Error:', result.error);
  }
}

run();
```

---

## 📚 API Reference

### `new UdiDecoderClient(config)`
- `config.apiKey` *(optional)*: RapidAPI Key (`x-rapidapi-key`).
- `config.baseUrl` *(optional)*: Direct edge worker override URL.

### `client.validate(payload)`
Dispatches standard validation / parse request with sub-5ms latency.

### `client.getHealth()`
Checks edge isolate health and responsiveness.

---

## 🔗 Links
- 📖 [RapidAPI Documentation & Key](https://rapidapi.com/noor-mkdad-apis-noor-mkdad-apis-default/api/fda-eu-mdr-medical-device-udi-decoder-gs1-hibcc-iccbba)

## 📄 License
MIT © Noor Mkdad
