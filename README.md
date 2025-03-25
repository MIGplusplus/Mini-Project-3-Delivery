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

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Installation

1. Get a free API Key at [https://example.com](https://example.com)
2. Clone the repo
   ```sh
   git clone https://github.com/github_username/repo_name.git
   ```
3. Install NPM packages
   ```sh
   npm install
   ```
4. Enter your API in `config.js`
   ```js
   const API_KEY = 'ENTER YOUR API';
   ```
5. Change git remote url to avoid accidental pushes to base project
   ```sh
   git remote set-url origin github_username/repo_name
   git remote -v # confirm the changes
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- TROUBLESHOOTING -->
## Troubleshooting
### It's not letting me run the file!
If you cannot run the executable file (whether it be the `.exe` or the script), then this may indicate that you do not have the correct permissions for the file.

In a Linux system, you can ensure that the user has permission to execute the file by running the following command: `$ chmod +x dist/loglens`.

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
[product-screenshot]: images/screenshot.png

[Python.py]:https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54

[Python-url]:https://www.python.org/
[Pyinstaller-url]: https://pyinstaller.org/en/stable/
[Pyinstaller.py]: https://img.shields.io/pypi/v/pyinstaller