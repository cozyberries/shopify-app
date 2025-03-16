# Shopify App

A Shopify theme application for Cozyberries.

## Prerequisites

- macOS (for this guide)
- Node.js (v16 or higher)
- Shopify CLI
- Shopify Partners account
- Development store

## Installation Steps

1. Install Node.js:
```bash
brew install node
```

2. Install Shopify CLI:
```bash
brew tap shopify/shopify
brew install shopify-cli
```

3. Verify Shopify CLI installation:
```bash
shopify version
```

## Project Setup

1. Clone the repository:
```bash
git clone https://github.com/cozyberries/shopify-app.git
cd shopify-app
```

2. Install dependencies (if any):
```bash
npm install
```

3. Set up environment variables:
```bash
# For macOS/Linux
export SHOPIFY_FLAG_STORE=4v6ju2-7e.myshopify.com

# To make it permanent, add to your ~/.zshrc or ~/.bash_profile:
echo 'export SHOPIFY_FLAG_STORE=4v6ju2-7e.myshopify.com' >> ~/.zshrc
source ~/.zshrc
```

## Running the App Locally

1. Make sure you have a development store set up in your Shopify Partners account
2. Start the development server:
```bash
shopify theme dev
```
Note: If you haven't set the environment variable, you can still specify the store URL directly:
```bash
shopify theme dev --store=4v6ju2-7e.myshopify.com
```

3. When prompted:
   - Press any key to open the login page in your browser
   - Log in to your Shopify Partners account
   - Enter the verification code shown in the terminal
   - Authorize the CLI to access your store

4. The development server will start and:
   - Watch for changes in your theme files
   - Hot-reload changes in your browser
   - Allow you to preview your theme in real-time

## Project Structure

```
shopify-app/
├── assets/          # Theme assets (JS, CSS, images)
├── config/          # Theme configuration files
├── layout/          # Theme layout templates
├── locales/         # Translation files
├── sections/        # Theme section templates
├── snippets/        # Reusable code snippets
└── templates/       # Theme templates for different page types
```

## Development Guidelines

- Follow Shopify's best practices for theme development
- Use semantic HTML and follow accessibility guidelines
- Ensure responsive design for all device types
- Follow BEM naming convention for CSS classes
- Document code thoroughly

## Useful Resources

- [Shopify Developer Documentation](https://shopify.dev/docs)
- [Shopify Liquid Reference](https://shopify.dev/docs/themes/liquid/reference)
- [Shopify Theme Development](https://shopify.dev/docs/themes)
- [Shopify Partners Dashboard](https://partners.shopify.com)