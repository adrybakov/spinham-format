.. _mapping_two-ion-crystal-field:

*********************
Two-ion crystal field
*********************

McPhase
-------

In :ref:`zoo_mcphase` the two-ion crystal field term is written with Stevens
operators as

.. math::

    \hat{\mathcal{H}}
    =
    -\dfrac{1}{2}
    \sum_{nn^{\prime}}
    \sum_{ll^{\prime}}
    \sum_{mm^{\prime}}
    K_{ll^{\prime}}^{mm^{\prime}}(nn^{\prime})
    \hat{O}_{lm}(\mathbf{J}^n)
    \hat{O}_{l^{\prime}m^{\prime}}(\mathbf{J}^{n^{\prime}})

or with the Wybourne operators  as

.. math::

    \hat{\mathcal{H}}
    =
    -
    \dfrac{1}{2}
    \sum_{nn^{\prime}}
    \Biggl[
        \sum_{kk^{\prime}}
        \sum_{qq^{\prime}}
        \mathcal{K}_{kk^{\prime}}^{qq^{\prime}}(nn^{\prime})
        \hat{T}_{kq}^n
        \hat{T}_{k^{\prime}q^{\prime}}^{n^{\prime}}
    \Biggr]


Notice, that the sets of integer pairs :math:`(l,m)`,
:math:`(l^{\prime},m^{\prime})`, :math:`(k,q)`, and :math:`(k^{\prime},q^{\prime})`
are finite, therefore, they can be enumerated by single index. Then,
by renaming indices as :math:`(l,m) \rightarrow i_1`, 
:math:`(l^{\prime},m^{\prime}) \rightarrow i_2`,
:math:`(k,q) \rightarrow i_1`, :math:`(k^{\prime},q^{\prime}) \rightarrow i_2`,
:math:`n \rightarrow (\mu_1, \alpha_1)`, :math:`n^{\prime} \rightarrow (\mu_2, \alpha_2)`
one gets

.. math::

    \hat{\mathcal{H}}
    =
    -\dfrac{1}{2}
    \sum_{\mu_1, \mu_2, \alpha_1, \alpha_2}
    \sum_{i_1, i_2}
    K_{i_1, i_2}(\mu_1, \alpha_1; \mu_2, \alpha_2)
    \hat{O}_{i_1}(\mathbf{J}^{\mu_1, \alpha_1})
    \hat{O}_{i_2}(\mathbf{J}^{\mu_2, \alpha_2})

or 

.. math::

    \hat{\mathcal{H}}
    =
    -
    \dfrac{1}{2}
    \sum_{\mu_1, \mu_2, \alpha_1, \alpha_2}
    \Biggl[
        \sum_{i_1, i_2}
        \mathcal{K}_{i_1, i_2}(\mu_1, \alpha_1; \mu_2, \alpha_2)
        \hat{T}_{i_1}^{\mu_1, \alpha_1}
        \hat{T}_{i_2}^{\mu_2, \alpha_2}
    \Biggr]

where indicex :math:`i_1` runs over all pairs of :math:`(l,m)` or :math:`(k,q)` 
in the original sums and :math:`i_2` runs over all pairs of
:math:`(l^{\prime},m^{\prime})` or :math:`(k^{\prime},q^{\prime})`.
From here the correspondence to the term of the general Hamiltonian with two
entities and two sites (:math:`k = 2`, :math:`l = 1`, :math:`m_{2,1} = 2`) is
clear

.. math::
    
    \mathcal{H}_{2, 1}
    =
    C_{2, 1}
    \sum_{\substack{\mu_1, \mu_2, \\ \alpha_1, \alpha_2, \\ i_1, i_2}}
    V_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2}
    \cdot
    X_{\mu_1; \alpha_1}^{i_1}
    \cdot
    X_{\mu_2; \alpha_2}^{i_2}

with 

.. math::

    C_{2, 1} &= -\dfrac{1}{2}
    \\
    V_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2} &= K_{i_1, i_2}(\mu_1, \alpha_1; \mu_2, \alpha_2)
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= \hat{O}_{i_1}(\mathbf{J}^{\mu_1, \alpha_1})
    \\
    X_{\mu_2; \alpha_2}^{i_2} &= \hat{O}_{i_2}(\mathbf{J}^{\mu_2, \alpha_2})

or 

.. math::

    C_{2, 1} &= -\dfrac{1}{2}
    \\
    V_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2} &= \mathcal{K}_{i_1, i_2}(\mu_1, \alpha_1; \mu_2, \alpha_2)
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= \hat{T}_{i_1}^{\mu_1, \alpha_1}
    \\
    X_{\mu_2; \alpha_2}^{i_2} &= \hat{T}_{i_2}^{\mu_2, \alpha_2}


.. _mapping_two-ion-crystal-field_ambiguity:

Two-ion crystal field (ambiguity)
---------------------------------

Two-ion crystal field terms suffer from the same ambiguity as the 
single-ion crystal field terms, see :ref:`mapping_crystal-field_ambiguity`.

An alternative mapping will result in terms of the general Hamiltonian with two
sites and arbitrary amount of entities.