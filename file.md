Credify API doc OpenAPI Definition
TypeScript types
This repository automatically generates TypeScript interfaces based on openapi.yaml. Please install the latest version with npm or yarn.

Install
yarn add -D @credify/api-docs

npm install --dev @credify/api-docs
Usage
components contains all the definitions.

import { components } from "@credify/api-docs";

const response: components["AccessTokenResponse"] = {
  ...
}
# abc thêm test
