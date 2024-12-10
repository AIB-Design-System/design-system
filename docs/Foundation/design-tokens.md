---
sidebar_position: 1
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# Design Tokens

Design tokens are the building blocks of all UI elements. The same tokens are used in designs, tools, and code.

## Prototypes embedding

<div className="row">
  {/* Left Column */}
  <div className="col col--6">
    <iframe 
  style={{ border: "none" }} 
  width="390" 
  height="924" 
  src="https://embed.figma.com/proto/sgpxUkDc1WBiNukJqZKTx1/Untitled?page-id=8%3A6&node-id=8-334&node-type=canvas&viewport=896%2C713%2C1.52&scaling=scale-down&content-scaling=fixed&embed-host=share&chrome=0&embed-host=share" 
  allowfullscreen
></iframe>
  </div>

  {/* Right Column */}
  <div className="col col--6">
   <iframe 
  style={{ border: "none" }} 
  width="390" 
  height="924" 
  src="https://embed.figma.com/proto/sgpxUkDc1WBiNukJqZKTx1/Untitled?page-id=8%3A6&node-id=8-334&node-type=canvas&viewport=896%2C713%2C1.52&scaling=scale-down&content-scaling=fixed&embed-host=share&chrome=0&embed-host=share" 
  allowfullscreen
></iframe>
  </div>
</div>

## Tabbing navigation

<Tabs>
<TabItem value="npm" label="npm" default>
bash
npm install --save raw-loader
</TabItem> 
<TabItem value="yarn" label="Yarn">
yarn add raw-loader
</TabItem> 
<TabItem value="pnpm" label="pnpm">
pnpm add raw-loader
</TabItem>
</Tabs>

## Create a docs version

Release a version 1.0 of your project:

```bash
npm run docusaurus docs:version 1.0
```

The `docs` folder is copied into `versioned_docs/version-1.0` and `versions.json` is created.

Your docs now have 2 versions:

- `1.0` at `http://localhost:3000/docs/` for the version 1.0 docs
- `current` at `http://localhost:3000/docs/next/` for the **upcoming, unreleased docs**

## Add a Version Dropdown

To navigate seamlessly across versions, add a version dropdown.

Modify the `docusaurus.config.js` file:

```js title="docusaurus.config.js"
export default {
  themeConfig: {
    navbar: {
      items: [
        // highlight-start
        {
          type: 'docsVersionDropdown',
        },
        // highlight-end
      ],
    },
  },
};
```

The docs version dropdown appears in your navbar:

![Docs Version Dropdown](./img/docsVersionDropdown.png)

## Update an existing version

It is possible to edit versioned docs in their respective folder:

- `versioned_docs/version-1.0/hello.md` updates `http://localhost:3000/docs/hello`
- `docs/hello.md` updates `http://localhost:3000/docs/next/hello`
