## Table of Contents

Satoshi Toyosawa / 豊沢 聡, Ph. D.

- [Academic papers / 学術論文](./Papers.md)
- [Books](./Books.en.md) / [書籍](./Books.ja.md)
- [Magazine articles / 雑誌記事](./Magazines.md)
- [F5 DevCentral Technical articles / F5 DevCentral 技術資料](./DevCentral.md)
- [Lectures / 講義](./Lectures.md)
- [Presentations / プレゼンテーション](./Presentations.md)
- [Patents / 特許](./Tokkyo.md)

```bash
[File] main.py
  1  import streamlit as st
  2
  3  if 'image_upload' in st.session_state:
  4      st.sidebar.markdown(f'ファイル: {st.session_state.image_upload.filename}')
  5
  6  if 'image_scale' in st.session_state:
  7      st.sidebar.markdown(f'リサイズ: {st.session_state.image_scale}')
  8
  9  if 'image_colors' in st.session_state:
 10      st.sidebar.markdown(f'色数: {st.session_state.image_colors}')
 11
 12  pg = st.navigation({
 13      '画像処理サービス': [
 14          st.Page('page1.py', title='アップロード', icon='📤'),
 15          st.Page('page2.py', title='リサイズ', icon='📐'),
 16          st.Page('page3.py', title='ポスタリゼーション', icon='🎨')
 17      ]})
 18  pg.run()
```