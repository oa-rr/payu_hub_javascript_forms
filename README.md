# Collecting Card Information - JavaScript Forms - PayU Hub

## Installation

- OPTIONAL: Create a [virtual environment](https://pypi.org/project/nodeenv/) with the command
    #### Local installation
    Linux/Mac 
    ```virtualenv venv```

- OPTIONAL: Activate the virtual environment:

    Linux/Mac ```. venv/bin/activate``` and `deactivate` to exit

    It should appear (venv) in the console. Whenever a new console is executed, the virtual machine has a libraries and dependencies other than those found in the normal Windows environment, this to maintain the integrity of the applications in the operating system.

- MANDATORY for creating local python server:

    * Download and install Python https://www.python.org/downloads/ or 
    
    run for MAC OS `brew install python`

    run for WINDOWS OS, from PowerShell as admin
        1. `@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"`
        2. `choco install -y python3`
        3. `python --version`

- MANDATORY if want to run tests having a valid SSL certificate:

    * Sign up on https://ngrok.com/
    * Download ngrok
    * Connect your local machine with your ngrok account by running: 
        `ngrok authtoken YOUR_NGROK_TOKEN` or see instructions on https://ngrok.com/
        
        Note: you should be able to get your ngrok authentication token from https://ngrok.com/

## Execution

- On the folder path of the project run `python3 -m http.server` or `python -m http.server`

    Note: this will create a local server on your machine, please check the `PORT` number in which the server is running, you will needed for the next step.

- On a different path exececute `ngrok http PORT`, for example `ngrok http 8000`


## Documentation

- [Setting up PaymentsOS](https://developers.paymentsos.com/docs/getting-started/setting-up-paymentsos.html) you need to create a business unit in your paymentsos account for testing.

- [Finding a Provider](https://developers.paymentsos.com/docs/connect/finding-a-provider.html)

- [Collecting Card Information](https://developers.paymentsos.com/docs/getting-started/collecting-card-information.html)

- [Javascript API Reference](https://developers.paymentsos.com/apis-and-sdks/client-library-references/javascript-api-reference.html)

- [Secure Fields Form Reference](https://developers.paymentsos.com/apis-and-sdks/client-library-references/securefieldsreference.html)

- [Secure CVV Form Reference](https://developers.paymentsos.com/apis-and-sdks/client-library-references/securecvvreference.html)
