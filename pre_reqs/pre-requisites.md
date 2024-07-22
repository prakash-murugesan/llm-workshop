# Unlocking the Power of LLMs for Customizable Problem-Solving

## Pre-Requisites

### Python SetUp

To ensure a smooth experience, please make sure you have Python 3.9 and the latest version of pip installed on your system.

The setup process consists of four steps, which can be completed either directly in your IDE or via the terminal. Below, we will guide you through the steps using the terminal. If you prefer to use your IDE, please refer to its documentation for instructions.


**Step 1: Clone the GitHub Repository**

```{SSH}
$ git clone git@github.com:cgamamx/llm-workshop.git
$ cd llm-workshop
```

**Step 2: Install Virtual Environment and Activate it**
   
Install `virtualenv`, create a new virtual environment named `venv`, and activate it. Note that depending on your installation, you may need to use `pip` instead of `pip3` for this step:


```{SSH}
$ pip3 install virtualenv
$ virtualenv venv
$ source  venv/bin/activate
```
   
**Step 3: Install Required Libraries**

Install the libraries listed in the requirements.txt file. Make sure your virtual environment is active.


```{SSH}
(venv) $ pip install -r requirements.txt
```

**Step 4: Configure Your IDE** 

Finally, follow the steps specific to your IDE to use the newly created Python environment. Please refer to your IDE's documentation for instructions on how to do this.

### Ollama setup: 

**Step 1. Download and install Ollama**

**Mac or Windows:**
1. Go to the [Ollama download page](https://ollama.com/download) and select your platform to download the installer.
2. Double-click the downloaded file, and follow the instructions to install Ollama.

**Linux:**

1. Open a terminal and run the following command to download and install Ollama:

```
$ curl -fsSL https://ollama.com/install.sh | sh
```

**Step 2: Download and Test Llama3**

1. Open a terminal or console and run the following command to download the Llama3 8b model (4-bit quantized, ~4.7 GB):

```
$ ollama pull llama3
```

2. (Optional) Run the following command to download the Llama3 70b chat model (4-bit quantized, ~39 GB):

```
ollama pull llama3:70b
```

3. Run the following command to test Llama3:

```
ollama run llama3
```

Ask Llama3 questions, such as "who wrote the book godfather?" or "who wrote the book godfather? answer in one sentence."

*Note: If you completed step 2 then you can also try running `ollama run llama3:70b`, but the inference speed may be too slow (e.g., over 10 seconds to generate one token on an Apple M1 Pro with 32GB RAM).*
