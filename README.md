# server

[![style: very good analysis][very_good_analysis_badge]][very_good_analysis_link]
[![License: MIT][license_badge]][license_link]
[![Powered by Dart Frog](https://img.shields.io/endpoint?url=https://tinyurl.com/dartfrog-badge)](https://dartfrog.vgv.dev)

An example application built with dart_frog

[license_badge]: https://img.shields.io/badge/license-MIT-blue.svg
[license_link]: https://opensource.org/licenses/MIT
[very_good_analysis_badge]: https://img.shields.io/badge/style-very_good_analysis-B22C89.svg
[very_good_analysis_link]: https://pub.dev/packages/very_good_analysis


reference: https://blog.codemagic.io/writing-your-backend-in-dart/





Create empty flutter project then run in terminal:
dart pub global activate dart_frog_cli

(if you get zsh: command not found: dart_frog
Do these steps:
Set path for zsh on Mac:

Run vim ~/.zshrc
Press i
Paste export PATH="$PATH":"$HOME/.pub-cache/bin"
Press esc
Type :wq! and press enter
Restart the terminal)

if not go forward with this next step:

dart_frog create --project-name server .


And the result will be as follows:
├── .dart_tool
├── routes
│    └── index.dart
├── test
│    └── routes_test.dart
│       └── index_test.dart
├── .dockerignore
├── .gitignore
├── analysis_options.yaml
├── pubspec.lock
├── pubspec.yaml
└── README.md


To start our server, we just need to use another Dart Frog CLI command:
dart_frog dev

now open another terminal
curl http://localhost:8080
We can now see a message saying, “Welcome to Dart Frog!”