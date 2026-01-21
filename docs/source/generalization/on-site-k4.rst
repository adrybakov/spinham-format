.. _mapping_on-site-k4:

**************************
On-site anisotropy (k = 4)
**************************

.. include:: on-site.inc

Contributions to the term with :math:`k = 1` are discussed in
:ref:`mapping_zeeman`, with :math:`k = 2` in :ref:`mapping_on-site-k2`.

In this page we discuss the term with :math:`k = 4`, which can be written as

.. math::

    \mathcal{H}_{4,5}
    =
    C_{4, 5}
    \sum_{\mu_1, \alpha_1, i_1, i_2, i_3, i_4}
    V_{\mu_1; \alpha_1}^{i_1, i_2}
    X_{\mu_1; \alpha_1}^{i_1}
    X_{\mu_1; \alpha_1}^{i_2}
    X_{\mu_1; \alpha_1}^{i_3}
    X_{\mu_1; \alpha_1}^{i_4}

.. note::
    :math:`p(4) = 5`.


Spirit
------

In :ref:`zoo_spirit`, the on-site anisotropy term that maps to general
form with :math:`k = 4`  is written as

.. math::
    \mathcal{H}_{\rm cubic} = - \frac12 \sum_j K_j ([\vec{n}_j]_x^4 + [\vec{n}_j]_y^4 + [\vec{n}_j]_z^4)

By renaming the indices as
:math:`j \rightarrow (\mu_1, \alpha_1)` one gets


.. math::
    \mathcal{H}_{\rm cubic}
    =
    - \frac12
    \sum_{\mu_1, \alpha_1}
    K_{\mu_1, \alpha_1}
    ([\vec{n}_{\mu_1, \alpha_1}]_x^4 + [\vec{n}_{\mu_1, \alpha_1}]_y^4 + [\vec{n}_{\mu_1, \alpha_1}]_z^4)

This Hamiltonian has the form of the general on-site Hamiltonian with
:math:`k = 4`, which is

.. note::
    :math:`p(4) = 5`.

.. math::

    H_{4,5}
    =
    C_{4, 5}
    \sum_{\mu_1, \alpha_1, i_1, i_2, i_3, i_4}
    V_{\mu_1; \alpha_1}^{i_1, i_2, i_3, i_4}
    X_{\mu_1; \alpha_1}^{i_1}
    X_{\mu_1; \alpha_1}^{i_2}
    X_{\mu_1; \alpha_1}^{i_3}
    X_{\mu_1; \alpha_1}^{i_4}

where 

.. math::

    X_{\mu_1; \alpha_1}^{i_1} = n_{\mu_1; \alpha_1}^{i_1}

and the interaction parameter is defined as

.. math::
    V_{\mu_1; \alpha_1}^{xxxx}
    =
    V_{\mu_1; \alpha_1}^{yyyy}
    =
    V_{\mu_1; \alpha_1}^{zzzz}
    =
    K_{\mu_1, \alpha_1}

and all other components of :math:`V_{\mu_1; \alpha_1}^{i_1, i_2, i_3, i_4}` are
zero.
    

   