# microBlock
Project that utilizes host configuration files to block ads and malicious sites

biggest current issue is that large host list makes it difficult to delete/refresh the hosts list because itll be in use by "dns client." can be fixed by disabling via regedit and restarting. 

notes:
 - need to find way to disable client via cmd, and reenable at every start if possible
    - https://softaro.net/en/dns-client-service-disable/
    - https://thegeekpage.com/start-stop-option-of-dns-client-service-is-greyed-out-i/#:~:text=Step%201%3A%20Press%20Win%20%2B%20X,DNS%20Client%20from%20the%20list.

goals:
 - on start:
    - download and refresh ban list everytime computer starts
 - on uninstall:
    - kill and delete executables
    - delete and replace original hosts list
    - delete uninstaller
