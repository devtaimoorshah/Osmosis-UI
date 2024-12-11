# Frontend UI Clone for Statoswap 🚀🌐

![Osmosischain-banner](https://user-images.githubusercontent.com/4606373/167008669-fb3cafa8-e66e-4cdf-8599-3308039cc58c.png)

> Note: This codebase is a frontend UI clone where I have replicated the user interface design and improved it for a better experience. There is an API issue that I created myself due to performance concerns, but don't worry—we will be developing our own API for the MantraChain project as it will be deployed on the MantraChain blockchain. Everything is under control, and we will resolve any issues as we move forward.

## Overview 💻

This project is a UI frontend clone with the following technologies:

- [TypeScript](https://www.typescriptlang.org/): for type checking
- [React](https://reactjs.org/): for UI components and rendering
- [Tailwind CSS](https://tailwindcss.com/): for styling and theming
- [Next.js](https://nextjs.org/): for server-side rendering (SSR), CDN, and SEO
  - Deployed on [Vercel](https://vercel.com/solutions/nextjs) for optimizations out of the box, behind [CloudFlare](https://www.cloudflare.com/)
- [Turbo Repo](https://turbo.build/repo): for mono repo management with package script execution and build caching (including shared remote caching in Vercel)
- [Lerna](https://lerna.js.org/): for managing package releases

## Getting Started 🚀

### Prerequisites

1. **Install Yarn** if you haven't already:

   - Install Yarn from [here](https://yarnpkg.com/getting-started/install).

2. **Install Node.js**:
   - Ensure you have [Node.js](https://nodejs.org/en/) installed (version 20 or higher).

### Steps to Run the Frontend

1. **Install dependencies:**

```bash
yarn
```

2. **Build the application:**

```bash
yarn build
```

3. **Go to web dependency:**

```bash
cd packages
cd web
```

4. **Run the frontend:**

```bash
yarn dev
```

This will start the application locally at [localhost:3000](http://localhost:3000).

## Osmosis API Issue 🔧

While developing the UI, I noticed an issue with the API performance, which I decided to address by creating an API myself to resolve the lag. However, as you mentioned that the project will be deployed on the MantraChain blockchain, we will be building our own API specifically for the project. Rest assured, this is being worked on, and we will ensure everything is functioning smoothly.

## Contributions 👨‍💻

We welcome contributions! If you're interested in helping out, please follow these steps to get started:

1. **Install dependencies:**

```bash
yarn
```

2. **Run a local build:**

```bash
yarn build
```

3. **Run the local server:**

```bash
yarn dev
```

4. **If you have a Vercel account, optionally sign into Turbo Repo for remote caching by running:**

```bash
npx turbo login npx turbo link
```

## Testing on Osmosis Testnet

To develop against the Osmosis testnet, set up your `.env.local` file in the `web` package root with the appropriate settings:

## Osmosis Chain Configuration

```bash
NEXT_PUBLIC_IS_TESTNET=true
NEXT_PUBLIC_OSMOSIS_RPC_OVERWRITE=http://localhost:26657/
NEXT_PUBLIC_OSMOSIS_REST_OVERWRITE=http://localhost:1317/
NEXT_PUBLIC_OSMOSIS_CHAIN_ID_OVERWRITE=localosmosis
# NEXT_PUBLIC_OSMOSIS_EXPLORER_URL_OVERWRITE=https://testnet.mintscan.io/osmosis-testnet/txs/{txHash}
# NEXT_PUBLIC_OSMOSIS_CHAIN_NAME_OVERWRITE=Osmosis (Testnet v13.X latest)
```

## Deployment 🚀

To deploy the frontend, run the following commands:

1. **Build the app:**

```bash
yarn build
```

2. **Start the production server:**

```bash
yarn start
```

## Translations 🌍

To add translations, edit the JSON translation files in `packages/web/translations` or use the [inlang](https://inlang.com/) editor. For a list of localization tasks, check the localization scripts in the web package.

## License 📄

This project is licensed under the [MIT License](LICENSE).

## Contact Us 📧

If you encounter any issues or need any assistance, feel free to reach out to us:

- Email: [info@techsurge.co.uk](mailto:info@techsurge.co.uk)
- Phone: +44 7404 925516
