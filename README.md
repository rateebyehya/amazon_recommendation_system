# Building Amazon Recommendation System for 25K Products

## Introduction 

Hello everyone, 

I am excited to share the details of a project my team and I developed as part of the Amazon Hackathon challenge organized for UCLA MSBA students in the Fall of 2022. The challenge required us to build a recommendation system for products using a dataset containing 25,000 products and 26 features. 

## Data 

The dataset consists of 25,000 rows and 26 features, owned by Amazon. The columns are: 

- product id 
- brand 
- bullet_point 
- color 
- item_id 
- item_name
- model_name 
- model_number 
- model_year 
- product_type 
- style 
- item_keywords 
- country 
- marketplace 
- item_weight 
- material 
- fabric_type 
- product_description 
- pattern 
- finish_type 
- item_shape
- item_height
- item_length 
- item_width 
- cleaned_description 
- product_category

## Approach 

Our team decided to approach the problem by leveraging the power of APIs and natural language processing techniques to provide users with a list of complementary products for any given product input. Here is a brief overview of what we did: 

1) We used ChatGPT APIs to generate a list of complementary products based on the product type. 
2) We then mapped these complementary product types back to our existing dataset and narrowed our search to these products only 
3) We then used NLP to tokenize the words of all complementary products based on our product descriptions, item_keyowords, and other relevant string columns. 
4) We then calculated the cosine similarity scores between the tokenized complementary products and our input product.
5) Finally, we outputted the top 10 complementary products based on the cosine similarity scores. 

## Conclusion 

Our recommendation system performed well in terms of accuracy and speed, and we believe it has the potential to be further improved with additional features and optimizations. 

## Data Restrictions 

Because the data is sourced from Amazon, I will not be able to share the notebook. However, I have attached a demo video which we have presented to the Senior Analytics Insights Manager at Amazon during our final presentation. 

## Interview Tips 

In one of my interviews for a data science position at a healthcare company, I was asked why I used cosine similarity score instead of other scores. Pause for a second and think about why cosine similarity is commonly used in NLP. 
