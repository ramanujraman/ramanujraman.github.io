---
tags:
  - condensed_matter_physics
  - notes
  - solid_state_physics
---
## Introduction
So we discussed about the mathematical formulation of the Drude's Model we have $$\frac{dp}{dt}=-\frac{p(t)}{\tau}+f(t)$$
Now we'll try to look for the case when we have AC field applied to the metal as $E(t)=Re(E(\omega)e^{i\omega t})$ the we look for steady state solution as $\vec{p}(t)=\mathrm{Re}(\vec{p(\omega)e^{i\omega t}})$. Sowe have 
$$
i\omega \vec{p}(\omega)= -\frac{\vec{p}(\omega)}{\tau}-e\vec{E}(\omega)
$$
this implies
$$
\vec{p}(\omega)= \frac{-e\vec{E}(\omega)}{(\frac{1}{\tau}+i\omega)}
$$
now the expression can be written in the form as 
$$
\vec{p}(\omega)= \frac{-e\vec{E}(\omega)\tau}{(1+i\omega \tau)}
$$
one can put the above expression in the formula for current density ($\vec{j}$) as
$$
\vec{j}(\omega)=-ne\frac{\vec{p}(\omega)}{m}=\frac{ne^2\tau}{m(1+i\omega \tau)}\vec{E}(\omega)
$$
where  $\sigma_{o}=\frac{ne^2\tau}{m}$  is the DC conductivity and the expression can be written as 
$$
\vec{j}(\omega)=-ne\frac{\vec{p}(\omega)}{m}=\frac{\sigma_{o}}{(1+i\omega \tau)}\vec{E}(\omega)
$$
and we have the final expression as 

$$
\vec{j}(\omega)=\sigma(\omega)\vec{E}(\omega)
$$

and we have $\sigma(\omega)=\frac{\sigma_{o}}{(1+i\omega \tau)}$ and for limit $\omega \rightarrow 0$ we have $\sigma(\omega)=\sigma_{o}$.
## Problems with Model
1. This model explains the movement of electromagnetic radiation in the metal but a time oscillating electric field clearly have accompanying magnetic field and our expression doesn't count for one. 
2. For a propagating wave in a metal both fields change in both space and time and we haven't counted for it in our model.
Well for the first one, we may have an extra term as $-\frac{e\vec{p}}{mc}\times\vec{H}$ the correction is very small and hence be ignored. 
The second point pose a bigger problem as we assumed that same force is experienced by each electron in the metal when placed in an electric field but it is not true for space propagating EM waves. But in our model we have collisions for every $v\tau$ and if our electric field constant over that scale we are good to go as $\vec{j}(\vec{r},\omega)=\sigma(\omega)\vec{E}(\vec{r},\omega)$ so for $\lambda >v\tau$ the above expression clearly works. Otherwise we need to resort to other models of greater complexity.
## Propagation of Electromagnetic Wave in Metal 
Consider a EM wave is traveling through the metal with $\lambda>v\tau$  then we have Maxwell's Equations as 
$$
\vec{\nabla}\vec{E}=0 ; \vec{\nabla}\times \vec{H}=\frac{4\pi}{c}\vec{j}+\frac{1}{c}\frac{\partial\vec{H}}{\partial t} ; \vec{\nabla}\vec{H}=0;\vec{\nabla}\times \vec{E}=\frac{1}{c}\frac{\partial\vec{H}}{\partial t}
$$
Now by taking 
$$
\nabla\times (\nabla \times E)=-\nabla^2\vec{E}=\frac{i\omega}{c}\nabla \times H
$$
we have $\vec{\nabla}\times \vec{H}=\frac{4\pi}{c}\vec{j}+\frac{1}{c}\frac{\partial\vec{H}}{\partial t}$  and using a propagating wave solution as $e^{i\omega t}$ we have from above expression as
$$
-\nabla^2 \vec{E}=\frac{i\omega}{c}\left( \frac{4\pi}{c}\vec{j}+\frac{1}{c}\frac{\partial \vec{H}}{\partial t} \right)
$$
we can use results from above and place into the above expression and we have
$$
-\nabla^2 \vec{E}=\frac{i\omega}{c}\left( \frac{4\pi}{c}\sigma-\frac{i\omega}{c} \right)\vec{E}
$$

