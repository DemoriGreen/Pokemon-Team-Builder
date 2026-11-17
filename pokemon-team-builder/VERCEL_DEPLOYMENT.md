# Vercel deployment checklist

1. Push this project to a public GitHub repository.
2. In Vercel, choose Add New → Project and import the GitHub repository.
3. Use the Vite defaults: Build Command `npm run build`; Output Directory `dist`; Install Command `npm install`.
4. Deploy and test `/`, `/pokedex`, `/pokemon/pikachu`, `/teams`, and a team detail route.
5. If refreshing nested routes returns a 404, add a `vercel.json` rewrite to serve `/index.html` for application routes, then redeploy.
