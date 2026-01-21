.. _mapping_exchange_striction:

******************
Exchange striction
******************


involves two magnetic sites and two "entities". Therefore, it
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

McPhase
-------

In :ref:`zoo_mcphase`, the exchange striction term is written as

.. math::

    \hat{\mathcal{H}}
    =
    -
    \dfrac{1}{2}
    \sum_{\substack{nn^{\prime},\alpha\beta\alpha^{\prime}\gamma=1,2,3\\\beta^{\prime}=1-6}}
    \Biggl(
        \dfrac{\partial \mathcal{J}_{\alpha\beta}}{\partial \epsilon_{\beta^{\prime}}}
        +
        \dfrac{\partial \mathcal{J}_{\alpha\beta}}{\partial R_{nn^{\prime}}^{\alpha^{\prime}}}
        \dfrac{\partial \epsilon_{\alpha^{\prime}\gamma} R_{nn^{\prime}}^{\gamma}}{\partial \epsilon_{\beta^{\prime}}}
    \Biggr)
    \epsilon_{\beta^{\prime}}
    \hat{\mathcal{I}}_{\alpha}^n
    \hat{\mathcal{I}}_{\beta}^{n^{\prime}}

By renaming indices as :math:`n \rightarrow (\mu_1, \alpha_1)`, 
:math:`n^{\prime} \rightarrow (\mu_2, \alpha_2)`, :math:`\alpha \rightarrow i_1`,
:math:`\beta \rightarrow i_2` one gets


.. math::

    \hat{\mathcal{H}}
    =
    -
    \dfrac{1}{2}
    \sum_{\substack{\mu_1, \mu_2, \alpha_1, \alpha_2, i_1, i_2}}
    \sum_{\alpha^{\prime}\gamma=1,2,3\\\beta^{\prime}=1-6}
    \Biggl(
        \dfrac{\partial \mathcal{J}_{i_1,i_2}}{\partial \epsilon_{\beta^{\prime}}}
        +
        \dfrac{\partial \mathcal{J}_{i_1,i_2}}{\partial R_{\mu_1,\mu_2;\alpha_1,\alpha_2}^{\alpha^{\prime}}}
        \dfrac{\partial \epsilon_{\alpha^{\prime}\gamma} R_{\mu_1,\mu_2;\alpha_1,\alpha_2}^{\gamma}}{\partial \epsilon_{\beta^{\prime}}}
    \Biggr)
    \epsilon_{\beta^{\prime}}
    \hat{\mathcal{I}}_{i_1}^{\mu_1,\alpha_1}
    \hat{\mathcal{I}}_{i_2}^{\mu_2,\alpha_2}

where :math:`i_1, i_2 = x, y, z`. From here the correspondence is clear

.. math::

    C_{2, 1} &= -\dfrac{1}{2} \\
    V_{\mu_1, \mu_2; \alpha_1, \alpha_2}^{i_1, i_2}
    &=
    \sum_{\alpha^{\prime}\gamma=1,2,3\\\beta^{\prime}=1-6}
    \Biggl(
        \dfrac{\partial \mathcal{J}_{i_1,i_2}}{\partial \epsilon_{\beta^{\prime}}}
        +
        \dfrac{\partial \mathcal{J}_{i_1,i_2}}{\partial R_{\mu_1,\mu_2;\alpha_1,\alpha_2}^{\alpha^{\prime}}}
        \dfrac{\partial \epsilon_{\alpha^{\prime}\gamma} R_{\mu_1,\mu_2;\alpha_1,\alpha_2}^{\gamma}}{\partial \epsilon_{\beta^{\prime}}}
    \Biggr)
    \epsilon_{\beta^{\prime}}
    \\
    X_{\mu_1; \alpha_1}^{i_1} &= \hat{\mathcal{I}}_{i_1}^{\mu_1,\alpha_1} \\
    X_{\mu_2; \alpha_2}^{i_2} &= \hat{\mathcal{I}}_{i_2}^{\mu_2,\alpha_2}