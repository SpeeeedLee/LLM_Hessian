```bash
cd ./llm-hessain-main


```


```bash
python3 src/single_layer_single_block.py \
        --model facebook/opt-125m \
        --layer_name self_attn.q_proj \
        --block_index 0 \
        --t 5 \
        --b 30 \
        --model_input_bs 1 \
        --seed 0 \
        --cache_dir llm_weights \
        --device 'cuda:0'

python3 src/single_layer_single_block.py \
        --model meta-llama/Llama-3.2-1B \
        --layer_name self_attn.q_proj \
        --block_index 0 \
        --t 5 \
        --b 30 \
        --model_input_bs 1 \
        --seed 0 \
        --cache_dir llm_weights \
        --device 'cuda:0'

```