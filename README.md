
# Tableau Python Server - Alpha

Tableau Python Server (TabPy) is part of Tableau's expanding range of extensibility options. These include [R execution](http://onlinehelp.tableau.com/current/pro/desktop/en-us/help.html#r_connection_manage.html) via the calculation editor interface, along with the web data connector SDK, the JavaScript API, the REST API, the Tableau Data Extract API, and Tableau Document API. For details, see the [Tableau Developer Portal](https://community.tableau.com/community/developers).

TabPy framework allows Tableau to remotely execute Python code. It has two components:

1. A [server](server.md) process built on Tornado, which allows for the remote execution of Python code through a set of REST APIs. Code can either be immediately executed or persisted in the server process and exposed as a REST endpoint, to be called later.
2. A [client library](client.md) that enables the deployment of such endpoints, based on Python functions.

Tableau can connect to the TabPy server to execute Python code on the fly and display results in Tableau visualizations. Users can control data and parameters being sent to TabPy by interacting with their Tableau worksheets, dashboard or stories. 

To run Python code in your Tableau calculated fields, enter the address and port number for a TabPy server instance in Tableau.

On Tableau Server, use the [tabadmin](https://onlinehelp.tableau.com/current/server/en-us/tabadmin.htm) command line utility to configure a TabPy connection.

It is not necessary to install TabPy on the Tableau Server or Desktop computer-all that is required is a pointer to a TabPy server instance.

<p align="center"><img alt="Screenshot of Configuration on Tableau Desktop" src="external-service-configuration.png"></p>

Once the configuration is done, you can use Python in calculated fields in Tableau.

<p align="center"><img alt="Screenshot of a Python calculated field on Tableau Desktop" src="python-calculated-field.png"></p>