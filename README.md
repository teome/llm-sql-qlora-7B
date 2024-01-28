# LLM QLoRA fine tune for Mistral-7B (any <= 7B model) for SQL Generation

Use Hugging Face [TRL](https://huggingface.co/docs/trl/index) library to train QLoRA adaptors on Mistral-7B.

Using [sql-create-context](https://huggingface.co/datasets/b-mc2/sql-create-context) dataset. Each row has a natural language instruction, a context that contains the schema of a DB and the answer as a SQL query. This is useful in lots of situations and the same approach can be applied to other DSLs or tools

Test on the evaulation set and give examples for running with inference servers