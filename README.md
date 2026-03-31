# Chord Glow

iPhone Safari で試せる最小の音パッドモックです。

## Run

ローカルで開くなら、ここで静的サーバーを立てます。

```bash
python3 -m http.server 8000
```

そのあと `http://localhost:8000` を開いてください。iPhone 実機で試すなら、同じネットワーク上で Mac の IP に向ければ動きます。

## What It Does

- 6個のコードパッドをタップすると和音が鳴る
- `Harmonica` `Fan Organ` `Fuzz Guitar` の3音色を切り替えられる
- `Drive` スライダーで歪み量を変えられる
- Web Audio API だけで完結しているので、サンプル素材は不要

## Next

- 長押し中だけ持続音にする
- XY パッドでフィルターとビブラートを同時操作
- 録音とループ再生
- iPhone アプリ化するなら SwiftUI + AVAudioEngine に移植
