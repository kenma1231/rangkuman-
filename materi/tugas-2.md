\documentclass{article}
\usepackage{amsmath}
\usepackage{geometry}
\geometry{a4paper, margin=1in}

\begin{document}

\section*{Tugas Eliminasi Gaussian}

\subsection*{1. SPL (Sistem Persamaan Linear)}

$$
\begin{cases}
x_1 + x_2 + x_3 + x_4 + x_5 = 15 \\
2x_1 + x_2 + x_3 + x_4 + x_5 = 16 \\
x_1 + 2x_2 + x_3 + x_4 + x_5 = 16 \\
x_1 + x_2 + 2x_3 + x_4 + x_5 = 17 \\
x_1 + x_2 + x_3 + 2x_4 + x_5 = 18
\end{cases}
$$

\subsection*{2. Matriks Augmented}

$$
\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
2 & 1 & 1 & 1 & 1 & 16 \\
1 & 2 & 1 & 1 & 1 & 16 \\
1 & 1 & 2 & 1 & 1 & 17 \\
1 & 1 & 1 & 2 & 1 & 18
\end{array}
\right]
$$

\subsection*{3. Eliminasi Gauss (OBE)}

\subsubsection*{Langkah 1. Nolkan elemen di bawah pivot kolom 1}

Operasi baris: \\
$R_2 \rightarrow R_2 - 2R_1$ \\
$R_3 \rightarrow R_3 - R_1$ \\
$R_4 \rightarrow R_4 - R_1$ \\
$R_5 \rightarrow R_5 - R_1$

$$
\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
0 & -1 & -1 & -1 & -1 & -14 \\
0 & 1 & 0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0 & 0 & 2 \\
0 & 0 & 0 & 1 & 0 & 3
\end{array}
\right]
$$

\subsubsection*{Langkah 2. Nolkan elemen di bawah pivot kolom 2}

Operasi baris: \\
$R_3 \rightarrow R_3 + R_2$

$$
\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
0 & -1 & -1 & -1 & -1 & -14 \\
0 & 0 & -1 & -1 & -1 & -13 \\
0 & 0 & 1 & 0 & 0 & 2 \\
0 & 0 & 0 & 1 & 0 & 3
\end{array}
\right]
$$

\subsubsection*{Langkah 3. Nolkan elemen di bawah pivot kolom 3}

Operasi baris: \\
$R_4 \rightarrow R_4 + R_3$

$$
\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
0 & -1 & -1 & -1 & -1 & -14 \\
0 & 0 & -1 & -1 & -1 & -13 \\
0 & 0 & 0 & -1 & -1 & -11 \\
0 & 0 & 0 & 1 & 0 & 3
\end{array}
\right]
$$

\subsubsection*{Langkah 4. Nolkan elemen di bawah pivot kolom 4}

Operasi baris: \\
$R_5 \rightarrow R_5 + R_4$

$$
\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
0 & -1 & -1 & -1 & -1 & -14 \\
0 & 0 & -1 & -1 & -1 & -13 \\
0 & 0 & 0 & -1 & -1 & -11 \\
0 & 0 & 0 & 0 & -1 & -8
\end{array}
\right]
$$

\subsection*{4. Hasil Akhir}

$$
x_1 = 1,\quad x_2 = 2,\quad x_3 = 3,\quad x_4 = 4,\quad x_5 = 5
$$

\end{document}