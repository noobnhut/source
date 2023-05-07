# npm create vite@latest
# axios: npm install axios :
# Setup 1: 
import axios from 'axios'

const instance = axios.create({
  baseURL: `${import.meta.env.VITE_API_BASE_URL}`,
  headers: {
    'Content-Type': 'application/json'
  }
})

export default {
  install: (app) => {
    app.config.globalProperties.$axios = instance
  }
}

# Setup 2
import axios from 'axios' :))
# route: npm install vue-router@4
import {
  createRouter,
  createWebHistory
} from 'vue-router'

const router = createRouter({
  history: createWebHistory(),
  routes: [{
      path: '?',
      name: '?',
     component: () => import('?')
    }, 
  ]
})
export default router;

# dotenv: npm i dotenv - VITE_API_BASE_URL=http://localhost:3000/api/
# tailwindcss: 
# npm install -D tailwindcss postcss autoprefixer
# tailwind.config.js:
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{vue,js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}


# postcss.config.js
export default {
  plugins: {
    tailwindcss: {},
    autoprefixer: {},
  },
}

# style css 
@tailwind base;
@tailwind components;
@tailwind utilities;