# ML Playground

A frontend-only Machine Learning teaching app. Every model (Logistic
Regression, Decision Tree, Random Forest, Gradient Boosting, Naive Bayes,
KNN, SVM, Linear/Ridge/Lasso/ElasticNet, KMeans, DBSCAN, Agglomerative
Clustering) is implemented in plain JavaScript and actually trains, in the
browser, on real embedded datasets (Iris, Wine, Breast Cancer, Titanic,
California Housing, and a digits dataset standing in for MNIST) — or on a
CSV you upload yourself. No backend, no API keys.

## Run it locally

```bash
npm install
npm run dev
```

Then open the printed `localhost` URL.

## Build for production

```bash
npm run build
```

Static files are written to `dist/`. Deploy that folder to any static host
(Vercel, Netlify, Cloudflare Pages, GitHub Pages, S3, etc.) — there is
nothing else to configure.

## Project structure

```
index.html          Vite entry HTML
src/main.jsx         Mounts the React app
src/App.jsx           The entire application (components, ML engine, data, styles)
```

`src/App.jsx` is intentionally a single large file — it was built as a
self-contained artifact, so all logic, styling, and data live together
rather than being split across many files.
