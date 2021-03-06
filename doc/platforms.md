# Supported Platforms

Flame runs on top of Flutter, so its supported platforms depend on how mature/stable support for each platform is by Flutter.

At the moment, mobile has full support, and we try to keep supporting web the best we can.

## Flutter channels

Flame keeps it support on the stable and beta channel, dev and master channel should work, but we don't support them. This mean that issues happening outside stable or beta channel, are not a priority.

## Flame web

To use Flame on web you need to be on the beta channel of Flutter and the game should be running using skia rendering, otherwise weird side effects may happen.

To run your game using skia in release mode, use the following command:

`$ flutter run -d Chrome --release --dart-define=FLUTTER_WEB_USE_SKIA=true`

To run with skia on debug mode, just start the project using the conventional command:

`$ flutter run -d Chrome`

And when the app starts and the debug is setup, press the `k` key. That will enable the `CanvasKit` mode.

To build the game for production, using skia, use the following:

`$ flutter build web --release --dart-define=FLUTTER_WEB_USE_SKIA=true`

