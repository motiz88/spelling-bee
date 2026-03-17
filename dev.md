## Build Setup

```shell
# current versions are:
# node 20.5.1
# npm  9.8.0

# install dependencies
npm install

# dev server
npm run dev
# production build (fails to open locally with file:// protocol due to cors)
npm run build
```

### Create derivative files

_Warning_: this operation may result in the same puzzle repeating too often.
This operation is not idempotent. Re-creating allAnswers.json will change the order of the puzzles, which could result in the same puzzle twice in a row on deploy in the worst case. As of the latest version (v2.2.0) I've made `createRandomGenerator` that produces pseudo-random numbers but can be given a seed to produce the same sequence of random numbers. This should make the operation idempotent.

1. Create `AllWords.txt`
   This is only required if there are changes to `wordsAdded.txt` or `wordsRemoved.txt`.

   ```shell
   npm run createAllWords
   ```

2. Create `allAnswers$N.json`

   ```shell
   npm run createFiles
   ```

   `AllWords.txt` must already exist. It must contain a single word per line.
   `answers.txt` and pangrams.txt are created for debugging.
   `allAnswers.json` is created for use in the game.

## Linting

```
# lint check
npm run lint
# lint autofix
npm run lintfix
```

## Versioning

```shell
# set version explicitly
npm version <version>

# bump minor version
npm version minor
```

## Favicon

Favicons created with http://faviconer.com
http://faviconer.com/user/17914

## Page stats

Page counting at https://spelling-b.goatcounter.com/

- https://www.goatcounter.com/help/gdpr
  - github alt: https://github.com/arp242/goatcounter/blob/c8c50d8720862e605049c3492fd7b4f285de6e98/tpl/help/gdpr.markdown
- https://github.com/arp242/goatcounter/blob/c8c50d8720862e605049c3492fd7b4f285de6e98/tpl/help/consent.markdown
