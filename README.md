# OptimaML Studio

OptimaML Studio is a fully client-side Machine Learning sandbox and interactive visualization platform. The application implements popular supervised and unsupervised algorithms from scratch in pure JavaScript, training models directly inside the browser with zero backend dependencies, API keys, or database integrations.

---

## Demo 
- https://ml-playground-lyart.vercel.app/
## Key Features

- **Zero-Backend Client-Side Training**: All mathematical calculations, gradient descent steps, tree-splitting, and coordinate descents run natively in the browser.
- **Interactive Predictor Panel**: Tune model input features dynamically using synchronized sliders and numeric inputs, and view live classification probability breakdowns or regression gauges.
- **Preprocessing & Exploration Suite**: Inspect data summaries, compute correlation matrices, evaluate missing values, and handle category encoding directly inside the UI.
- **Visualization Studio**: Render scatter plots, histograms, bar charts, pie charts, and PCA (Power Iteration) projections computed on real-time dataset coordinates.
- **Model Evaluation Dashboard**: Access performance metrics including macro/micro Precision, Recall, F1-Scores, Confusion Matrices, ROC/AUC sweeps, and Feature Importance reports.
- **Enterprise Dark Slate Theme**: Polished, professional dark-slate aesthetic designed for optimal data readability.

---

## Supported Algorithms (Implemented from Scratch)

### Supervised Learning
- **Classification**: Logistic Regression (Softmax GD), Decision Trees (CART/Gini/Entropy), Random Forests (Bootstrap Bagging), Gradient Boosting, Gaussian Naive Bayes, K-Nearest Neighbors, Support Vector Machines (Linear/RBF Hinge-Loss via Pegasos SGD).
- **Regression**: Linear Regression, Ridge Regression (L2), Lasso Regression (L1), ElasticNet Regression, Decision Tree Regressors, Random Forest Regressors.

### Unsupervised Learning
- **Clustering**: K-Means Clustering, DBSCAN (Density-Based Clustering), Agglomerative Hierarchical Clustering.

---

## Quick Start (Local Development)

### Prerequisites
- Node.js (v18+)
- npm

### Installation
Clone the repository, install dependencies, and spin up the Vite development server:

```bash
# Clone the repository
git clone https://github.com/sauravv-kunwar/ML_Playground.git
cd ML_Playground

# Install dependencies
npm install

# Start development server
npm run dev
```

The dev server will host the site at `http://localhost:5173/`.

---

## Production Build & Deployment

To package the application for production:

```bash
npm run build
```

This compiles optimized static assets into the `dist/` directory. You can deploy this folder directly to any static hosting provider (e.g. Vercel, Netlify, Cloudflare Pages, or GitHub Pages) with zero extra configuration.

---

## Architecture & Project Structure

The project is structured simply to optimize modularity and loading speed:

```
index.html          # Entrypoint HTML document
src/main.jsx        # Mounts the React application
src/App.jsx         # App shell, UI components, stylesheet, and ML algorithms
vite.config.js      # Bundling settings
```

---

## License

This project is licensed under the MIT License - see the LICENSE file for details.
