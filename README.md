# Lý thuyết điều khiển tự động — Bài tập và lời giải

Tài liệu gồm các đề bài và lời giải được biên soạn từ ghi chép môn **Lý thuyết điều khiển tự động**.

## Nội dung

- `main.tex`: mã nguồn LaTeX.
- `main.pdf`: bản PDF đã biên dịch.
- `.github/workflows/build-latex.yml`: tự động biên dịch lại PDF khi `main.tex` thay đổi.

## Biên dịch cục bộ

```bash
latexmk -pdf -interaction=nonstopmode -halt-on-error main.tex
```

Workflow GitHub Actions dùng cùng cách biên dịch và, khi PDF thay đổi, commit `main.pdf` với danh tính Git của tài khoản `dt-thenf` để lịch sử contributor không phát sinh `github-actions[bot]` ở các commit mới.
