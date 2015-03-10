# gh-pagesify

Publish gh-pages like a breeze.

# Usage

Configure your `package.json`.

```json
{
  "scripts": {
    "deploy": "build_by_yourself && gh-pagesify"
  },
  "devDependencies": {
    "gh-pagesify": "^0.1.0"
  },
  "gh-pages": {
    "repository": "foo/bar",
    "static": "public",
    "deploy": "deploy",
    "branch": "gh-pages"
  }
}
```

## Options

- `repository`: **Required.** `user-name/repository-name`
- `static`: Directory for static files. Default: `public`
- `deploy`: Temporary directory for deployment. Default: `deploy`
- `branch`: Branch for gh-pages. Default: `gh-pages`
