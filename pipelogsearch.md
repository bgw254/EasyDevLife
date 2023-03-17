When working with command line interfaces, it is often necessary to search for specific text in the logs of a command. The following `mac pipe` commands can be used to search for text in the log outputs of a command:

1. **grep command**: The `grep` command is a powerful and widely used command-line utility that searches for patterns in files or input. To search for a specific text in the logs, use the following command:
    
    ```
    command | grep "text"
    
    ```
    
    Replace `command` with the command you want to search in the logs, and `text` with the text you want to search for.
    
2. **awk command**: The `awk` command is another powerful utility that can be used to search for specific text in the logs. To search for text using `awk`, use the following command:
    
    ```
    command | awk '/text/ {print}'
    
    ```
    
    Replace `command` with the command you want to search in the logs, and `text` with the text you want to search for.
    
3. **sed command**: The `sed` command is a stream editor that can perform various functions on the input stream. To search for text using `sed`, use the following command:
    
    ```
    command | sed -n '/text/p'
    
    ```
    
    Replace `command` with the command you want to search in the logs, and `text` with the text you want to search for.
    

These are some of the `mac pipe` commands that can be used to search for specific text in the logs of a command. Depending on your requirements, you can choose the command that best suits your needs.