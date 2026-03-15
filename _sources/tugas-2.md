# Tugas Eliminasi Gaussian

## 1. SPL (Sistem Persamaan Linear)

$$
\begin{cases}
x_1 + x_2 + x_3 + x_4 + x_5 = 15 \\
x_2 + x_3 + x_4 + x_5 = 14 \\
x_3 + x_4 + x_5 = 12 \\
x_4 + x_5 = 9 \\
x_5 = 5
\end{cases}
$$

## 2. Matriks Augmented

$$
\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
0 & 1 & 1 & 1 & 1 & 14 \\
0 & 0 & 1 & 1 & 1 & 12 \\
0 & 0 & 0 & 1 & 1 & 9 \\
0 & 0 & 0 & 0 & 1 & 5
\end{array}
\right]
$$

## 3. Eliminasi Gauss (OBE)

### Langkah 1

Pivot baris 1 kolom 1 = 1

$$
\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
0 & 1 & 1 & 1 & 1 & 14 \\
0 & 0 & 1 & 1 & 1 & 12 \\
0 & 0 & 0 & 1 & 1 & 9 \\
0 & 0 & 0 & 0 & 1 & 5
\end{array}
\right]
$$

### Langkah 2

Operasi baris

$$
R_4 \leftarrow R_4 - R_5
$$

$$
R_3 \leftarrow R_3 - R_5
$$

$$
R_2 \leftarrow R_2 - R_5
$$

$$
R_1 \leftarrow R_1 - R_5
$$

Hasil

$$
\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 0 & 10 \\
0 & 1 & 1 & 1 & 0 & 9 \\
0 & 0 & 1 & 1 & 0 & 7 \\
0 & 0 & 0 & 1 & 0 & 4 \\
0 & 0 & 0 & 0 & 1 & 5
\end{array}
\right]
$$

### Langkah 3

$$
R_3 \leftarrow R_3 - R_4
$$

$$
R_2 \leftarrow R_2 - R_4
$$

$$
R_1 \leftarrow R_1 - R_4
$$

$$
\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 0 & 0 & 6 \\
0 & 1 & 1 & 0 & 0 & 5 \\
0 & 0 & 1 & 0 & 0 & 3 \\
0 & 0 & 0 & 1 & 0 & 4 \\
0 & 0 & 0 & 0 & 1 & 5
\end{array}
\right]
$$

### Langkah 4

$$
R_2 \leftarrow R_2 - R_3
$$

$$
R_1 \leftarrow R_1 - R_3
$$

$$
\left[
\begin{array}{ccccc|c}
1 & 1 & 0 & 0 & 0 & 3 \\
0 & 1 & 0 & 0 & 0 & 2 \\
0 & 0 & 1 & 0 & 0 & 3 \\
0 & 0 & 0 & 1 & 0 & 4 \\
0 & 0 & 0 & 0 & 1 & 5
\end{array}
\right]
$$

### Langkah 5

$$
R_1 \leftarrow R_1 - R_2
$$

$$
\left[
\begin{array}{ccccc|c}
1 & 0 & 0 & 0 & 0 & 1 \\
0 & 1 & 0 & 0 & 0 & 2 \\
0 & 0 & 1 & 0 & 0 & 3 \\
0 & 0 & 0 & 1 & 0 & 4 \\
0 & 0 & 0 & 0 & 1 & 5
\end{array}
\right]
$$

## 4. Hasil Akhir

$$
x_1 = 1,\quad x_2 = 2,\quad x_3 = 3,\quad x_4 = 4,\quad x_5 = 5
$$