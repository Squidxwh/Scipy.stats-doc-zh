
.. _continuous-nakagami:

Nakagami Distribution
=====================

Generalization of the chi distribution. Shape parameter is :math:`\nu>0.` The support is :math:`x\geq0.`

.. math::
   :nowrap:

    \begin{eqnarray*} f\left(x;\nu\right) & = & \frac{2\nu^{\nu}}{\Gamma\left(\nu\right)}x^{2\nu-1}\exp\left(-\nu x^{2}\right)\\
    F\left(x;\nu\right) & = & \frac{\gamma\left(\nu,\nu x^{2}\right)}{\Gamma\left(\nu\right)}\\
    G\left(q;\nu\right) & = & \sqrt{\frac{1}{\nu}\gamma^{-1}\left(\nu,q{\Gamma\left(\nu\right)}\right)}\end{eqnarray*}

where :math:`\gamma` is the lower incomplete gamma function, :math:`\gamma\left(\nu, x\right) = \int_0^x t^{\nu-1} e^{-t} dt`.

.. math::
   :nowrap:

    \begin{eqnarray*} \mu & = & \frac{\Gamma\left(\nu+\frac{1}{2}\right)}{\sqrt{\nu}\Gamma\left(\nu\right)}\\
    \mu_{2} & = & \left[1-\mu^{2}\right]\\
    \gamma_{1} & = & \frac{\mu\left(1-4v\mu_{2}\right)}{2\nu\mu_{2}^{3/2}}\\
    \gamma_{2} & = & \frac{-6\mu^{4}\nu+\left(8\nu-2\right)\mu^{2}-2\nu+1}{\nu\mu_{2}^{2}}\end{eqnarray*}

Implementation: `scipy.stats.nakagami`
