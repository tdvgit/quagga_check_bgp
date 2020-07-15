# quagga_check_bgp
nagios plugin для мониторинга BGP сессий в quagga

Изначально был использован вариант описанный http://www.hilik.org.ua/nagios-monitoring-bgp-quagga/

Для мониторинга через nrpe2.
В конфигурации nrpe2 скрипт прописывается так:

command[check_bgp_peer1]=/usr/local/libexec/nagios/check_bgp xxx.xxx.xxx.xxx

Здесь xxx.xxx.xxx.xxx ip адрес соседа.
В случае обрыва сессии возникнет alert.
