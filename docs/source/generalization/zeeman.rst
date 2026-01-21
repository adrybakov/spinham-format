.. _mapping_zeeman:

******************
Zeeman interaction
******************

Zeeman interaction involves one magnetic site and one "entity". Therefore, it
should map to the term of the Hamiltonian with

- :math:`k = 1`
- :math:`l = 1`

Then, :math:`m_{1,1} = 1` and the term have the form

.. math::

    \mathcal{H}_{1,1}
    =
    C_{1, 1}
    \sum_{\mu_1; \alpha_1; i_1}
    V_{\mu_1; \alpha_1}^{i_1}
    X_{\mu_1; \alpha_1}^{i_1}

Magpie, SpinW, Sunny
--------------------

In :ref:`zoo_magpie`, :ref:`zoo_spinw` and :ref:`zoo_sunny`, the Zeeman term is
written as (with :math:`H` in magpie and spinW, instead of :math:`B`)

.. math::

    \mathcal{H}
    =
    \mu_B
    \mathbf{B}
    \sum_{i}
    g_i
    \mathbf{S}_i

By renaming the indices as :math:`i \rightarrow (\mu_1, \alpha_1)` and writing
the scalar product explicitly as a sum over Cartesian components, one gets

.. math::

    \mathcal{H}
    =
    \mu_B
    \sum_{\mu_1; \alpha_1; i_1}
    g_{\mu_1, \alpha_1}
    B^{i_1}
    S_{\mu_1, \alpha_1}^{i_1}

where :math:`i_1 = x, y, z`. From here the correspondence is clear

.. math::

    C_{1, 1} &= 1
    \\
    V_{\mu_1; \alpha_1}^{i_1} &= \mu_B g_{\mu_1, \alpha_1} B^{i_1}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= S_{\mu_1, \alpha_1}^{i_1}

McPhase
-------

In :ref:`zoo_mcphase`, the Zeeman term is written as

.. math::

    \hat{\mathcal{H}}_{Z-J}
    =
    -
    \sum_{n, \alpha=1,2,3}
    g_n
    \mu_B
    \hat{J}^{n}_{\alpha}
    H_{\alpha}

or

.. math::

    \hat{\mathcal{H}}_{Z-LS}
    =
    -
    \sum_{n, \alpha=1,2,3}
    \mu_B
    \Bigl(
        2 \hat{S}^n_{\alpha} + \hat{L}^n_{\alpha}
    \Bigr)
    H_{\alpha}

By renaming the indices as :math:`n \rightarrow (\mu_1, \alpha_1)` and
:math:`\alpha \rightarrow i_1`, one gets

.. math::

    \hat{\mathcal{H}}
    =
    -
    \sum_{\mu_1; \alpha_1, i_1}
    g_{\mu_1, \alpha_1}
    \mu_B
    \hat{J}^{\mu_1, \alpha_1}_{i_1}
    H_{i_1}

or

.. math::

    \hat{\mathcal{H}}
    =
    -
    \sum_{\mu_1; \alpha_1, i_1}
    \mu_B
    \Bigl(
        2 \hat{S}^{\mu_1, \alpha_1}_{i_1} + \hat{L}^{\mu_1, \alpha_1}_{i_1}
    \Bigr)
    H_{i_1}

From here the correspondence is clear

.. math::

    C_{1, 1} &= -1
    \\
    V_{\mu_1; \alpha_1}^{i_1} &= g_{\mu_1, \alpha_1} \mu_B H_{i_1}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= \hat{J}^{\mu_1, \alpha_1}_{i_1}

or

.. math::

    C_{1, 1} &= -1
    \\
    V_{\mu_1; \alpha_1}^{i_1} &= \mu_B H_{i_1}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= 2 \hat{S}^{\mu_1, \alpha_1}_{i_1} + \hat{L}^{\mu_1, \alpha_1}_{i_1}

Spirit
------

In :ref:`zoo_spirit`, the Zeeman term is written as 

.. math::

   \mathcal{H}_{\rm Zeeman}
   =
   -\sum_i \mu_i \vec{B}\cdot \vec{n}_i

By renaming the indices as :math:`i \rightarrow (\mu_1, \alpha_1)` and writing
the scalar product explicitly as a sum over Cartesian components, one gets

.. math::

   \mathcal{H}_{\rm Zeeman}
   =
   -\sum_{\mu_1, \alpha_1, i_1} \mu_{\mu_1, \alpha_1} B^{i_1} n_{\mu_1, \alpha_1}^{i_1}


From here the correspondence is clear

.. math::

    C_{1, 1} &= -1
    \\
    V_{\mu_1; \alpha_1}^{i_1} &= \mu_{\mu_1, \alpha_1} B^{i_1}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= n_{\mu_1, \alpha_1}^{i_1}


