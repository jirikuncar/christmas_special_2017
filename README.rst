===============================
PyData Zurich meetup Blockchain
===============================

This is a basic implementation for the **Build your own Blockchain** 🎄 PyData Zurich 🎄 Xmas special and is mainly derived from this `repository <https://github.com/dvf/blockchain>`_.

Click the badge to run the notebooks from your browser:

.. image:: https://mybinder.org/badge.svg
  :target: https://mybinder.org/v2/gh/pydatazrh/christmas_special_2017/master?filepath=notebooks

The app is deployed on Heroku an accessible:


.. image:: https://img.shields.io/badge/Heroku-blockchain_pydatazrh-orange.svg?style=flat
        :target: https://blockchain-pydatazrh.herokuapp.com/#/default

---------
Resources
---------

- `Slides <https://docs.google.com/presentation/d/1GaoGagHTQYcABOVAgY40T1SVCzFKpH6H_4T8jVZlnsU/edit#slide=id.p>`_
- Notebooks
    - `Hash functions <https://mybinder.org/v2/gh/pydatazrh/christmas_special_2017/master?filepath=notebooks/01-hash-functions.ipynb>`_
    - `Transaction list <https://mybinder.org/v2/gh/pydatazrh/christmas_special_2017/master?filepath=notebooks/02-transaction-list.ipynb>`_
    - `Proof of work <https://mybinder.org/v2/gh/pydatazrh/christmas_special_2017/master?filepath=notebooks/03-proof-of-work.ipynb>`_
    - `Blocks and blockchain <https://mybinder.org/v2/gh/pydatazrh/christmas_special_2017/master?filepath=notebooks/04-blocks-and-blockchain.ipynb>`_


------
Local
------

To run the application locally make sure to have all dependencies installed and then launch the server::

    > pip3 install -r requirements.txt

    > python3 api.py


------
Docker
------

To run the blockchain in a docker environment run::

    > docker build -t blockchain_pydatazrh:latest .

    > docker run -d -p 8080:5000 blockchain_pydatazrh


------
Heroku
------

If you want to run it on your own Heroku account simply type::

    > heroku login

    > heroku create

    > git push heroku master

    > heroku ps:scale web=1

    > heroku open
