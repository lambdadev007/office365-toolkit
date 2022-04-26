# Outlook email verifier

## Installation
1. You need to have Python installed. If you haven't, please [download Python](https://www.python.org/downloads/) and install on your machine.
2. You need to have some packages installed. Please use the below commands to get them installed.
    ```
    pip install dnspython
    ```

## How it works
Before running the application, you need to confirm how many threads you want to run at a time.

Open `bulk-verifier.py` and update the value for `TotalNumberOfThreads`.

And then update the input files approprately.
For example, if you set the `TotalNumberOfThreads` as 3, you should set the 3 input files in the `InputFiles` array.
```
e.g.
TotalNumberOfThreads = 3
InputFiles = [
    "./input/verifier/emails_1.csv",
    "./input/verifier/emails_2.csv",
    "./input/verifier/emails_3.csv",
]
``` 

Now you can execute the bulk fetcher by running command `python bulk-verifier.py` or directly execute by mouse double click on the bulk-fetcher.py.

It will save the result in the `results/verifier` directory.