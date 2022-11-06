# Sum Frequency Generation-Orientation Analysis 
Sum frequency generation (SFG) is a coherent second-order nonlinear process which involves three photons of visible, infrared (IR), and SFG, at a surface. Using SFG molecular orientation on a surface can be determined. 

![SFG process]( https://github.com/jhjang101/SFG-Orientation/blob/main/SFG%20process.png)

 Spectral magnitudes of SFG are directly proportional to the induced second-order nonlinear dipole moment per unit volume, , by the two incident light fields.
$$I_{SFG} \propto | P^{(2)}_{eff}= \chi^{(2)}_{eff}:E_{Vis} E_{IR}|$$
$\chi^{(2)}_{eff}$ is a third-rank tensor, which contains tensorial Fresnel factors at the interface and macroscopic second-order nonlinear susceptibilities, $\chi^{(2)}_{ijk}$.  Here, $i$, $j$ , $k$ and are laboratory coordinates of SFG, visible, and IR, respectively. $\chi^{(2)}_{ijk}$ consists of the orientational average of the second-order hyperpolarizability, $\beta^{(2)}_{lmn}$. The $i$, $j$ , and $k$ represents surface coordinates system $x$, $y$, and $z$, and the $l$, $m$ , and $n$ represents molecular coordinates system $a$, $b$, and $c$.
 The linear combination of molecular hyperpolarizability tensor elements to express each macroscopic susceptibility tensor element is made by Euler transformations between laboratory coordinates (_x_, _y_ and _z_) and molecular coordinates (_a_, _b_ and _c_).
 
 ![Euler transformation](https://github.com/jhjang101/SFG-Orientation/blob/main/Euler%20transformation.png)
 
 In this repo, I write a Mathematica notebook to identify composition of molecular hyperpolarizability elements in non-vanishing $\chi^{(2)}_{ijk}$ tenser elements for $C_{3V}$, $C_{2V}$, and $C_{\infty V}$ molecular symmetry on a surface.
