# Notes on Physics

Ghi chép môn **Vật lý II** (điện, từ, quang) của sinh viên Trường Đại học Khoa học Tự nhiên, ĐHQG-HCM, viết bằng LaTeX. Phần điện từ tham khảo giáo trình *Introduction to Electrodynamics* của David J. Griffiths.

## Nội dung

| Chương | Tên | File |
|---|---|---|
| 1 | Vector Calculus: toán tử nabla, tích phân đường, mặt, khối, tọa độ cầu, định lý Helmholtz | `sections/vector_calculus.tex` |
| 2 | Electrostatics: điện trường, định luật Gauss, thế điện, phương trình Poisson | `sections/electrostatics.tex` |
| 3 | Magnetostatics: lực Lorentz, định luật Biot–Savart–Laplace, định luật Ampère, cảm ứng điện từ, tự cảm | `sections/magnetostatics.tex` |
| 4 | Optics: định luật Descartes, nguyên lý Fermat, giao thoa, nhiễu xạ | `sections/optics.tex` |

## Cấu trúc thư mục

- `Physics_II.tex`: file chính.
- `arxiv_book.sty`: preamble (gói, font, môi trường định lý, ký hiệu).
- `sections/`: nội dung từng chương.
- `figures/`: ảnh dùng trong sách và ảnh bìa (`cover.pdf`, `cover.png`).

## Biên dịch

Cần **MiKTeX** hoặc **TeX Live** có XeLaTeX và `latexmk`, kèm font **TeX Gyre Termes** và **TeX Gyre Termes Math**.

```
latexmk -xelatex Physics_II.tex
```

Kết quả là `Physics_II.pdf`. Các file phụ (`.aux`, `.log`, …) đã được bỏ qua trong `.gitignore`.

