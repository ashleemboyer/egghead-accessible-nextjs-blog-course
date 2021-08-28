# How I Set up the Course Example

## Steps

1. Added a `.gitignore` file:
   ```
   .next
   node_modules
   ```
2. Installed main dependencies

   ```bash
   yarn add next react react-dom
   ```

3. Installed dev dependencies:

   ```bash
   yarn add --dev typescript @types/react
   ```

4. Added a `pages` directory
5. Added a `_app.tsx` file under `pages`:

   ```tsx
   import type { AppProps } from 'next/app';

   const App = ({ Component, pageProps }: AppProps) => {
     return <Component {...pageProps} />;
   };

   export default App;
   ```

6. Added a `tsconfig.json` file
7. Ran `yarn next`
8. Added an `index.tsx` file under `pages`:

   ```tsx
   const IndexPage = () => <h1>Hello, World!</h1>;

   export default IndexPage;
   ```

## Resources

- [Next.js - Manual Setup](https://nextjs.org/docs/getting-started#manual-setup)
- [Next.js - Adding TypeScript to Existing Projects](https://nextjs.org/docs/basic-features/typescript#existing-projects)
