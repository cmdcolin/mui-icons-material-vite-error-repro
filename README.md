# mui-icons-material-vite-error-repro

Based on `yarn create vite --template react-ts vite-mui`

xref https://github.com/mui/material-ui/issues/45233

```bash

git clone https://github.com/cmdcolin/mui-icons-material-vite-error-repro
cd  mui-icons-material-vite-error-repro
yarn
yarn dev

```

## Error

```
  VITE v6.1.0  ready in 142 ms

  ➜  Local:   http://localhost:5173/
  ➜  Network: use --host to expose
  ➜  press h + enter to show help
2:59:14 PM [vite] Internal server error: Failed to resolve import "@mui/icons-material/Delete" from "src/App.tsx". Does the file exist?
  Plugin: vite:import-analysis
  File: /home/cdiesh/vite-mui/src/App.tsx:2:23
  16 |  }
  17 |  import IconButton from "@mui/material/IconButton";
  18 |  import DeleteIcon from "@mui/icons-material/Delete";
     |                          ^
  19 |  export default function IconButtons() {
  20 |    return /* @__PURE__ */ jsxDEV(IconButton, { "aria-label": "delete", children: /* @__PURE__ */ jsxDEV(DeleteIcon, {}, void 0, false, {
      at TransformPluginContext._formatLog (file:///home/cdiesh/vite-mui/node_modules/vite/dist/node/chunks/dep-CfG9u7Cn.js:47802:41)
      at TransformPluginContext.error (file:///home/cdiesh/vite-mui/node_modules/vite/dist/node/chunks/dep-CfG9u7Cn.js:47799:16)
      at normalizeUrl (file:///home/cdiesh/vite-mui/node_modules/vite/dist/node/chunks/dep-CfG9u7Cn.js:45942:23)
      at process.processTicksAndRejections (node:internal/process/task_queues:105:5)
      at async file:///home/cdiesh/vite-mui/node_modules/vite/dist/node/chunks/dep-CfG9u7Cn.js:46061:37
      at async Promise.all (index 4)
      at async TransformPluginContext.transform (file:///home/cdiesh/vite-mui/node_modules/vite/dist/node/chunks/dep-CfG9u7Cn.js:45988:7)
      at async EnvironmentPluginContainer.transform (file:///home/cdiesh/vite-mui/node_modules/vite/dist/node/chunks/dep-CfG9u7Cn.js:47597:18)
      at async loadAndTransform (file:///home/cdiesh/vite-mui/node_modules/vite/dist/node/chunks/dep-CfG9u7Cn.js:41305:27)
2:59:14 PM [vite] (client) Pre-transform error: Failed to resolve import "@mui/icons-material/Delete" from "src/App.tsx". Does the file exist?
  Plugin: vite:import-analysis
  File: /home/cdiesh/vite-mui/src/App.tsx:2:23
  16 |  }
  17 |  import IconButton from "@mui/material/IconButton";
  18 |  import DeleteIcon from "@mui/icons-material/Delete";
     |                          ^
  19 |  export default function IconButtons() {
  20 |    return /* @__PURE__ */ jsxDEV(IconButton, { "aria-label": "delete", children: /* @__PURE__ */ jsxDEV(DeleteIcon, {}, void 0, false, {



```
