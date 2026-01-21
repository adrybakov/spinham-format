.. _mapping_bilinear-exchange:

*****************
Bilinear exchange
*****************

Bilinear exchange involves two magnetic sites and two "entities". Therefore, it
should map to the term of the Hamiltonian with

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

GROGU
-----

In :ref:`zoo_grogu`, the bilinear exchange term is written as

.. math::

    \mathcal{H}
    =
    \frac{1}{2}
    \sum_{i\neq j}
    \boldsymbol{e}_{i}
    \cdot
    \boldsymbol{J}_{ij}
    \cdot
    \boldsymbol{e}_{j}

By renaming the indices as :math:`i \rightarrow (\mu_1, \alpha_1)`, 
:math:`j \rightarrow (\mu_2, \alpha_2)` and writing the matrix products 
explicitly as sums over Cartesian components, one gets

.. math::

    \mathcal{H}
    =
    \frac{1}{2}
    \sum_{\substack{\mu_1, \mu_2,\\ \alpha_1, \alpha_2,\\ i_1, i_2}}
    J_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_1, i_2}
    e_{\mu_1, \alpha_1}^{i_1}
    e_{\mu_2, \alpha_2}^{i_2}

where :math:`i_1, i_2 = x, y, z`. From here the correspondence is clear

.. math::

    C_{2, 1} &= \frac{1}{2}
    \\
    V_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2} &= J_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_1, i_2}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= e_{\mu_1, \alpha_1}^{i_1}
    \\
    X_{\mu_2; \alpha_2}^{i_2} &= e_{\mu_2, \alpha_2}^{i_2}

juKKR, TB2J
-----------

In :ref:`zoo_jukkr` and :ref:`zoo_tb2j`, the bilinear exchange term is written as


.. math::

    \mathcal{H}
    =
    -
    \sum_{i\ne j}
    \mathbf{S}_{i}
    \cdot
    \boldsymbol{J}_{ij}
    \cdot
    \mathbf{S}_{j}

By renaming the indices as :math:`i \rightarrow (\mu_1, \alpha_1)`,
:math:`j \rightarrow (\mu_2, \alpha_2)` and writing the matrix products
explicitly as sums over Cartesian components, one gets  

.. math::

    \mathcal{H}
    =
    -
    \sum_{\substack{\mu_1, \mu_2,\\ \alpha_1, \alpha_2,\\ i_1, i_2}}
    J_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_1, i_2}
    S_{\mu_1, \alpha_1}^{i_1}
    S_{\mu_2, \alpha_2}^{i_2}

where :math:`i_1, i_2 = x, y, z`. From here the correspondence is clear

.. math::

    C_{2, 1} &= -1
    \\
    V_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2} &= J_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_1, i_2}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= S_{\mu_1, \alpha_1}^{i_1}
    \\
    X_{\mu_2; \alpha_2}^{i_2} &= S_{\mu_2, \alpha_2}^{i_2}

Magpie
------

In :ref:`zoo_magpie`, the bilinear exchange term is written as

.. math::

    \mathcal{H}
    =
    \sum_{i \neq j}
    J_{ij}
    \,
    \mathbf{S}_i
    \cdot
    \mathbf{S}_j
    +
    \sum_{i \neq j}
    \mathbf{D}_{ij}
    \cdot
    \left(
    \mathbf{S}_i
    \times
    \mathbf{S}_j
    \right)

By renaming the indices as :math:`i \rightarrow (\mu_1, \alpha_1)`,
:math:`j \rightarrow (\mu_2, \alpha_2)` and writing the scalar and vector 
products explicitly as sums over Cartesian components, one gets


.. math::

    \mathcal{H}
    =
    \sum_{\substack{\mu_1, \mu_2,\\ \alpha_1, \alpha_2,\\ i_1, i_2}}
    J_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_1, i_2}
    S_{\mu_1, \alpha_1}^{i_1}
    S_{\mu_2, \alpha_2}^{i_2}
    +
    \sum_{\substack{\mu_1, \mu_2,\\ \alpha_1, \alpha_2,\\ i_1, i_2, i_3}}
    D_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_3}
    e_{i_1, i_2, i_3}
    S_{\mu_1, \alpha_1}^{i_1}
    S_{\mu_2, \alpha_2}^{i_2}
    =
    \sum_{\substack{\mu_1, \mu_2,\\ \alpha_1, \alpha_2,\\ i_1, i_2}}
    S_{\mu_1, \alpha_1}^{i_1}
    S_{\mu_2, \alpha_2}^{i_2}
    \Bigl(
    J_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_1, i_2}
    +
    \sum_{i_3}
    D_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_3}
    e_{i_1, i_2, i_3}
    \Bigr)

where :math:`i_1, i_2, i_3 = x, y, z` and :math:`e_{i_2, i_3, i_1}` is the
Levi-Civita symbol. From here the correspondence is clear

.. math::

    C_{2, 1} &= 1
    \\
    V_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2} &= 
    J_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_1, i_2}
    +
    \sum_{i_3}
    D_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_3}
    e_{i_1, i_2, i_3}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= S_{\mu_1, \alpha_1}^{i_1}
    \\
    X_{\mu_2; \alpha_2}^{i_2} &= S_{\mu_2, \alpha_2}^{i_2}

McPhase
-------

in :ref:`zoo_mcphase`, the bilinear exchange term is written as

.. math::

    \hat{\mathcal{H}}
    =
    -
    \dfrac{1}{2}
    \sum_{nn^{\prime}, \alpha\beta}
    \mathcal{J}(\mathbf{R}_{n^{\prime}} - \mathbf{R}_{n})
    \hat{\mathcal{I}}_{\alpha}^n
    \hat{\mathcal{I}}_{\beta}^{n^{\prime}}

where operators :math:`\hat{\mathcal{I}}` are interpreted as either 

.. math::

    \begin{pmatrix}
        \hat{\mathcal{I}}_1^n \\
        \hat{\mathcal{I}}_2^n \\
        \hat{\mathcal{I}}_3^n
    \end{pmatrix}
    =
    \begin{pmatrix}
        \hat{J}_x^n \\
        \hat{J}_y^n \\
        \hat{J}_z^n
    \end{pmatrix}
    

or 

.. math::

    \hat{\mathcal{I}}^n
    \begin{pmatrix}
        \hat{\mathcal{I}}_1^n \\
        \hat{\mathcal{I}}_2^n \\
        \hat{\mathcal{I}}_3^n \\
        \hat{\mathcal{I}}_4^n \\
        \hat{\mathcal{I}}_5^n \\
        \hat{\mathcal{I}}_6^n
    \end{pmatrix}
    =
    \begin{pmatrix}
        \hat{S}_x^n \\
        \hat{S}_y^n \\
        \hat{S}_z^n \\
        \hat{L}_x^n \\
        \hat{L}_y^n \\
        \hat{L}_z^n
    \end{pmatrix}

By renaming the indices as :math:`n \rightarrow (\mu_1, \alpha_1)`,
:math:`n^{\prime} \rightarrow (\mu_2, \alpha_2)`, :math:`\alpha \rightarrow i_1`,
:math:`\beta \rightarrow i_2` one gets

.. math::

    \hat{\mathcal{H}}
    =
    -
    \dfrac{1}{2}
    \sum_{\substack{\mu_1, \mu_2,\\ \alpha_1, \alpha_2,\\ i_1, i_2}}
    \mathcal{J}^{i_1,i_2}(\mathbf{R}_{\mu_2, \alpha_2} - \mathbf{R}_{\mu_1, \alpha_1})
    \hat{\mathcal{I}}^{\mu_1; \alpha_1}_{i_1}
    \hat{\mathcal{I}}^{\mu_2; \alpha_2}_{i_2}

where indices :math:`i_1, i_2` run either over three or six components. From
here the correspondence is clear

.. math::

    C_{2, 1} &= -\dfrac{1}{2}
    \\
    V_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2} &= \mathcal{J}^{i_1,i_2}(\mathbf{R}_{\mu_2, \alpha_2} - \mathbf{R}_{\mu_1, \alpha_1})
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= \hat{\mathcal{I}}^{\mu_1; \alpha_1}_{i_1}
    \\
    X_{\mu_2; \alpha_2}^{i_2} &= \hat{\mathcal{I}}^{\mu_2; \alpha_2}_{i_2}

SpinW
-----

In :ref:`zoo_spinw`, the bilinear exchange term is written as

.. math::
    \mathcal{H}
    =
    \sum_{i \neq j}
    \mathbf{S}_i J_{ij} \mathbf{S}_j

By renaming the indices as :math:`i \rightarrow (\mu_1, \alpha_1)`, 
:math:`j \rightarrow (\mu_2, \alpha_2)` and writing the matrix products
explicitly as sums over Cartesian components, one gets

.. math::

    \mathcal{H}
    =
    \sum_{\substack{\mu_1, \mu_2,\\ \alpha_1, \alpha_2,\\ i_1, i_2}}
    J_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_1, i_2}
    S_{\mu_1, \alpha_1}^{i_1}
    S_{\mu_2, \alpha_2}^{i_2}

where :math:`i_1, i_2 = x, y, z`. From here the correspondence is clear

.. math::

    C_{2, 1} &= 1
    \\
    V_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2} &= J_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_1, i_2}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= S_{\mu_1, \alpha_1}^{i_1}
    \\
    X_{\mu_2; \alpha_2}^{i_2} &= S_{\mu_2, \alpha_2}^{i_2}

Spirit
------

In :ref:`zoo_spirit`, the bilinear exchange term is written as

.. math::

    \mathcal{H}
    =
    -\frac{1}{2}
    \sum_{i\neq j}
    J_{ij}^{\alpha\beta}
    n_i^\alpha
    n_j^\beta

By renaming the indices as :math:`i \rightarrow (\mu_1, \alpha_1)`,
:math:`j \rightarrow (\mu_2, \alpha_2)`, :math:`\alpha \rightarrow i_1`,
:math:`\beta \rightarrow i_2` one gets

.. math::

    \mathcal{H}
    =
    -\frac{1}{2}
    \sum_{\substack{\mu_1, \mu_2,\\ \alpha_1, \alpha_2,\\ i_1, i_2}}
    J_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_1, i_2}
    n_{\mu_1, \alpha_1}^{i_1}
    n_{\mu_2, \alpha_2}^{i_2}

where :math:`i_1, i_2 = x, y, z`. From here the correspondence is clear

.. math::

    C_{2, 1} &= -\frac{1}{2}
    \\
    V_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2} &= J_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_1, i_2}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= n_{\mu_1, \alpha_1}^{i_1}
    \\
    X_{\mu_2; \alpha_2}^{i_2} &= n_{\mu_2, \alpha_2}^{i_2}


Sunny
-----

In :ref:`zoo_sunny`, the bilinear exchange term is written as

.. math::

    \mathcal{H}
    =
    \sum_{i<j}
    \mathbf{S}_{j}
    J_{ij}
    \mathbf{S}_{j}

By renaming the indices as :math:`i \rightarrow (\mu_1, \alpha_1)`,
:math:`j \rightarrow (\mu_2, \alpha_2)` and writing the matrix products
explicitly as sums over Cartesian components, one gets

.. math::

    \mathcal{H}
    =
    \sum_{\substack{\mu_1, \mu_2,\\ \alpha_1, \alpha_2,\\ i_1, i_2}}
    J_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_1, i_2}
    S_{\mu_1, \alpha_1}^{i_1}
    S_{\mu_2, \alpha_2}^{i_2}

where :math:`i_1, i_2 = x, y, z`. From here the correspondence is clear

.. math::

    C_{2, 1} &= 1
    \\
    V_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2} &= J_{\mu_1, \alpha_1; \mu_2, \alpha_2}^{i_1, i_2}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= S_{\mu_1, \alpha_1}^{i_1}
    \\
    X_{\mu_2; \alpha_2}^{i_2} &= S_{\mu_2, \alpha_2}^{i_2}
    \\
    (\mu_1, \alpha_1) &< (\mu_2, \alpha_2)