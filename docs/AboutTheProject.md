Possible Project Ideas:
Food Nutrition Detector

Where can we find datasets:
Kaggle
Hugging Face
Perplexity
Arxiv

Available dataset:
https://github.com/google-research-datasets/Nutrition5k
https://huggingface.co/datasets/TeeA/nutrition5k-food-name-gemini


Voxel Food Nutrition Detector
GitHub [Link]
Colab [Link]


Voc, coco, image classification directory tree


Nutritional facts
https://www.kaggle.com/datasets/trolukovich/nutritional-values-for-common-foods-and-products


First Slide: 
Problem Statement: 
Millions of people worldwide have dietary restrictions due to health conditions such as diabetes, food allergies, celiac disease, or chronic kidney disease. These individuals must carefully monitor their intake of specific nutrients and ingredients to maintain their health. However, when dining at restaurants, it is often difficult to obtain accurate and detailed nutritional information about meals, especially for those with unique dietary needs.

To address this challenge, we propose developing a computer vision-based application that allows users to take a picture of their meal and receive detailed nutritional information in real time. The application will leverage image recognition and AI-powered food analysis to estimate macronutrient and micronutrient content, detect potential allergens, and highlight ingredients that may be restricted based on the user's dietary profile.

This system will empower individuals with dietary restrictions to make informed choices about their meals, improving their ability to dine out safely and confidently.
Second Slide:
Dataset we chose and why we chose this dataset - 
Originally we wanted to go with Nutrition5k but we had limitations here because of its size 181.4GB. This dataset had a lot of great information like Per-ingredient mass and Fat, protein, and carbohydrate macronutrient masses which would have made development a bit easier if we could have figured out a way to drop the video data columns. 

There does exist a dataset on hugging face which has just dish_id, , food_name, and dish_image. So we ended up going with that. 

Through our exploration of this dataset on Voxel51, we noticed that certain images were (incorrectly?) labelled. A few of the images were blurry or had other items that got incorrectly identified. Some of datas 

Third Slide:
Model we chose

Fourth Slide:
Demonstration



