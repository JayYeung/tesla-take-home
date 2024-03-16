## Requirements

Jay used Python 3.11.8. Using Python 3.12.1 led to conflicts with `langchain`. It is recommended to use `pyenv` to manage Python versions.

```bash
git clone https://github.com/JayYeung/tesla-take-home.git
cd tesla-take-home
```

```bash
pip install -r requirements.txt
```

## Running the scripts (Preqrequisite: OpenAI API Key)

Add `OPENAI_API_KEY` to your environment (bash, zsh, etc.):

1. Navigate to [OpenAI Platform](https://platform.openai.com/api-keys) and create an API key and set up billing payments if you haven't.
2. Copy and paste it into your environment config (`~/.bashrc`, `~/.zshrc`, etc.) by writing `export OPENAI_API_KEY='{copied API key}'` with the single quotation marks.
3. Execute the commands in your config file by running `source ~/.bashrc` or `source ~/.zshrc`. This will allow scripts, like Python ones, to access your OpenAI API key without revealing it or pushing it to GitHub. It sort of acts like a **secret** but other people can of course still see your API key if they look at your config files.

Now, you can run Python scripts to use your OpenAI API key to use Langchain.

## Running the scripts

Open `langchain.ipynb` in Jupyter Notebook and run the cells. Testcases can be inputted through the `testcase/` folder and output will be saved in the `output/` folder.
