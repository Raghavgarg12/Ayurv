## LLM for Ayurvedic Knowledge

This project was made for Samrt India hackathon 2023 internal hack [Problem Statement 1347].
This LLM offers Ayurvedic insights for patients and doctors.

* **Powered by privateGPT:** Ensures data confidentiality. Works on your local machine without internet.
* **Patient-friendly language:** Easy to understand.
* **Supports doctors:** Research, treatment options, patient insights.
* **Quotes sources:** Information can be verified from books.
  
**Disclaimer:** Information only, consult a qualified Ayurvedic practitioner or doctor for diagnosis and treatment.

Built with [LangChain](https://github.com/hwchase17/langchain), [GPT4All](https://github.com/nomic-ai/gpt4all), [LlamaCpp](https://github.com/ggerganov/llama.cpp), [Chroma](https://www.trychroma.com/) and [SentenceTransformers](https://www.sbert.net/).

![image](https://github.com/Raghavgarg12/Ayurv/assets/97753861/cd7dd02c-9fb9-40a4-85e0-d2794e9b6aaa)

## Environment Setup
In order to set your environment up to run the code here, first install all requirements:

```shell
pip3 install -r requirements.txt
```
Then, download the LLM model and place it in a directory of your choice:
- LLM: default to [ggml-gpt4all-j-v1.3-groovy.bin](https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin). If you prefer a different GPT4All-J compatible model, just download it and reference it in your `.env` file.

## Ask questions to your documents, locally!
In order to ask a question, run a command like:

```shell
python privateGPT.py
```

And wait for the script to require your input.

```plaintext
> Enter a query:
```

Hit enter. You'll need to wait 20-30 seconds (depending on your machine) while the LLM model consumes the prompt and prepares the answer. Once done, it will print the answer and the 4 sources it used as context from your documents; you can then ask another question without re-running the script, just wait for the prompt again.

Note: you could turn off your internet connection, and the script inference would still work. No data gets out of your local environment.

Type `exit` to finish the script.
