# Food Across The Globe

A data science project exploring how geography, culture, and history shape
cuisines around the world, using a dataset of ~20,000 recipes.

## Research Question
How do geography, culture, and history influence the world's cuisines?

## Dataset
[Food.com Recipes and User Interactions](https://www.kaggle.com/datasets/shuyangli94/food-com-recipes-and-user-interactions)
— recipe names, ingredients, tags, and metadata. Cuisine labels were extracted
from the `tags` column, filtered to cuisines with at least 100 labeled recipes:
American, Italian, Mexican, African, Indian, French, Greek, German, and Chinese.

## Methods
1. Loaded and cleaned the raw dataset (20,000 recipes sampled).
2. Extracted cuisine labels from tag lists.
3. Parsed ingredient lists and computed ingredient frequency per cuisine.
4. Computed pairwise Jaccard similarity between cuisines' ingredient sets.
5. Visualized results as bar charts and a similarity heatmap.

## Key Findings
- Each cuisine has a distinctive ingredient signature (e.g. garam masala/turmeric
  for Indian, soy sauce/ginger for Chinese, chili powder/cilantro for Mexican).
- American recipes had the lowest similarity to every other cuisine, likely due
  to having the largest and most varied ingredient vocabulary in the dataset.
- Mediterranean-adjacent cuisines (Italian, Greek, French) showed relatively
  higher similarity to each other than to other regions.

## Project Structure
data/raw - original dataset
data/cleaned - processed data (if saved)
notebooks/ - analysis notebooks
images/ - saved chart outputs
src/ - reusable code (future work)

## Next Steps
- Network analysis of ingredient co-occurrence
- Interactive geographic visualization