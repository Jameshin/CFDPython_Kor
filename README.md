Text provided under a Creative Commons Attribution license, CC-BY.  All code is made available under the FSF-approved MIT license.  (c) Lorena A. Barba, Gilbert F. Forsyth 2015. Thanks to NSF for support via CAREER award #1149784.
@LorenaABarba

- Lorena A Barba 교수의 CFDPython 강의 번역본

The $v$-momentum equation:
<font color='red'>$v$-운동량 방정식은 다음과 같습니다.</font>

\begin{eqnarray}
&&\frac{v_{i,j}^{n+1}-v_{i,j}^{n}}{\Delta t}+u_{i,j}^{n}\frac{v_{i,j}^{n}-v_{i-1,j}^{n}}{\Delta x}+v_{i,j}^{n}\frac{v_{i,j}^{n}-v_{i,j-1}^{n}}{\Delta y}\\\
&&=-\frac{1}{\rho}\frac{p_{i,j+1}^{n}-p_{i,j-1}^{n}}{2\Delta y}\\\
&&+\nu\left(\frac{v_{i+1,j}^{n}-2v_{i,j}^{n}+v_{i-1,j}^{n}}{\Delta x^2}+\frac{v_{i,j+1}^{n}-2v_{i,j}^{n}+v_{i,j-1}^{n}}{\Delta y^2}\right)
\end{eqnarray}

And the pressure equation:
<font color='red'>마지막으로 압력 방정식은 다음과 같습니다.</font>

\begin{eqnarray}
&&\frac{p_{i+1,j}^{n}-2p_{i,j}^{n}+p_{i-1,j}^{n}}{\Delta x^2}+\frac{p_{i,j+1}^{n}-2*p_{i,j}^{n}+p_{i,j-1}^{n}}{\Delta y^2}\\\
&&=\rho\left(\frac{1}{\Delta t}\left(\frac{u_{i+1,j}-u_{i-1,j}}{2\Delta x}+\frac{v_{i,j+1}-v_{i,j-1}}{2\Delta y}\right)\right.\\\
&&-\frac{u_{i+1,j}-u_{i-1,j}}{2\Delta x}\frac{u_{i+1,j}-u_{i-1,j}}{2\Delta x}\\\
&&-2\frac{u_{i,j+1}-u_{i,j-1}}{2\Delta y}\frac{v_{i+1,j}-v_{i-1,j}}{2\Delta x}\\\
&&-\left.\frac{v_{i,j+1}-v_{i,j-1}}{2\Delta y}\frac{v_{i,j+1}-v_{i,j-1}}{2\Delta y}\right)
\end{eqnarray}

![StreamlinesTrailingEdge](https://github.com/user-attachments/assets/59c81ea5-129b-406e-b429-95f1778090f3)
