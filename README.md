<!-- PROJECT HEADER -->
<div align="center">
  <!-- <img src="docs/img/logo.png" alt="Logo" width="80" height="80">
  --><h3 align="center">API Central</h3>

  <p align="center">
    Node.js RESTful API that provides management and access to different APIs, handling authentication and permissions.
    <br />
    <a href="https://github.com/ThomasLvll/API-Central"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/ThomasLvll/API-Central">View Demo</a>
    ·
    <a href="https://github.com/ThomasLvll/API-Central/issues">Report Bug</a>
    ·
    <a href="https://github.com/ThomasLvll/API-Central/issues">Request Feature</a>
  </p>
</div>



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
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li>
      <a href="#documentation">Documentation</a>
      <ul>
        <li><a href="#api">API</a></li>
        <li><a href="#permissions">Permissions</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
      <ul>
        <li>
	  <a href="#api-usage-flow">API Usage Flow</a>
          <ol>
            <li><a href="#1-register-into-api">Register into API</a></li>
            <li><a href="#2-request-an-api-token">Request an API token</a></li>
            <li><a href="#3-call-the-api">Call the API</a></li>
          </ol>
      </ul>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

API Central is a Node.js API that aims to simplify access and authentication management of many APIs.

Here's a blank template to get started: To avoid retyping too much info. Do a search and replace with your text editor for the following: `github_username`, `repo_name`, `twitter_handle`, `linkedin_username`, `email_client`, `email`, `project_title`, `project_description`

### Built With

* [Node.js](https://nodejs.org/)
* [MongoDB](https://mongodb.com/)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* npm
  ```sh
  npm install npm@latest -g
  ```

### Installation

1. Get a free API Key at [https://example.com](https://example.com)
2. Clone the repo
   ```sh
   git clone https://github.com/ThomasLvll/API-Central.git
   ```
3. Install NPM packages
   ```sh
   npm install
   ```
4. Enter your API in `config.js`
   ```js
   const API_KEY = 'ENTER YOUR API';
   ```

<p align="right">(<a href="#top">back to top</a>)</p>



## [Documentation](docs)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

### API Usage Flow

#### 1. Register into API

___This step only should be performed once.___

You can sign up and subscribe to API through Central web interface.



#### 2. Request an API token

___This step should be repeated each time the token expires.___

You can do so by making a `GET /token` HTTP request to API, passing the client ID and secret keys returned in previous step as `Authorization` HTTP request header.

The header must strictly match the following format:
```
Authorization: Bearer <authToken>
```

where `authToken` is a __base64-encoded__ string in this format:
```
<clientId>:<clientSecretHash>:<listOfPermissions>
```
where `clientId` obviously is your client ID key, and `clientSecretHash` is a hash of your client secret key. Supported hashing methods are the following:
* MD5
* SHA1

`listOfPermissions` parameter is a comma-separated list of [permissions](#permissions) you want your API token to own.

The HTTP request finally looks like:
```
GET /token
Authorization: Bearer af456zjk54...
```

In case of success, the JSON response body has the following form:
```json
{
	"apiToken": "kl593fkfd240...",
	"expirationDate": "2022-04-26 17:10:25.230 +00:00",
	"refreshUrl": "https://example.com/token/refresh/kl593fkfd240..."
}
```



#### 3. Call the API

Once your API token has been obtained, you can make requests to [endpoints of the API](#api-endpoints).

Even if not all paths require an authorization, it is recommended to always include API token in your requests. It must be passed as `Authorization` HTTP request header, strictly matching the following format:
```
Authorization: Bearer <authToken>
```

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [ ] Feature 1
- [ ] Feature 2
- [ ] Feature 3
    - [ ] Nested Feature

See the [open issues](https://github.com/github_username/repo_name/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the [GNU GPLv3](https://choosealicense.com/licenses/gpl-3.0/) License. See [`COPYING`](COPYING) for more information.

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Thomas Léveillé - leveille.thomas77@gmail.com

Project Link: [https://github.com/ThomasLvll/API-Central](https://github.com/ThomasLvll/API-Central)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* []()
* []()
* []()

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/ThomasLvll/API-Central.svg?style=for-the-badge
[contributors-url]: https://github.com/ThomasLvll/API-Central/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/ThomasLvll/API-Central.svg?style=for-the-badge
[forks-url]: https://github.com/ThomasLvll/API-Central/network/members
[stars-shield]: https://img.shields.io/github/stars/ThomasLvll/API-Central.svg?style=for-the-badge
[stars-url]: https://github.com/ThomasLvll/API-Central/stargazers
[issues-shield]: https://img.shields.io/github/issues/ThomasLvll/API-Central.svg?style=for-the-badge
[issues-url]: https://github.com/ThomasLvll/API-Central/issues
[license-shield]: https://img.shields.io/github/license/ThomasLvll/API-Central.svg?style=for-the-badge
[license-url]: https://github.com/ThomasLvll/API-Central/blob/master/LICENSE.txt

[portfolio-shield]: https://img.shields.io/badge/-Portfolio-important.svg?style=for-the-badge
[portfolio-url]: http://thomasleveille.com
[product-screenshot]: docs/img/screenshot.png
