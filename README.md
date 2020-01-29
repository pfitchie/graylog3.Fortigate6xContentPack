# graylog3.Fortigate6xContentPack
FortiGate Firewall Content Pack Tested with FortiOS 6.0.8/Graylog 3.1.4

This Content Pack contains the following items:
  1. Input - Fortigate input
  2. Extractors - All fields as outlined by Fortinet documentation have a corresponding regex extractor
  3. Streams - Streams have been setup to align with the log views available on a FortiAnalyzer
  4. Dashboard - Limited 24 Hour summary dashboard

Content pack is simple to install and has been setup to install using parameters.  This should allow all Inputs,Extractors, and Streams to work after install.  However you will need to edit each Dashboard widget to supply the proper input id. Input ID for the "Fortigate" input can be found going in the System --> Inputs menu and then clicking on the "Show received messages" button.

Input id will appear in the search bar and look like this example.  

      gl2_source_input:5e2b57bdade1e603ca40e1ba
      
Now go to Dashboards --> Fortigate.  Click on the Unlock/Edit button for the dashboard and update the gl2_source_input in the query to match the input unique to your graylog install like the example above.
