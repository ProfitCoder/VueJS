# VueJS

A hands-on repository for learning Vue 3 with JavaScript and Vite. It includes a simple name list that demonstrates how Vue connects user input, reactive state, and the UI, along with a starter project for further practice.

## Projects

| Project | Description |
| --- | --- |
| [`first-vue-project`](./first-vue-project) | A Vue 3 example that reads a name from an input, adds it to a reactive list, and clears the input. |
| [`Excercises1_Vue`](./Excercises1_Vue) | A Vue 3 and Vite starter with a minimal `App.vue`, ready for additional exercises. |

## Concepts Covered

- Reactive state with `ref()` and the Composition API
- Two-way binding between an input and application state with `v-model`
- Click event handling with `@click`
- Rendering a list from reactive data with `v-for`

## Getting Started

### Requirements

- Node.js 22.18.0 or later within the 22.x series, or Node.js 24.12.0 or later
- npm and Git

### Run Locally

```bash
git clone https://github.com/ProfitCoder/VueJS.git
cd VueJS/first-vue-project
npm install
npm run dev
```

Open the local URL shown in the terminal. Enter a name and click **Añadir a la lista** to add it to the ordered list.

To run the starter project, use `cd VueJS/Excercises1_Vue` after cloning and run the same npm commands. Each project has its own `package.json` and dependencies.

## npm Scripts

Run these commands from the project directory.

| Command | Purpose |
| --- | --- |
| `npm run dev` | Start the Vite development server. |
| `npm run build` | Generate a production build in `dist/`. |
| `npm run preview` | Preview the production build locally after running `npm run build`. |

## Author

[ProfitCoder](https://github.com/ProfitCoder)
