# Praetexo

Praetexo is an extremely lightweight CSS only framework that offers a responsive 12 column grid and navbar.

Note that this project is still in its early stages and so may not yet provide complete/full functionality. We will be building up functionality over the next few months through numerous small iterative releases.

## Table of Contents
- [Praetexo](#praetexo)
  - [Table of Contents](#table-of-contents)
  - [About The Project](#about-the-project)
    - [Features](#features)
  - [Getting Started](#getting-started)
    - [Installation](#installation)
    - [Import Package](#import-package)
  - [Usage](#usage)
  - [Roadmap](#roadmap)
  - [Contributing](#contributing)
  - [License](#license)
  - [Contact](#contact)
  - [Limitation of Liability](#limitation-of-liability)

## About The Project

Praetexo is designed to be a very lightweight CSS only (no JavaScript) framework that is intended as an almost drop-in replacement for Bootstrap.

### Features
- Extremely lightweight
- CSS only, no JavaScript
- 12 column responsive grid
- Navigation bar


## Getting Started

Add the package as a dependency.

### Installation
Add the package to your dependencies.

```
npm install praetexo
```

### Import Package

Import the library in your code.

```html
<link rel="stylesheet" href="praetexo.css">
```

### Example HTML

```html
<!DOCTYPE html>
<html>
<head>
    <title>Site Name</title>
    <link rel="stylesheet" href="../dist/praetexo.css">
</head>
<body>
    <div class="container">
        <nav>
            <a class="page-title" href="#">Site Name</a>
            <label for="menu" tabindex="0">
                <span></span>
                <span></span>
                <span></span>
            </label>
            <input id="menu" type="checkbox" />
            <ul>
                <li><a href="#">Mastodon</a></li>
                <li><a href="#">Twitter</a></li>
                <li><a href="#">Github</a></li>
            </ul>
        </nav>
        <main>
            <div class="row">
                <div class="col-12 text-center">
                    <h1>Hello</h1>
                    <h3>Some or other byline goes here.</h3>
                </div>
            </div>
            <div class="row">
                <div class="col-4">
                    <h2>Blaherty 1</h2>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur eu augue consequat, ...</p>
                </div>
                <div class="col-4">
                    <h2>Blaherty 2</h2>
                    <p>Quisque et blandit risus. Praesent diam dolor, tempus scelerisque orci a, ...</p>
                </div>
                <div class="col-4">
                    <h2>Blaherty 3</h2>
                    <p>Etiam sed nisi a massa varius elementum. Nam mollis est leo, ...</p>
                </div>
            </div>
        </main>
        <footer>
            <div class="row footer">
                <div class="col-6">
                    Copyright 2024 Acme Corp.
                </div>
                <div class="col-6 right">
                    <a href="#">Privacy Policy</a>
                </div>
            </div>
        </footer>
    </div>
</body>
</html>
```

## Usage

See the [User Guide](doc/user-guide.md) for detailed information.

## Roadmap

See the [open issues](https://github.com/Limeslice-Software-Foundation/praetexo/issues) for a full list of proposed features (and known issues).


## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


## License

Distributed under the MIT License. See `LICENSE` for more information.


## Contact

Limeslice Software Foundation [https://limeslice.org](https://limeslice.org)


## Limitation of Liability

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.