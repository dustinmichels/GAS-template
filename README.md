# Clasp Starter Template

Starter template for [Google Apps Script](https://developers.google.com/apps-script/) projects using [clasp](https://github.com/google/clasp).

Includes some helper functions and polyfills that I frequently use.

## Setup

### Install pacakges

```bash
# Make sure clasp & typescript are installed globally
npm install -g typescript
npm install -g @google/clasp

# install GAS types locally
npm i -S @types/google-apps-script
```

### Configure Stuff

```bash
# reset Git project
rm -rf .git
git init

# create package.json
npm init -y
```

### Setup Clasp

- `clasp login`
- Update `scriptId` in `.clasp.json` with an existing google script

## Development Notes

Git is set to ignore changes to `.gitignore`, because I want to ignore my `package-lock.json` in the template, but not in projects copied from template. Confusing...

To undo:

```bash
git update-index --no-assume-unchanged .gitignore
```
