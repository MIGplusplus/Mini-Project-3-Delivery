# Mini-Project-3-Delivery

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage examples">Usage</a></li>
    <li><a href="#troubleshooting">Troubleshooting</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

The original application, `loglens` was programmed by our Professor `Dr. Eric Rapos`,  it functions as a log analysis and monitoring tool. It processes log files, applies filters, generates statistics, and produces reports to help users understand and monitor system health or identify issues. Key features include:

- Filtering: By date range, severity level, or patterns (using regex).
- Analysis: Extracts metrics like severity counts, error rates, and common terms.
- Alerts: Detects and notifies when error rates exceed user-defined thresholds.
- Reports: Generates customizable reports in text or CSV format.


Our goal, was to package and deliver the program sucessfully to users using an Appropriate Packaging Method of our choosing. After careful consideration, we chose to use `pyinstaller` over `virtualenv` due to its relative straightforward approach -> simply download the `loglens.exe` file or on linux/mac the scrip file to run the application. With Virtual Environment, it would need a python interpreter downloaded initially in order to set up on a given user's machine. 


<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With

* [![Python][Python.py]][Python-url]
* [![Pyinstaller][Pyinstaller.py]][Pyinstaller-url]


<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

Instructions on how to setup the program locally on your machine. 

### Installation

1. Obtain the Program:
   -  From this github repository, you will need to download the necessary file in order to run the program.
2. **Operating System** Specific:
   - Navigate to the `EXPORTS` folder, and Identify what OS your machine is running. 
     - **Windows:** download the entire `windows` folder
     - **Linux:** download the entire `linux` folder
3. Once the folder is downloaded, the executable file will be situtated inside `dist/`. Be sure to note where this is located.
  
4. Run the Program:
   - Refer to the <a href="#Usage">Usage</a> section for further instructions
   

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage
Once the program is installed (make sure to follow all the instructions in the <a href="#installation">Installation</a> section), using it is very simple.

Ensure that you have the `dist` and `build` folders together, as well as a log file (such as the provided `python-example-log.txt`). 

To execute the program, one simply has to run the executable located in the `dist` folder, and provide the log file as a command-line argument:

- Open a terminal or command prompt.
   - Use the following command to run the program:
   
      ```sh
      dist/loglens <log_file>
      ```
      
   - Make sure you use the correct path to the `loglens` path.s
   - Replace `<log_file>` with the path to your log file and specify additional options as needed (refer to the usage guide below). 
   - **Additionally**, theres a provided example log file titled `python-example-log.txt` if the user wishes to test it out beforehand. 

- For example:
  ```
  $ dist/loglens python-example-log.txt
  ```

- Or, if you cloned the entire repository:

  ```
  $ EXPORTS/linux/dist/loglens EXPORTS/linux/python-example-log.txt
  ```

Similarly, the `.exe` file will need to be run through a command line in Windows systems as well.

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- TROUBLESHOOTING -->
## Troubleshooting
### It's not letting me run the file!
If you cannot run the executable file (whether it be the `.exe` or the script), then this may indicate that you do not have the correct permissions for the file.

In a Linux system, you can ensure that the user has permission to execute the file by running the following command:
```
$ chmod +x dist/loglens
```

In a Windows system, the permissions work differently. As the file is an executable (`.exe`), it should be able to natively run. If it does not, then try right-clicking and running it as an administrator. If this does not work, one should right-click on the file, click `Properties` (or alternatively, use the `Alt+Enter` shortcut), and then check the permissions under the 'Security' tab. 

### The app is immediately closing!
If—upon running it—the app opens up a terminal window that immediately closes, then this means that it was probably run incorrectly.

The file has to be run through the terminal, and a log file has to be provided as a command-line argument.

Please make sure to re-read the <a href="#usage">Usage instructions</a> for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTRIBUTING -->
## Contributing


### Contributors:
- Hayden Robinson
- Miguel Dela Torre
- Nooh Alavi
- Shawn Xiao

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- LICENSE -->
## License

Distributed under the MIT license. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[Python.py]:https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54

[Python-url]:https://www.python.org/
[Pyinstaller-url]: https://pyinstaller.org/en/stable/
[Pyinstaller.py]: https://img.shields.io/pypi/v/pyinstaller