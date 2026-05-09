
# train

```sh
# tiny — fast, good for testing ideas (~5 min on M3 Pro)
uv run train.py --n_layer 2 --n_head 2 --n_embd 128

# small — good for quick experiments (~20 min)
uv run train.py --n_layer 4 --n_head 4 --n_embd 256

# medium — default, best results on Shakespeare (~45 min)
uv run train.py --n_layer 6 --n_head 6 --n_embd 384
```

# generate

```sh
uv run generate.py checkpoint_final.pt --prompt "To be or not" --seed 42

# example submission command
uv run generate.py checkpoint_final.pt --prompt "The morning sun" --temperature 0.7 --top_k 30 --seed 42
```
