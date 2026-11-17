# Steam Game Description Generator Using GPT-2

## Project Overview
This project explores whether a pretrained GPT-2 language model can generate video game descriptions based on genre information.

## Dataset
The dataset contains 290 Steam games, including their genres and descriptions.

* Training set: 232 games (80%)
* Validation set: 58 games (20%)

## Technologies

* Python
* PyTorch
* Hugging Face Transformers
* tiktoken
* pandas
* Matplotlib
* Google Colab

## Methodology

1. Clean and preprocess game descriptions.
2. Tokenize genre prompts and descriptions.
3. Prepare training and validation DataLoaders.
4. Fine-tune pretrained GPT-2 for two epochs.
5. Evaluate training and validation loss.
6. Generate descriptions for different genre combinations.

## Model Training Results

| Epoch | Training Loss | Validation Loss |
|-------|---------------|-----------------|
| 1 | 3.7026 | 3.5972 |
| 2 | 3.5264 | 3.5802 |

## Example Input

```python
genres = "Action RPG, Mythology, Adventure"

prompt = f"Genres: {genres}\nDescription:"
```

## Example Generated Output

> About This Game A fantasy adventure set in
> the world of Dromund Kaas.

## Project Limitations

The generated descriptions occasionally contain
repetition, inconsistent grammar, or references
to existing video game franchises.

## Future Improvements

- Expand the training dataset.
- Improve text generation quality.
- Test additional genre combinations.
