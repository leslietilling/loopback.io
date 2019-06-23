---
lang: en
title: 'API docs: openapi-v3.getmodelschemaref'
keywords: LoopBack 4.0, LoopBack 4
sidebar: lb4_sidebar
permalink: /doc/en/lb4/apidocs.openapi-v3.getmodelschemaref.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/openapi-v3](./openapi-v3.md) &gt; [getModelSchemaRef](./openapi-v3.getmodelschemaref.md)

## getModelSchemaRef() function

Describe the provided Model as a reference to a definition shared by multiple endpoints. The definition is included in the returned schema.

<b>Signature:</b>

```typescript
export declare function getModelSchemaRef(modelCtor: Function, options?: JsonSchemaOptions): SchemaRef;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  modelCtor | <code>Function</code> | The model constructor (e.g. <code>Product</code>) |
|  options | <code>JsonSchemaOptions</code> | Additional options |

<b>Returns:</b>

`SchemaRef`

## Example


```ts
const schema = {
  $ref: '#/components/schemas/Product',
  definitions: {
    Product: {
      title: 'Product',
      properties: {
        // etc.
      }
    }
  }
}

```

