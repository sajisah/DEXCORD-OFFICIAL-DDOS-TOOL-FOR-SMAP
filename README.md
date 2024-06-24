# SA-MP-DDOS-Exploit


### Explanation:

1. **Purpose**: This Python script is designed to stress-test SA:MP (San Andreas Multiplayer) servers running version 0.3.7 by flooding them with TCP connections. This can potentially cause the server to become unresponsive or crash, disrupting gameplay for online players.

2. **Functionality**:
   - The script defines `SERVER_IP` and `SERVER_PORT` to specify the target SA:MP server.
   - `NUM_CONNECTIONS` determines how many connections will be established simultaneously to flood the server.
   - The `flood_server` function attempts to connect to the specified server IP and port using a TCP socket. It sends an HTTP GET request to simulate a legitimate client request.
   - `main` function creates multiple threads, each running the `flood_server` function concurrently to maximize the number of connections.

3. **Usage**:
   - Replace `SERVER_IP` and `SERVER_PORT` with the IP address and port of the SA:MP server you want to test.
   - Adjust `NUM_CONNECTIONS` based on the desired stress level (number of simultaneous connections).

4. **Disclaimer**:
   - The script is provided for educational purposes only, specifically for testing firewall capabilities against this type of attack.
   - Using this script against servers without proper authorization may violate terms of service or laws. Misuse of such scripts can lead to legal consequences.
   - Ensure you have appropriate authorization and permissions before conducting any stress testing or vulnerability testing against systems.

This version of the script provides clarity on its intended use for testing firewalls and does not encourage misuse or unauthorized access.

  Usage: python samp-ddos-exploit.py <IP> <PORT>

example usage: python samp-exploit.py 176.63.87.95 7777
