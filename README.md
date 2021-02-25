# GitHub Issue Action

This Action opens a new GitHub Issue.

## Inputs

### `token`

**Required** GitHub Token.

### `title`

**Required** Issue Title.

### `body`

Issue Body.

### `assignees`

Issue assignees. Passed as a formatted multi-line string using the | character.

## Outputs

### `issue`

The issue object as a json string.

## Example Usage

```yaml
uses: michael-crawford/open-issue@v1
with:
  token: ${{ secrets.GITHUB_TOKEN }}
  title: My Issue Title
  body: My Issue Body
  assignees: |
    michael-crawford
    cayman-crawford
```
