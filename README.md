# Local Ollama Docker setup

🎯 Overview
-----------

This project contains instructions on how to locally run Ollama together with Ollama WebUI.

📦 Requirements
----------------

In order to be able to create Weaviate one needs at least.

1. Docker


💡 Running using Docker compose
-------------------------------

In order to run the setup locally running only docker compose use this comman to run the environment:

```sh
docker compose up -d
```

In order to pull ollama models issue:

```sh
docker exec -i ollama ollama pull <model_name>
```

for example if you want to download a latest multilingual large language model from Cohere - Aya issue:

```sh
docker exec -i ollama ollama pull aya
```

more models can be found using [Ollama library](https://ollama.com/library) site.

Ollama WebUI will start woking on port `8080`, just type `localhost:8080` in your browser. Please note that at the very first login attempt you would need to create an account with which you can then login to Ollama WebUI.
