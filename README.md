### To replicate perform the following steps:
- Clone the repo
- Run `pip install -r requirements.txt` in your virtual environment.
- To test the application run:
    ```
    python3 drag_drop.py
        or 
    python drag_drop.py
    ```
- If you are experiencing this kind of error:
    ```
    from matplotlib import ft2font: “ImportError: DLL load failed: The specified procedure could not be found.”
    ```
    - Then first uninstall the matplotlib using:
        ```pip3 uninstall matplotlib```
    - Install the Microsoft Visual C Runtime:
        ```pip3 install msvc-runtime```
    - Then install the matplotlib:
        ```pip3 install --upgrade matplotlib```

- To compile a standalone exe file from the code:
    - Install pyinstaller 
    ```pip install pyinstaller```
    - Run the following command:
    ```pyinstaller --onefile --windowed drag_drop.py```


    Note: Make sure you have PyQt version 5.15.3 installed. Otherwise you will get this error with pyinstaller
    ```
    AttributeError: Module 'PyQt5' has no attribute '__version__'
    ```

