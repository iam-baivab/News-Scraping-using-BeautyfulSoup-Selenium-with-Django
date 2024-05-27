# News-Scraping-using-BeautifulSoup-Selenium-with-Django

[![Apache 2.0 License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

## Table of Contents
1. [About The Project](#about-the-project)
2. [Features](#features)
3. [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
4. [Usage](#usage)
5. [Changelog](#changelog)
6. [Contributing](#contributing)
7. [License](#license)
8. [Contact](#contact)
9. [Acknowledgements](#acknowledgements)

## About The Project

This project automates the process of scraping news articles from various sources using BeautifulSoup and Selenium, integrated into a Django application. It supports multiple websites and can run scraping tasks concurrently using threading. The data is stored in an Excel file and optionally in a MySQL database.

## Features

- Scrapes news articles from Hindustan Times, Hindustan Times Bangla, Zee News, TV9 Bangla, and Ananda Bazar.
- Concurrent scraping using threading with a delay between iterations.
- Supports both on-demand scraping and scheduled scraping tasks.
- Saves scraped data to Excel files and a MySQL database.
- Creates a new folder for data storage based on the current date.

## Getting Started

To get a local copy up and running, follow these steps.

### Prerequisites

- Python 3.6+
- Django 3.0+
- Selenium
- BeautifulSoup
- MySQL (for database storage)

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/iam-baivab/News-Scraping-using-BeautifulSoup-Selenium-with-Django.git
    ```
2. Navigate to the project directory:
    ```sh
    cd News-Scraping-using-BeautifulSoup-Selenium-with-Django
    ```
3. Install required Python packages:
    ```sh
    pip install -r requirements.txt
    ```
4. Set up the Django project:
    ```sh
    python manage.py migrate
    python manage.py createsuperuser
    ```
5. Update the database configuration in `settings.py` if using MySQL.

## Usage

Run the Django development server:
```sh
python manage.py runserver
```

Navigate to the admin panel, configure the scraping tasks, and start the scraping process. The scraped data will be saved in the specified formats and locations.

## Changelog

### v1.0.1

- Initial release with scraping from Hindustan Times.

### v1.0.1.1

- Added scraping from Hindustan Times Bangla.

### v1.0.1.2

- Added scraping from Zee News.

### v1.0.1.3

- Added scraping from TV9 Bangla.

### v1.0.1.4

- Added scraping from Ananda Bazar.

### v2.0.1

- Dynamic scraping based on request value.

### v2.0.1.1

- Appending data to existing `scraped_data.xlsx`.

### v3.0.1

- Concurrent scraping with threading.

### v3.0.1.1

- Automatic folder creation based on current date.

### v4.0.1

- Integration with MySQL database and updated Django models.

## License

Distributed under the Apache License 2.0. See `LICENSE` for more information.

## Acknowledgements

- [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/)
- [Selenium](https://www.selenium.dev/)
- [Django](https://www.djangoproject.com/)

[license-shield]: https://img.shields.io/badge/License-Apache%202.0-blue.svg
[license-url]: https://github.com/iam-baivab/News-Scraping-using-BeautyfulSoup-Selenium-with-Django/blob/main/LICENSE
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/baivabsarkar/

---
