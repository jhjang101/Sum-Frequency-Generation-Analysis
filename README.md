# Sum Frequency Generation-Orientation Analysis 
Sum frequency generation (SFG) is a coherent second-order nonlinear process which involves three photons of visible, infrared (IR), and SFG, at a surface. Using SFG molecular orientation on a surface can be determined. 

![SFG process]( https://github.com/jhjang101/SFG-Orientation/blob/main/SFG%20process.png)

 Spectral magnitudes of SFG are directly proportional to the induced second-order nonlinear dipole moment per unit volume, , by the two incident light fields.
 
$$I\_{SFG} \propto | P^{(2)\}_{eff}= \chi^{(2)}\_{eff}:E_{Vis} E\_{IR}|$$

$\chi^{(2)}\_{eff}$ is a third-rank tensor, which contains tensorial Fresnel factors at the interface and macroscopic second-order nonlinear susceptibilities, $\chi^{(2)}\_{ijk}$.  Here, $i$, $j$ , $k$ and are laboratory coordinates of SFG, visible, and IR, respectively. $\chi^{(2)}\_{ijk}$ consists of the orientational average of the second-order hyperpolarizability, $\beta^{(2)}\_{lmn}$. The $i$, $j$ , and $k$ represents surface coordinates system $x$, $y$, and $z$, and the $l$, $m$ , and $n$ represents molecular coordinates system $a$, $b$, and $c$.
 The linear combination of molecular hyperpolarizability tensor elements to express each macroscopic susceptibility tensor element is made by Euler transformations between laboratory coordinates (_x_, _y_ and _z_) and molecular coordinates (_a_, _b_ and _c_).
 
 ![Euler transformation](https://github.com/jhjang101/SFG-Orientation/blob/main/Euler%20transformation.png)
 
 In this repo, I write a Mathematica notebook to identify composition of molecular hyperpolarizability elements in non-vanishing $\chi^{(2)}\_{ijk}$ tenser elements for  $C\_{3V}$, $C\_{2V}$, and $C\_{\infty V}$ molecular symmetry on a surface.
 
# Gaussian Distribution Analysis
The SFG orientation analysis demonstrated in previous section are based on delta-function distribution, assuming all molecules have same tilt angle. In reality, the molecules on a surface do not have a unique tilt angle but show an orientational distribution, $\sigma$. Thus, the orientational average SFG intensity does not provide a good interpretation for considering that each molecule on the surface has its own tilt angle. In order to address this problem, Gaussian distribution is used to describe the heterogeneity of the surface molecules as follows.

$$I\_{SFG}(\theta,\sigma)=|\frac{\int_0^{180} \chi\_{eff} \sin\theta\ Gauss\ \mathrm{d}\theta}{\int_0^{180} \sin\theta\ Gauss\ \mathrm{d}\theta}|^2 $$

$$Gauss=\frac{1}{\sqrt{2\pi}}e^{-\frac{(\theta-\theta_c)^2}{2\sigma^2}}$$

Here, $\sigma$ and $\theta\_c$ are orientation distribution and center orientation angle.
As an example, plot (a) and (b) shows simulated SFG intensity changes of $C\_{3V}$ symmetry molecules on isotropic surface for ssp and ppp polarization combination, respectively. The Plot (c) shows the intensity ratio of ppp and ssp polarization combination. Each orientation curve has been simulated at 0° to 90° of orientation distribution angle, $\sigma$. The Mathematica codes for generating the orientation curve with Gaussian convolution are included in this repo.

![SFG orientation distribution](https://github.com/jhjang101/SFG-Orientation/blob/main/Orientation%20distribution.png)
