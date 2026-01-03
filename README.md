# Marp Theme Collection

YouTube収録用のMarpカスタムテーマ集。

## Themes

| Theme | Description |
|-------|-------------|
| `youtube-theme.css` | YouTube収録用テーマ（Blue-Cyanグラデーション） |

## Usage

### GitHub Pages URL

```yaml
---
marp: true
theme: https://tomada1114.github.io/marp-theme/youtube-theme.css
---
```

### Local Clone

```bash
git clone https://github.com/tomada1114/marp-theme.git ~/workspace/marp-theme
```

```yaml
---
marp: true
theme: /Users/yourname/workspace/marp-theme/youtube-theme.css
---
```

## Theme Classes

### Slide Types

| Class | Usage |
|-------|-------|
| `title` | タイトルスライド（中央揃え、背景グレー） |
| `section` | セクション区切り（グラデーション背景） |
| `no-header` | ヘッダーなし（上部パディング縮小） |

### Layout

| Class | Usage |
|-------|-------|
| `align-center` | コンテンツを垂直中央揃え |
| `text-center` | テキストを水平中央揃え |
| `subtitle-safe` | 字幕用に下部パディング追加（180px） |
| `small-text` | フォントサイズ縮小 |
| `col2` | 2カラムグリッド |
| `col3` | 3カラムグリッド |

## Example

```markdown
---
marp: true
theme: https://tomada1114.github.io/marp-theme/youtube-theme.css
paginate: false
---

<!-- _class: title -->

# Episode Title

## Subtitle

---

<!-- _class: section -->

## Section 1

---

# Normal Slide

- Point 1
- Point 2
- Point 3

---

<!-- _class: align-center text-center -->

# Thank you for watching!
```

## License

MIT
