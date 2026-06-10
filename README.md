# Linkspector Experiments

Experiments with [Linkspector](https://github.com/UmbrellaDocs/linkspector).

Linkspector v0.5.3 complained about correct links if there were more than 10 links to the same resource that differ only in their anchor values.

To test:
- clone repo
- `npm i`
- `npm t`

The only difference between the input files `correct-links*.md` is that some of the links are commented out:
- `correct-links3.md` contains 13 links, the last three of which result in a `null Cannot read properties of null (reading 'status')` error message
- `correct-links2.md` contains the same 13 links, the first link commented out, and now only the last two links cause errors
- `correct-links1.md` has the first two commented out, and only the last one causes an error
- `correct-links.md` has the first three commented out, and now there are no errors

[Fixed](https://github.com/UmbrellaDocs/linkspector/pull/178) with Linkspector v0.5.5 :smile:
