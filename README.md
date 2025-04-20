# Welcome to your Lovable project

## Project info

**URL**: https://lovable.dev/projects/04d36fb9-1dbb-4700-98f5-c8a6d37a77bb

## How can I edit this code?

There are several ways of editing your application.

**Use Lovable**

Simply visit the [Lovable Project](https://lovable.dev/projects/04d36fb9-1dbb-4700-98f5-c8a6d37a77bb) and start prompting.

Changes made via Lovable will be committed automatically to this repo.

**Use your preferred IDE**

If you want to work locally using your own IDE, you can clone this repo and push changes. Pushed changes will also be reflected in Lovable.

The only requirement is having Node.js & npm installed - [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating)

Follow these steps:

```sh
# Step 1: Clone the repository using the project's Git URL.
git clone <YOUR_GIT_URL>

# Step 2: Navigate to the project directory.
cd <YOUR_PROJECT_NAME>

# Step 3: Install the necessary dependencies.
npm i

# Step 4: Start the development server with auto-reloading and an instant preview.
npm run dev
```

**Edit a file directly in GitHub**

- Navigate to the desired file(s).
- Click the "Edit" button (pencil icon) at the top right of the file view.
- Make your changes and commit the changes.

**Use GitHub Codespaces**

- Navigate to the main page of your repository.
- Click on the "Code" button (green button) near the top right.
- Select the "Codespaces" tab.
- Click on "New codespace" to launch a new Codespace environment.
- Edit files directly within the Codespace and commit and push your changes once you're done.

## What technologies are used for this project?

This project is built with:

- Vite
- TypeScript
- React
- shadcn-ui
- Tailwind CSS

## Eco Badge & Enhanced Product Integration

### Eco Badge for Organic Products
- Organic products (detected via name/materials/certifications) display an "Organic" eco badge in the product listing.
- Badge is visible in the UI via the `EcoBadge` component.

### Enhanced Product Scraping
- Backend scrapes myecokart.com and ecovians.com for eco-friendly products.
- Scraping logic attempts to detect "organic" status and adds it to product data.

### Ingredient-based Eco Score Calculation
- The `/api/eco-score-percent` endpoint accepts a dictionary of ingredient names and percentages, returning a weighted eco score.
- The frontend (EcoScoreTool) uses this endpoint for ingredient analysis.

## How to Run & Test

1. **Install dependencies:**
   ```sh
   npm install
   cd backend && npm install
   ```
2. **Set up environment:**
   - Set `SERPAPI_KEY` in your environment for product scraping.
3. **Run backend:**
   ```sh
   cd backend && npm start
   ```
4. **Run frontend:**
   ```sh
   npm run dev
   ```
5. **Test features:**
   - Visit the Eco Score Tool and Product Catalog to see eco badges and ingredient-based eco scoring.
   - Check backend logs for scraping/debug info.

## API Endpoints

- `POST /api/eco-score-percent`: Calculate eco score from ingredient percentages.
- `GET /api/products`: Get eco-friendly products from integrated sites.

## Contribution & Troubleshooting
- If you encounter issues with badges or product scraping, check the backend logs and ensure your API keys are set.
- For feature requests or bugs, open an issue or contact the maintainers.


## How can I deploy this project?

Simply open [Lovable](https://lovable.dev/projects/04d36fb9-1dbb-4700-98f5-c8a6d37a77bb) and click on Share -> Publish.

## Can I connect a custom domain to my Lovable project?

Yes, you can!

To connect a domain, navigate to Project > Settings > Domains and click Connect Domain.

Read more here: [Setting up a custom domain](https://docs.lovable.dev/tips-tricks/custom-domain#step-by-step-guide)
