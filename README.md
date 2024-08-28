
# Browser Library Template (with sveltekit for demos)

Starter template for client side libraries

Uses sveltekit's "library" template as a base and therefore has its packaging npm scripts.

From https://kit.svelte.dev/docs/packaging:

"When you're creating an app, the contents of src/routes is the public-facing stuff; src/lib contains your app's internal library."

"A component library has the exact same structure as a SvelteKit app, except that src/lib is the public-facing bit, and your root package.json is used to publish the package. src/routes might be a documentation or demo site that accompanies the library, or it might just be a sandbox you use during development."

I.e.: The lib part is the part that gets built and is intended to be imported as a package from another project and the src part with routes is there for demonstration etc.

The base template (createde by choosing "library" when running `npm create svelte@latest`) Can be used as a svelte component lib or a regular JS code lib. This template overrides parts of the base template to make it a pure JS library starter with sveltekit for demos, docs, etc.

- Can still use playwright and vitest to do unit testing.
- Automatically sets exports in package.json to index.js in dist (which corresponds to index.ts in lib). 
    - When running the `package` npm script the contents of lib will get built to this dir but other dirs will be ignored










