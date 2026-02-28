To preview, run the following in the terminal, which follows the instructions [here](https://quartz.jzhao.xyz/build) but accommodates the custom directory **dcm-proj** rather than the default **content** (this is not strictly necessary given the sym link, see [[renaming the vault]])

```zsh
npx quartz build --serve --directory dcm-proj
```

Then visit <http://localhost:8080/> in a browser
