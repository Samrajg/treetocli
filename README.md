TreeToCLI

From Tree View to Terminal in Seconds

TreeToCLI is a web-based tool designed to streamline the process of generating terminal commands from folder structures across multiple platforms. It is ideal for developers, automation engineers, DevOps professionals, and students who want to save time and improve workflow efficiency by quickly converting a project’s folder tree into ready-to-run commands for Linux, macOS, Windows CMD, or Windows PowerShell.

Features

Cross-Platform Support: Generate commands for Linux, macOS, Windows CMD, and PowerShell.

Dynamic Folder Parsing: Detects directories and files, understands indentation, and converts tree structures into accurate commands.

Color-Coded Output: Directories and files are visually distinguished in the output for easy readability.

Copy & Download: Copy the generated commands to the clipboard or download as an executable script (.sh, .bat, .ps1) ready for immediate use.

SaaS-Like UI: Modern dark/glass interface with smooth transitions, light/dark theme toggle, and intuitive controls.

Template Management: Save your folder structures in the browser and reload them anytime.

Drag & Drop Support: Paste or drag your folder tree from a text file for instant command generation.

Example Templates: Preloaded example structures for quick testing and experimentation.

Responsive Design: Works perfectly on desktops, laptops, and tablets.

Demo

You can test TreeToCLI directly in your browser:

Live Demo: [Insert your GitHub Pages / live link here]

Getting Started

These instructions will help you get a local copy of TreeToCLI up and running for development and testing purposes.

Prerequisites

A modern web browser (Chrome, Firefox, Edge, Safari).

No backend required for Phase 4 – all processing is done in-browser.

Installation

Clone the repository:

git clone https://github.com/Samrajg/TreeToCLI.git

Navigate to the project folder:

cd TreeToCLI

Open the frontend:

Simply open index.html in your browser.

No additional setup is required.

Usage

Paste or drag your folder tree into the textarea.

Select your operating system:

Linux / macOS

Windows CMD

Windows PowerShell

Click Generate to create terminal commands.

Copy the commands to your clipboard or Download them as a script.

Optionally, Save Templates for future use or Load Template to reuse saved folder structures.

Example Usage

Paste the following tree in the textarea for testing:

project/
 ├── backend/
 │    ├── main.py
 │    └── requirements.txt
 ├── frontend/
 │    └── index.html
 └── README.md

The generated commands for Linux will be:

mkdir -p "project/backend"
touch "project/backend/main.py"
touch "project/backend/requirements.txt"
mkdir -p "project/frontend"
touch "project/frontend/index.html"
touch "project/README.md"

For Windows CMD, it will generate:

mkdir "project\backend"
type nul > "project\backend\main.py"
type nul > "project\backend\requirements.txt"
mkdir "project\frontend"
type nul > "project\frontend\index.html"
type nul > "project\README.md"

And for PowerShell:

New-Item -ItemType Directory "project\backend"
New-Item -ItemType File "project\backend\main.py"
New-Item -ItemType File "project\backend\requirements.txt"
New-Item -ItemType Directory "project\frontend"
New-Item -ItemType File "project\frontend\index.html"
New-Item -ItemType File "project\README.md"
Features in Depth

Indentation Detection: Automatically detects nested directories, even with mixed spaces or tabs.

Directory vs File Identification: Correctly distinguishes between directories (ending with /) and files.

Interactive UI: Commands are color-coded (directories in cyan/blue, files in yellow/orange) for clarity.

Template System: Users can save multiple templates locally, making it easier to reuse recurring project structures.

Drag & Drop: Supports dropping a .txt file containing a folder tree to instantly generate commands.

SaaS-Like Design: Smooth animations, responsive layout, and modern glass effects.

Contributing

Contributions are welcome! To contribute:

Fork the repository.

Create a new branch:

git checkout -b feature-name

Make your changes and commit:

git commit -m "Add feature XYZ"

Push to your branch:

git push origin feature-name

Open a Pull Request.

Roadmap

Phase 5: Multi-user SaaS, cloud storage for templates, shareable links.

Phase 6: Full SaaS production-ready platform, authentication, marketplace, collaboration.

Built With

HTML5 / CSS3 / JavaScript – Frontend implementation

LocalStorage – Template persistence

GitHub Pages – Hosting (optional)

Authors

Godwin Samraj – Developer & Project Creator

License

This project is licensed under the MIT License – see the LICENSE file for details.

Acknowledgments

Inspiration from common developer pain points with folder structures.

Thanks to GitHub Pages for free hosting.

Special thanks to the open-source community for CSS and JS utilities.
