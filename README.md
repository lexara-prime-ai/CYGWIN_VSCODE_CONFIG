## Integrating CygWin Terminal with Visual Studio Code

**CygWin** can be seamlessly integrated with Visual Studio Code using **Terminal Profiles**. Follow the steps below to set up a new profile for CygWin.

1.  **Create a New Terminal Profile**: Add the following configuration to your existing Visual Studio Code settings to create a CygWin profile:
    
```json
  "terminal.integrated.profiles.windows": {
        "Cygwin": {
            "path": "C:\\cygwin64\\bin\\bash.exe",
            "args": [
                "--login"
            ],
            "env": {
                "CHERE_INVOKING": "1"
            }
        }
 }
 ``` 
    
2.  **Note**:
    
    -   This configuration example uses the **64-bit** version of CygWin.
    -   Ensure that the path to `bash.exe` matches your CygWin installation directory.
