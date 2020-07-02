# 商研所碩士論文 CatBoost與LightGBM的比較

Some of the data used can be downloaded if you read the thesis and find the corresponding links.

Summary:
CatBoost tends to choose categorical features, while LightGBM uses numerical ones.
When the dataset has important numerical features, LightGBM performs better than CatBoost. But if the dataset has prominent categorical features, CatBoost tend to predict better.

Implication:
You should use CatBoost to predict if you want a better performance on common tabular medium-sized data. As for why catboost speed is much slower, I guess because Catboost preprocess categorical columns on its own, while LightGBM requires the data to be preprocessced before feeding into the model. Categorical column encoding is time consuming, and the CatBoost uses Target Encoding may be the reason why the model training speed is slow.

# Powerpoint file briefly introduce what I've done in this thesis, but mostly are in chinese, although I believe with graphics you can still understand what I'm trying to do.
