.. _mapping_biquadratic-exchange:

********************
Biquadratic exchange
********************

Biquadratic exchange involves two magnetic sites and four "entities" (two per
site). Therefore, it should map to the term of the Hamiltonian with

- :math:`k = 4`
- :math:`l = 3`

Then, :math:`m_{4,3} = 2` and the term have the form

.. math::

    \mathcal{H}_{4,3}
    =
    C_{4, 3}
    \sum_{\substack{\mu_1, \mu_2,\\ \alpha_1, \alpha_2,\\ i_1, i_2, i_3, i_4}}
    V_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2, i_3, i_4}
    X_{\mu_1; \alpha_1}^{i_1}
    X_{\mu_1; \alpha_1}^{i_2}
    X_{\mu_2; \alpha_2}^{i_3}
    X_{\mu_2; \alpha_2}^{i_4}

SpinW
-----

In :ref:`zoo_spinw`, the biquadratic exchange term is written as

.. math::
    \mathcal{H}
    =
    \sum_{i \neq j}
    B (\mathbf{S}_i \cdot \mathbf{S}_j)^2

By renaming the indices as :math:`i \rightarrow (\mu_1, \alpha_1)`,
:math:`j \rightarrow (\mu_2, \alpha_2)` and expanding the square, 
one can map this term in the form

.. math::

    \mathcal{H}
    =
    \sum_{\substack{\mu_1, \mu_2,\\ \alpha_1, \alpha_2,\\ i_1, i_2, i_3, i_4}}
    B^{i_1, i_2, i_3, i_4}
    S_{\mu_1; \alpha_1}^{i_1}
    S_{\mu_1; \alpha_1}^{i_2}
    S_{\mu_2; \alpha_2}^{i_3}
    S_{\mu_2; \alpha_2}^{i_4}

where :math:`i_1, i_2, i_3, i_4 = x, y, z`. Tensor :math:`B^{i_1, i_2, i_3, i_4}`
is defined as

.. math::

    B &= B^{xxxx} = B^{yyyy} = B^{zzzz} =
    \\
    &= B^{xyxy} = B^{xzxz} = B^{yzyz} = 
    \\
    &= B^{yxyx} = B^{zxzx} = B^{zyzy}

and all other components of :math:`B^{i_1, i_2, i_3, i_4}` are zero.

.. note::

    As :math:`i \ne j`, then :math:`\mathbf{S}_i` and :math:`\mathbf{S}_j` 
    commute, whether they are operators or vectors. 

From here the correspondence is clear

.. math::

    C_{4, 3} &= 1
    \\
    V_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2, i_3, i_4} &= B^{i_1, i_2, i_3, i_4}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= S_{\mu_1; \alpha_1}^{i_1}
    \\
    X_{\mu_2; \alpha_2}^{i_3} &= S_{\mu_2; \alpha_2}^{i_3}

Spirit
------

In :ref:`zoo_spirit`, the quadruplet interaction is written as

.. math::
    \mathcal{H}_{\rm quad}
    =
    - \sum_{ijkl} K_{ijkl} (\vec{n}_i \cdot \vec{n}_j)(\vec{n}_k \cdot \vec{n}_l)

if :math:`i = k` and :math:`j = l` (or, equivalently, :math:`i = l` and
:math:`j = k`), this interaction describe a biquadratic exchange between sites
:math:`i` and :math:`j`

.. math::
    \mathcal{H}_{\rm quad}
    =
    - \sum_{ij} K_{ij} (\vec{n}_i \cdot \vec{n}_j)^2

where :math:`K_{ij} \equiv K_{ijij}`. By renaming the indices as
:math:`i \rightarrow (\mu_1, \alpha_1)`, :math:`j \rightarrow (\mu_2, \alpha_2)` and
expanding the square, one can write this term in the form

.. math::

    \mathcal{H}_{\rm quad}
    =
    - \sum_{\substack{\mu_1, \mu_2,\\ \alpha_1, \alpha_2,\\ i_1, i_2, i_3, i_4}}
    K_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2, i_3, i_4}
    n_{\mu_1; \alpha_1}^{i_1}
    n_{\mu_1; \alpha_1}^{i_2}
    n_{\mu_2; \alpha_2}^{i_3}
    n_{\mu_2; \alpha_2}^{i_4}

where :math:`i_1, i_2, i_3, i_4 = x, y, z`. Tensor
:math:`K_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2, i_3, i_4}` is defined as

.. math::

    K_{ij} &= K_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{xxxx} = K_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{yyyy} = K_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{zzzz} =
    \\
    &= K_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{xyxy} = K_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{xzxz} = K_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{yzyz} = 
    \\
    &= K_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{yxyx} = K_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{zxzx} = K_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{zyzy}

and all other components of
:math:`K_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2, i_3, i_4}` are zero.

From here the correspondence is clear

.. math::

    C_{4, 3} &= -1
    \\
    V_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2, i_3, i_4} &= K_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2, i_3, i_4}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= n_{\mu_1; \alpha_1}^{i_1}
    \\
    X_{\mu_2; \alpha_2}^{i_3} &= n_{\mu_2; \alpha_2}^{i_3}


