# Contributing

1. Branch from `develop`; open the pull request against `develop`.
2. Write everything in English: page text, meta tags, comments, commit messages, PR title and description.
   No Cyrillic characters in tracked text files. Check locally:

   ```bash
   LC_ALL=C.UTF-8 git grep -nIP '[\x{0400}-\x{04FF}]'   # must print nothing
   ```

3. Do not edit `catalog/**` by hand; change `build-catalog.mjs` and regenerate.
4. Keep page URLs stable; keep canonical and hreflang links consistent with `sitemap.xml`.
