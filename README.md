
- The main logic is in pydriller10x.ipynb. It's a Jupyter Notebook
    - Be careful about the time range, the runtime can easily surpass 10min.
    - Jupyter Notebook sometimes freezes upon exception. To debug your code, pydriller10x.py is preferred.
- The data is gathered from two sources: commit metadata, and each modified file in each commit
    - If you want to gather additional data from each modified file, you need to check out following places.
        - analyze.py return statement
        - pydriller10x.py `commit_data` column declaration
        - pydriller10x.py `modified_src_data` column declaration
        - pydriller10x.py `modified_src_data` aggregation item and default value for `stat`
        - pydriller10x.py `commit_data.append`
