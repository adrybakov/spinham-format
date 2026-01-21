.. _mapping_crystal-field:

*************
Crystal field
*************


Sunny
-----

In :ref:`zoo_sunny`, crystal field term is written as

.. math::

    \mathcal{H}
    =
    \sum_{i}\sum_{k,q}
    c_{i,k,q}
    \mathcal{O}_{k,q}
    (\mathbf{S}_{i}).

set of integer pairs :math:`(k,q)` is finite, by assuming some order in the set
(fo instance, lexicographical order), one can enumerate them. Therefore, by 
renaming the indices as :math:`(k,q) \rightarrow i_1` and
:math:`n \rightarrow (\mu_1, \alpha_1)` one gets


.. math::

    \mathcal{H}
    =
    \sum_{\mu_1, \alpha_1, i_1}
    c_{\mu_1, \alpha_1, i_1}
    \mathcal{O}_{i_1}(\mathbf{S}_{\mu_1, \alpha_1})

where index :math:`i_1` runs over all pairs :math:`(k,q)` in the original sum.
From here the correspondence to the term of the general Hamiltonian with one
entity and one site (:math:`k = 1`, :math:`l = 1`, :math:`m_{1,1} = 1`) is clear

.. math::

    \mathcal{H}_{1,1}
    =
    C_{1, 1}
    \sum_{\mu_1; \alpha_1; i_1}
    V_{\mu_1; \alpha_1}^{i_1}
    X_{\mu_1; \alpha_1}^{i_1}

with 

.. math::

    C_{1, 1} &= 1
    \\
    V_{\mu_1; \alpha_1}^{i_1} &= c_{\mu_1, \alpha_1, i_1}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= \mathcal{O}_{i_1}(\mathbf{S}_{\mu_1, \alpha_1})


McPhase
-------

In :ref:`zoo_mcphase` the crystal field term is written as

.. math::

    \hat{\mathcal{H}}
    =
    \sum_n
    \sum_{lm}
    B_l^m
    \hat{O}_{lm}(\mathbf{J}^n)

using Stevens operators or as 

.. math::

    \hat{\mathcal{H}}
    =  
    \sum_n
    \sum_{lm}
    L_l^m(n)
    \hat{T}_{lm}^{n}

using Wybourne operators :math:`\hat{T}_{lm}^{n}`.

Set of integer pairs :math:`(l,m)` is finite, by assuming some order in the set
(for instance, lexicographical order), one can enumerate them. Therefore, by 
renaming the indices as :math:`(l,m) \rightarrow i_1` and
:math:`n \rightarrow (\mu_1, \alpha_1)` one gets


.. math::

    \hat{\mathcal{H}}
    =
    \sum_{\mu_1, \alpha_1}
    \sum_{i_1}
    B_{i_1}
    \hat{O}_{i_1}(\mathbf{J}^{\mu_1, \alpha_1})

or 

.. math::

    \hat{\mathcal{H}}
    =
    \sum_{\mu_1, \alpha_1}
    \sum_{i_1}
    L_{i_1}(\mu_1, \alpha_1)
    \hat{T}_{i_1}^{\mu_1, \alpha_1}

where index :math:`i_1` runs over all pairs :math:`(l,m)` in the original sum.
From here the correspondence to the term of the general Hamiltonian with one
entity and one site (:math:`k = 1`, :math:`l = 1`, :math:`m_{1,1} = 1`) is clear

.. math::

    \hat{\mathcal{H}}_{1,1}
    =
    C_{1, 1}
    \sum_{\mu_1; \alpha_1; i_1}
    V_{\mu_1; \alpha_1}^{i_1}
    X_{\mu_1; \alpha_1}^{i_1}

with

.. math::

    C_{1, 1} &= 1
    \\
    V_{\mu_1; \alpha_1}^{i_1} &= B_{i_1}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= \hat{O}_{i_1}(\mathbf{J}^{\mu_1, \alpha_1})

or

.. math::

    C_{1, 1} &= 1
    \\
    V_{\mu_1; \alpha_1}^{i_1} &= L_{i_1}(\mu_1, \alpha_1)
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= \hat{T}_{i_1}^{\mu_1, \alpha_1}
    
.. _mapping_crystal-field_ambiguity:

Crystal field (ambiguity)
-------------------------

The Crystal field term was mapped to the term of the general Hamiltonian with 
one entity and one site. However, there exist an alternative mapping.

Here is an example that illustrate it. Consider the term (in McPhase's notation)


.. math::

    \mathcal{H}
    =
    B_2^0 \hat{O}_{2}^0(\mathbf{J}^n)

With the procedure above the Stevens operators :math:`\hat{O}_{2}^0(\mathbf{J}^n)`
are mapped to the entities :math:`X_{\mu_1; \alpha_1}^{i_1}`. however, one can 
express the Stevens operators through angular momentum operator as

.. math::

    \mathcal{H}
    =
    B_2^0
    \Bigl(
        3 (\hat{J}_z^n)^2 - J(J+1)
    \Bigr)  
    =
    E_{const}
    +
    3B_2^0
    \hat{J}_z^n \hat{J}_z^n

By renaming indices as :math:`n \rightarrow (\mu_1, \alpha_1)` one can express
the non-constant part as

.. math::

    \mathcal{H}
    =
    C_{2,2}
    \sum_{\mu_1, \alpha_1, i_1, i_2}
    V_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2}
    X_{\mu_1; \alpha_1}^{i_1}
    X_{\mu_1; \alpha_1}^{i_1}

where 

.. math::

    C_{2,2} &= 1
    \\
    V_{\mu_1, \mu_2; \alpha_1, \alpha_2} &= 
    \begin{pmatrix}
        0 & 0 & 0 \\
        0 & 0 & 0 \\
        0 & 0 & 3B_2^0
    \end{pmatrix}
    \\
    X_{\mu_1; \alpha_1}^{i} &= \hat{J}_{i_1}^{\mu_1, \alpha_1}

which maps it to the term of the general Hamiltonian with two entities and
one site (:math:`k = 2`, :math:`l = 2`, :math:`m_{2,2} = 1`).

For the Stevens operators of higher order the alternative mapping will 
lead to the terms with one site and arbitrary amount of entities in the general
Hamiltonian.


