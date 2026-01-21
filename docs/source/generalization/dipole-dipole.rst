.. _mapping_dipole-dipole:

**********************************
Magnetic dipole-dipole interaction
**********************************

Magnetic dipole-dipole interaction involves two magnetic sites and
two "entities". Therefore, it should map to the term of the Hamiltonian with

- :math:`k = 2`
- :math:`l = 1`

Then, :math:`m_{2,1} = 2` and the term have the form

.. math::

    \mathcal{H}_{2,1}
    =
    C_{2, 1}
    \sum_{\substack{\mu_1, \mu_2,\\ \alpha_1, \alpha_2,\\ i_1, i_2}}
    V_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2}
    X_{\mu_1; \alpha_1}^{i_1}
    X_{\mu_2; \alpha_2}^{i_2}

McPhase, Sunny
--------------

In :ref:`zoo_mcphase` and :ref:`zoo_sunny`, the magnetic dipole-dipole
term is written as (in the notation of McPhase)

.. math::

    \mathcal{H}
    =
    -
    \dfrac{1}{2}
    \sum_{n\ne n^{\prime},\alpha\beta=1,2,3}
    \mathcal{J}_{\alpha\beta}(\mathbf{R}_{n^{\prime}} - \mathbf{R}_{n})
    \hat{\mathcal{I}}_{\alpha}^n
    \hat{\mathcal{I}}_{\beta}^{n^{\prime}}

where the operators are understood as
:math:`\hat{\mathcal{I}}_{1}  \leftrightarrow \hat{J}_x`,
:math:`\hat{\mathcal{I}}_{2}  \leftrightarrow \hat{J}_y`,
:math:`\hat{\mathcal{I}}_{3}  \leftrightarrow \hat{J}_z` in McPhase and
as :math:`\hat{\mathcal{I}}_{1}  \leftrightarrow \hat{S}_x`,
:math:`\hat{\mathcal{I}}_{2}  \leftrightarrow \hat{S}_y`,
:math:`\hat{\mathcal{I}}_{3}  \leftrightarrow \hat{S}_z` in Sunny. 

.. math::

    \mathcal{J}_{\alpha\beta}(\mathbf{R}_{n^{\prime}} - \mathbf{R}_{n})
    =
    \dfrac{\mu_0\mu_B^2 g_n g_{n^{\prime}}}{2\pi}
    \Biggl(
        3\dfrac{(R_{n^{\prime}}^{\alpha} - R_{n}^{\alpha})(R_{n^{\prime}}^{\beta} - R_{n}^{\beta})}{|\mathbf{R}_{n^{\prime}} - \mathbf{R}_{n}|^5}
        -
        \dfrac{\delta_{\alpha\beta}}{|\mathbf{R}_{n^{\prime}} - \mathbf{R}_{n}|^3}
    \Biggr)

By renaming indices as :math:`n \rightarrow (\mu_1, \alpha_1)`, 
:math:`n^{\prime} \rightarrow (\mu_2, \alpha_2)`, :math:`\alpha \rightarrow i_1`,
:math:`\beta \rightarrow i_2`, one gets

.. math::

    \mathcal{H}
    =
    \dfrac{1}{2}
    \sum_{\substack{\mu_1, \mu_2,\\ \alpha_1, \alpha_2,\\ i_1, i_2}}
    \mathcal{J}_{i_1, i_2}(\mathbf{R}_{\mu_2, \alpha_2} - \mathbf{R}_{\mu_1, \alpha_1})
    \hat{\mathcal{I}}_{i_1}^{\mu_1; \alpha_1}
    \hat{\mathcal{I}}_{i_2}^{\mu_2; \alpha_2}

.. math::

    \mathcal{J}_{i_1, i_2}(\mathbf{R}_{\mu_2, \alpha_2} - \mathbf{R}_{\mu_1, \alpha_1})
    =
    \dfrac{\mu_0\mu_B^2 g_{\mu_1, \alpha_1} g_{\mu_2, \alpha_2}}{2\pi}
    \Biggl(
        3\dfrac{(R_{\mu_2, \alpha_2}^{i_1} - R_{\mu_1, \alpha_1}^{i_1})(R_{\mu_2, \alpha_2}^{i_2} - R_{\mu_1, \alpha_1}^{i_2})}{|\mathbf{R}_{\mu_2, \alpha_2} - \mathbf{R}_{\mu_1, \alpha_1}|^5}
        -
        \dfrac{\delta_{i_1, i_2}}{|\mathbf{R}_{\mu_2, \alpha_2} - \mathbf{R}_{\mu_1, \alpha_1}|^3}
    \Biggr)

Where :math:`i_1, i_2 = x, y, z`. From here the correspondence is clear

.. math::
    C_{2, 1} &= -\dfrac{1}{2}
    \\
    V_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2} &= \mathcal{J}_{i_1, i_2}(\mathbf{R}_{\mu_2, \alpha_2} - \mathbf{R}_{\mu_1, \alpha_1})
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= \hat{\mathcal{I}}_{i_1}^{\mu_1; \alpha_1}
    \\
    X_{\mu_2; \alpha_2}^{i_2} &= \hat{\mathcal{I}}_{i_2}^{\mu_2; \alpha_2}

Spirit
------

In :ref:`zoo_spirit`, the magnetic dipole-dipole term is written as

.. math::
   \mathcal{H}
   =
   \frac{1}{2}\frac{\mu_0}{4\pi}
   \sum_{i \neq j} \mu_i \mu_j \frac{(\vec{n}_i \cdot \hat{r}_{ij}) (\vec{n}_j\cdot\hat{r}_{ij}) - (\vec{n}_i \cdot \vec{n}_j)}{{r_{ij}}^3}

By renaming indices as :math:`i \rightarrow (\mu_1, \alpha_1)`,
:math:`j \rightarrow (\mu_2, \alpha_2)` and writing the dot products explicitly, 
one gets

.. math::
    \mathcal{H}
    =
    \dfrac{1}{2}\frac{\mu_0}{4\pi}
    \sum_{\substack{\mu_1, \mu_2,\\ \alpha_1, \alpha_2,\\ i_1, i_2}}
    \mu_{\mu_1, \alpha_1} \mu_{\mu_2, \alpha_2}
    \frac{
    \hat{r}_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_1}
    \hat{r}_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_2}
    - \delta_{i_1, i_2}
    }
    {r_{\mu_1, \alpha_1; \mu_2, \alpha_2}^3}
    n_{\mu_1, \alpha_1}^{i_1}
    n_{\mu_2, \alpha_2}^{i_2}

From here the correspondence is clear

.. math::
    C_{2, 1} &= \dfrac{1}{2}
    \\
    V_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2} &= \frac{\mu_0}{4\pi}\mu_{\mu_1, \alpha_1} \mu_{\mu_2, \alpha_2}
    \frac{
    \hat{r}_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_1}
    \hat{r}_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_2}
    - \delta_{i_1, i_2}
    }
    {r_{\mu_1, \alpha_1; \mu_2, \alpha_2}^3}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= n_{\mu_1, \alpha_1}^{i_1}
    \\
    X_{\mu_2; \alpha_2}^{i_2} &= n_{\mu_2, \alpha_2}^{i_2}