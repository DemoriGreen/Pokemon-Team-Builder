# Pokémon Team Builder

A responsive React single-page application for exploring Pokémon and building teams of up to six Pokémon. This MVP follows the uploaded project proposal and uses the public PokéAPI.

## Features
- Browse a paginated Pokédex with name and type filters.
- Search Pokémon by name and view artwork, types, abilities, and base stats.
- Create multiple teams, add up to six Pokémon, and remove team members.
- Save team data in browser local storage (no account or cloud sync in this MVP).
- Responsive layout, loading/error states, and a not-found route.

## Routes
| Route | Purpose |
|---|---|
| `/` | Home and Pokémon name search |
| `/pokedex` | Browse, search, and filter Pokémon |
| `/pokemon/:name` | Pokémon details |
| `/teams` | Create and view teams |
| `/teams/:teamId` | Team details and member removal |
| `*` | 404 page |

## Technologies
React, Vite, React Router, React Context API, React Hooks, CSS, Vitest, React Testing Library, and PokéAPI.

## API
Base URL: `https://pokeapi.co/api/v2/`. Uses the Pokémon list and individual Pokémon endpoints. No API key is required. Documentation: https://pokeapi.co/docs/v2.

## Setup
1. Install Node.js LTS.
2. Open a terminal in this project folder.
3. Run `npm install`.
4. Run `npm run dev` and open the local URL printed by Vite.

## Tests and build
- `npm test` runs the Vitest/React Testing Library tests.
- `npm run build` creates the production build in `dist`.
- `npm run preview` previews the production build.

## Deployment
Not deployed yet. To deploy, push the project to GitHub, import the repository into Vercel, and use `npm run build` with output directory `dist`. Test direct navigation to nested routes after deployment.

## Known MVP limitations
- Authentication, user accounts, protected routes, and administrator tools are not included in this MVP.
- Teams are stored only in this browser's local storage; there is no cross-device sync.
- Type filtering applies to the currently loaded page of 24 Pokémon.
- Loading the Pokédex requests detail data for each displayed entry and depends on the public API/network.

## Future enhancements
Add authentication and roles, backend/database storage, team sharing, API caching, broader filtering, and more comprehensive tests.

## Submission links
- GitHub repository: **Add your public repository URL here after creating it.**
- Live Vercel application: **Not deployed yet. Add the live URL after deployment.**
