# HMM-based Part-of-Speech Tagger

Part-of-speech tagging with a Hidden Markov Model and the Viterbi algorithm,
built on the NLTK Treebank corpus — including modified Viterbi variants to
handle unknown words.

## What's inside

`HMM_based_POS_tagging.ipynb` walks through:

- Building transition and emission probabilities from the tagged Treebank
  training split
- Vanilla Viterbi decoding (~89% test accuracy)
- Modified Viterbi variants that back off for unknown words (rule-based and
  probability-weighted), improving accuracy on unseen tokens
- Error analysis comparing the variants

## Running it

```bash
pip install nltk numpy pandas
jupyter notebook HMM_based_POS_tagging.ipynb
```

The Treebank corpus downloads via `nltk.download()` inside the notebook.

## License

MIT — see [LICENSE](LICENSE).
