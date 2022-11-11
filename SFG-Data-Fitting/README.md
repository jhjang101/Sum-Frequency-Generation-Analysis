# SFG-Data-Fitting
Measured SFG intensity forms convolution of Lorentzian distribution function, because in SFG process, the lifetime of the vibrational state is given by the Lorentzian line shape.

$$\chi^{(2)}\_{R}\propto \frac{N<\beta>}{\omega\_q-\omega\_{IR}-i\Gamma\_q}$$

$\Gamma\_q$ is damping constant of the vibrational mode. Thus, overall SFG intensity is given by 

$$I\_{SFG}\propto |\chi^{(2)}|^2\propto |\frac{N<\beta>}{\omega\_q-\omega\_{IR}-i\Gamma\_q} + |\chi^{(2)}\_{NR}|e^{i\varrho}|^2$$

where $\varrho$ is phase of $\chi^{(2)}\_{NR}$.

In this repo, Mathematica code for simulating SFG spectra and Data fitting. 

![SFG spectra simulation and curve fitting](https://github.com/jhjang101/SFG-Data-Fitting/blob/main/SFG%20curve%20fitting.png)

The curve fit result shows the SFG data has 6 Lorentzian distribution and each of them is corresponding the molecular vibration in SFG field. Using this data, molecular density, orientation, and distributions are determined. The example contains real data I measured during PhD and the journal publication can be seen [here](https://pubs.acs.org/doi/abs/10.1021/jp404669j).
