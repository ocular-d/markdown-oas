<div align=center>
  <h1>Markdown OAS</h1>
  <p>Generate API docs from Swagger file into markdown file.</p>
</div>


Based on https://github.com/rmariuzzo/markdown-swagger

## Installation

```shell
npm install markdown-oas
```

### Usage

```shell
markdown-oas ./api/swagger/oas.yaml ./README.md
```

This will read the specified OAS file and generate a table describing the API inside the target markdown file.

The `markdown-oas` script will look for the for the following piece of text inside the target markdown file to do its stuff:

```markdown
<!-- markdown-oas -->
  Everything here will be replaced by markdown-oas
<!-- /markdown-oas -->
```

## Develop

### Testings

```shell
node index.js openapi.yaml test.md
```
