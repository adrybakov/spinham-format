.. _mapping_on-site-k2:

**************************
On-site anisotropy (k = 2)
**************************

.. include:: on-site.inc

Contributions to the term with :math:`k = 1` are discussed in
:ref:`mapping_zeeman`, with :math:`k = 4` in :ref:`mapping_on-site-k4`.

In this page we discuss the term with :math:`k = 2`, which can be written as

.. math::

    \mathcal{H}_{2,2}
    =
    C_{2, 2}
    \sum_{\mu_1, \alpha_1, i_1, i_2}
    V_{\mu_1; \alpha_1}^{i_1, i_2}
    X_{\mu_1; \alpha_1}^{i_1}
    X_{\mu_1; \alpha_1}^{i_2}

.. note::
    :math:`p(2) = 2`.

GROGU
-----

In :ref:`zoo_grogu`, the on-site anisotropy term (quadratic) is written as

.. math::

    \mathcal{H}
    =
    \sum_{i}
    \boldsymbol{e}_{i}
    \cdot
    \boldsymbol{K}_{i}
    \cdot
    \boldsymbol{e}_{i}

By renaming the indices as :math:`i \rightarrow (\mu_1, \alpha_1)` and
writing the matrix products explicitly as sums over Cartesian components, one
gets

.. math::

    \mathcal{H}
    =
    \sum_{\mu_1, \alpha_1, i_1, i_2}
    K_{\mu_1; \alpha_1}^{i_1, i_2}
    e_{\mu_1; \alpha_1}^{i_1}
    e_{\mu_1; \alpha_1}^{i_2}

where :math:`i_1, i_2 = x, y, z`. From here the correspondence with the on-site
term :math:`k = 2` of the general Hamiltonian is clear

.. math::

    C_{2, 2} &= 1
    \\
    V_{\mu_1; \alpha_1}^{i_1, i_2} &= K_{\mu_1; \alpha_1}^{i_1, i_2}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= e_{\mu_1; \alpha_1}^{i_1}



juKKR, Magpie, SpinW
--------------------

In :ref:`zoo_jukkr`, :ref:`zoo_magpie`, and :ref:`zoo_spinw`, the on-site
anisotropy term (quadratic) is written as


.. math::

    \mathcal{H}
    =
    \sum_{i}
    \mathbf{S}_{i}
    \cdot
    \boldsymbol{A}_{i}
    \cdot
    \mathbf{S}_{i}

By renaming the indices as :math:`i \rightarrow (\mu_1, \alpha_1)` and
writing the matrix products explicitly as sums over Cartesian components, one
gets

.. math::

    \mathcal{H}
    =
    \sum_{\mu_1, \alpha_1, i_1, i_2}
    A_{\mu_1; \alpha_1}^{i_1, i_2}
    S_{\mu_1; \alpha_1}^{i_1}
    S_{\mu_1; \alpha_1}^{i_2}

where :math:`i_1, i_2 = x, y, z`. From here the correspondence with the on-site
term :math:`k = 2` of the general Hamiltonian is clear

.. math::

    C_{2, 2} &= 1
    \\
    V_{\mu_1; \alpha_1}^{i_1, i_2} &= A_{\mu_1; \alpha_1}^{i_1, i_2}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= S_{\mu_1; \alpha_1}^{i_1}



Spirit
------

In :ref:`zoo_spirit`, the on-site anisotropy term that maps to general
form with :math:`k = 2`  is written as

.. math::
     \mathcal{H}_{\rm uni} = \sum_j K_j (\hat{K}_j\cdot\vec{n}_j)^2

By renaming the indices as :math:`j \rightarrow (\mu_1, \alpha_1)` and expanding
the square of the dot product, one gets

.. math::

    \mathcal{H}_{\rm uni}
    =
    \sum_{\mu_1, \alpha_1, i_1, i_2}
    K_{\mu_1; \alpha_1}^{i_1, i_2}
    n_{\mu_1; \alpha_1}^{i_1}
    n_{\mu_1; \alpha_1}^{i_2}

where :math:`i_1, i_2 = x, y, z` and matrix :math:`K_{\mu_1; \alpha_1}^{i_1, i_2}` 
is defined as

.. math::

    K_{\mu_1; \alpha_1}^{i_1, i_2}
    =
    \begin{pmatrix}
        K_j \hat{K}_{j,x}^2 & K_j \hat{K}_{j,x} \hat{K}_{j,y} & K_j \hat{K}_{j,x} \hat{K}_{j,z} \\
        K_j \hat{K}_{j,x} \hat{K}_{j,y} & K_j \hat{K}_{j,y}^2 & K_j \hat{K}_{j,y} \hat{K}_{j,z} \\
        K_j \hat{K}_{j,x} \hat{K}_{j,z} & K_j \hat{K}_{j,y} \hat{K}_{j,z} & K_j \hat{K}_{j,z}^2
    \end{pmatrix} 

From here the correspondence with the on-site term :math:`k = 2` of the general 
Hamiltonian is clear

.. math::

    C_{2, 2} &= 1
    \\
    V_{\mu_1; \alpha_1}^{i_1, i_2} &= K_{\mu_1; \alpha_1}^{i_1, i_2}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= n_{\mu_1; \alpha_1}^{i_1}
    

TB2J
----

In :ref:`zoo_tb2j`, the on-site anisotropy term (quadratic) is written as


.. math::

    \mathcal{H}
    =
    -
    \sum_{i}
    \mathbf{S}_{i}
    \cdot
    \boldsymbol{A}_{i}
    \cdot
    \mathbf{S}_{i}

By renaming the indices as :math:`i \rightarrow (\mu_1, \alpha_1)` and
writing the matrix products explicitly as sums over Cartesian components, one
gets

.. math::

    \mathcal{H}
    =
    -
    \sum_{\mu_1, \alpha_1, i_1, i_2}
    A_{\mu_1; \alpha_1}^{i_1, i_2}
    S_{\mu_1; \alpha_1}^{i_1}
    S_{\mu_1; \alpha_1}^{i_2}

where :math:`i_1, i_2 = x, y, z`. From here the correspondence with the on-site
term :math:`k = 2` of the general Hamiltonian is clear

.. math::

    C_{2, 2} &= -1
    \\
    V_{\mu_1; \alpha_1}^{i_1, i_2} &= A_{\mu_1; \alpha_1}^{i_1, i_2}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= S_{\mu_1; \alpha_1}^{i_1}