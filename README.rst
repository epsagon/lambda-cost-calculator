Lambda Functions Cost Calculator
================================

.. image:: https://github.com/epsagon/lambda-cost-calculator/blob/master/lambda-cost-calculator.png
   :align: center

(Based on `photo <https://commons.wikimedia.org/wiki/File:AWS_Lambda_logo.svg>`_ by Valve Software / `CC BY-SA 4.0 <https://creativecommons.org/licenses/by-sa/4.0/deed.en>`_)

Motivation
----------
- Understand the usage (invocations and avg. duration) of Lambda functions.
- Understand and estimate the cost of Lambda functions (projected monthly based on last day).


Setup
-----
.. code-block:: bash

    git clone https://github.com/epsagon/lambda-cost-calculator
    cd lambda-cost-calculator/
    pip install -r requirements.txt
    python lambda_cost_calculator.py


Example Outputs
---------------

CLI:

.. image:: https://github.com/epsagon/lambda-cost-calculator/blob/master/examples/cli.png

CSV file:

.. image:: https://github.com/epsagon/lambda-cost-calculator/blob/master/examples/csv.png


Usage
-----

Output data to CSV (**It will include more relevant data!**):

.. code-block:: bash

    python lambda_cost_calculator.py --csv lambda_cost.csv

Provide credentials:

.. code-block:: bash

    python lambda_cost_calculator.py --token-key-id <access_key_id> --token-secret <secret_access_key>
