## Outlook ruling automation

### Installation
1. You need to have Python installed. If you haven't, please [download Python](https://www.python.org/downloads/) and install on your machine.
2. You need to have some packages installed. Please use the below commands to get them installed.
    ```
    pip install selenium
    ```
    ```
    pip install webdriver-manager
    ```
    ```
    pip install mysql-connector-python
    ```
    ```
    pip install python-dotenv
    ```
3. Lastly, you need to setup environment variables.
    - Create **.env** file and copy the content from **.env.example** file.
    - Add the environment variables in the **.env** file.
        ```
        DB_HOST="0.0.0.0"
        DB_USER="root"
        DB_PASSWORD="xxxxxxx"
        DB_DATABASE="logs"
        DB_TABLE="office365"
        ```

### How it works
Before running the application, you need to confirm how many threads you want to run at a time.

Open ```bulk-ruler.py``` and update the value for ``` TotalNumberOfThreads ```


Now you can execute the bulk fetcher by running command ```python bulk-ruler.py``` or directly execute by mouse double click on the bulk-ruler.py.

It will start adding rules as fetching/updating entires from the remote database.