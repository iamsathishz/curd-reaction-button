[![pub package](https://img.shields.io/pub/v/curd_reaction_button.svg)](https://pub.dartlang.org/packages/curd_reaction_button)

# Flutter reaction button

Flutter Reaction Button is a customizable Flutter package that allows you to easily create interactive buttons with reaction emojis, similar to Facebook's iconic reaction buttons.


## Screenshot

![App Screenshot](https://raw.githubusercontent.com/GeekAbdelouahed/flutter-reaction-button/master/images/curd_reaction_button_preview.png)


## Installation

```yaml
# pubspec.yaml
dependencies:
  flutter:
    sdk: flutter
  curd_reaction_button: <last-version>
```
## Usage

```dart
import 'package:curd_reaction_button/curd_reaction_button.dart';

ReactionButton<String>(
    onReactionChanged: (Reaction<String>? reaction) {
        debugPrint('Selected value: ${reaction?.value}');
    },
    reactions: <Reaction<String>>[
        Reaction<String>(
            value: 'like',
            icon: widget,
        ),
        Reaction<String>(
            value: 'love',
            icon: widget,
        ),
        ...
    ],
    initialReaction: Reaction<String>(
        value: 'like',
        icon: widget,
    ),
    selectedReaction: Reaction<String>(
        value: 'like_fill',
        icon: widget,
    ),
)
```


## License

```legal
MIT License

Copyright (c) 2023 Abdelouahed Medjoudja

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
