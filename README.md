# gh-pagesify

Publish gh-pages like a breeze.

## Usage

1. `npm install -D gh-pagesify`
2. Configure your `package.json`.

    ```json
    {
      // ...
      "scripts": {
        "build": "# Build static files into `public` directory.",
        "deploy": "npm run build && gh-pagesify"
      },
      "gh-pages": {
        "repository": "foo/bar",
        "static": "public",
        "deploy": "deploy",
        "branch": "gh-pages"
      }
    }
    ```

3. `npm run deploy`

## Options

- `repository`: **Required.** `user-name/repository-name`
- `static`: Directory for static files. Default: `public`
- `deploy`: Temporary directory for deployment. Default: `deploy`
- `branch`: Branch for gh-pages. Default: `gh-pages`
