```shell
pip install -r requirements.txt
```
### Download the experimental data

```shell
./download.sh
```



## Sanitize the text inputs

We propose two sanitized mechanisms based on differential privacy: **SanText** and **SanText+**.
Here we show some examples for running these algorithms:
```shell
 python run_SanText.py \
  --task SST-2 \
  --method SanText \
  --epsilon 3.0 \
  --word_embedding_path ./data/glove.840B.300d.txt \
  --word_embedding_size 300 \
  --data_dir ./data/SST-2/ \
  --output_dir ./output_SanText_glove/SST-2/ \
  --threads 8 
```
