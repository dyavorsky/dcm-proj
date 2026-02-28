I want to point Obsidan to **dcm-proj/content**  so that Obsidian doesn't load the rest of the dcm-proj repo into the vault, but I don't want 'content' to be the name of the vault

Simply changing the subdirectory name from **dcm-proj/content** to **dcm-proj/dcm-proj** however wreaks havoc with Quartz, which expects the content directory to be named 'content'

The solution is to rename the sub-directory to make Obsidan happy, but then to create a sym-link to make Quartz happy:

```zsh
mv content dcm-proj     # rename
ln -s dcm-proj content  # sym link
```

