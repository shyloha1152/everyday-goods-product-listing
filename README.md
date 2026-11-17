# Everyday Goods Product Listing

An Angular 21 standalone application for browsing products by category and adding available products to a cart.

## Run locally

Install dependencies and start the development server:

```bash
npm install
npm start
```

Open [http://localhost:4200](http://localhost:4200). The page reloads when application files change.

## Build

```bash
npm run build
```

The optimized production output is written to `dist/product-listing/`.

## Product data

The listing contains Laptop, Phone, Desk, and Chair. Product illustrations are stored locally under `public/images/`.

## QA verification

The category filtering, filtered product counts, initial and updated cart count, success message, disabled out-of-stock action, and local images were checked in the browser. No unit-test suite is configured in this scaffold.

## Prepare a ZIP submission (PowerShell)

From the project directory, create a ZIP that includes the source and lockfile while excluding generated dependencies and build output:

```powershell
Get-ChildItem -Force |
  Where-Object { $_.Name -notin @('node_modules', '.angular', 'dist') } |
  Compress-Archive -DestinationPath '..\product-listing-submission.zip' -Force
```

Include `FIXES_SUMMARY.txt` in the submission.
