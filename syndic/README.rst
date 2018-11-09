Salt syndic example
===================


::

    docker-compose up


    docker-compose exec salt bash
    root@salt:/# salt '*' test.ping
    minion1:
        True
    syndic:
        True
    minion2:
        True
