To use this repo, first clone it to your local machine using `git clone https://github.com/zhamdan1252/cs614final` then cd into the cloned directory.

Once cloned, create a venv using `python -m venv .\venv` and on a windows device run `.\venv\Scripts\activate` to activate the venv

To initialize all dependencies, run `pip install -r requirements.txt` in the command terminal. After doing this you will likely need to add these as well using the commands shown below:
    pip install torch==2.2.2+cu118 torchvision==0.17.2+cu118 torchaudio==2.2.2+cu118 -f https://download.pytorch.org/whl/torch_stable.html  

    pip install transformers

Now you should be able to run the scripts accordingly. `emotion_classifier.ipynb` takes in "llm_input.csv" as input (which should be stored in the home directory of the project) and outputs "output_results.csv" with the generated results.

`eval.ipynb` will generate confusion matrices, scoring the results according to their ability to correctly identify the classified "emotion".
