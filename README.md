Reproduce error
===
Should work
---
```
npm install
npm run clean-build-run
```

Should fail
---
Remove comment in line 2 in `index.ts` (enable the call to `unknonwn()`)
```
npm run clean-build-run
```

Note
---
The command `npm run compile` will detect the problem and since `.parcelrc` is in place, so should the parcel command