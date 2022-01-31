# random-word-generator

A [Deno](https://deno.land/) CLI which returns a string of random words from a given word list.

```
> deno run --allow-read ./main.ts
> cheeking-signs-riches
```

Similar to [unique-names-generator](https://github.com/andreasonny83/unique-names-generator).

## Flags
- `--words`: path to a word list file where each word is delimited by a newline. Default value is `./words/xkcd.txt`.
- `--separator`: string to insert in between each word in the output. Default value is `-`.
- `--length`: the number of words to output. Default value is `3`.

## Included word lists
- `xkcd.txt`: the dictionary for [XKCD](https://xkcd.com/)'s [Simple Writer](https://xkcd.com/simplewriter/), [Up Goer Five](https://xkcd.com/1133/), and [Thing Explainer](https://blog.xkcd.com/2015/05/13/new-book-thing-explainer/), minus contractions.
- `google-10000.txt`: the top 10,000 most common English words from [Google's Trillion Word Corpus](https://books.google.com/ngrams/info), minus swear words.
- `gfycat.txt`: the adjectives and animal names that [gfycat](https://gfycat.com/) uses to generate URLs.

## Word list sources
- [XKCD Simple Writer Word List](https://xkcd.com/simplewriter/words.js)
- [first20hours/google-10000-english](https://github.com/first20hours/google-10000-english)
- [gfycat adjectives](http://assets.gfycat.com/adjectives) and [gfycat animals](http://assets.gfycat.com/animals)
