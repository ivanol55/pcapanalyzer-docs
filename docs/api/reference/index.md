# API reference

Here you can find example queries and responses to the PCAPAnalyzer API endpoints

## dblist

### Request

`curl https://{domain}/api/dblist.php?apikey=42af1e890d3`

### Response

	{
	  "code": 200,
	  "databases": [
	    "packetstream",
	    "analysis_ssh"
	  ]
	}

## insights

### Request

`curl https://{domain}/api/insights.php?apikey=47d16be1c459&database=packetstream`

### Response

	{
	  "code": 200,
	  "privateips": [
	    "192.168.1.111",
	    "192.168.1.99",
	    "172.17.168.163",
	    "172.17.16.225"
	  ],
	  "publicips": [
	    "216.58.201.170",
	    "13.33.237.133",
	    "151.101.134.214",
	    "52.34.194.35",
	    "216.58.209.74",
	    "52.43.242.4",
	    "93.176.183.102",
	    "192.0.73.2",
	    "142.250.184.161",
	    "192.99.17.213",
	    "45.148.10.66"
	  ],
	  "macaddresses": [
	    "33:33:ff:78:95:4f",
	    "33:33:ff:38:2d:11",
	    "33:33:00:00:00:02",
	    "33:33:00:01:00:02",
	    "33:33:00:00:00:16",
	    "01:00:5e:00:00:fb",
	    "ff:ff:ff:ff:ff:ff",
	    "d8:61:94:e6:db:bf",
	    "7c:d6:61:38:2d:11",
	    "33:33:ff:ad:66:57",
	    "38:22:e2:63:58:b6",
	    "08:00:27:d1:62:8e",
	    "4c:63:71:ad:66:57",
	    "33:33:ff:e1:53:1d",
	    "94:de:80:bc:71:45",
	    "8c:e1:17:e5:f1:2e",
	    "33:33:ff:63:58:b6",
	    "33:33:00:00:00:01",
	    "33:33:00:00:00:fb",
	    "20:89:86:ae:3e:98",
	    "e4:e1:30:78:95:4f",
	    "88:29:9c:c5:3c:45",
	    "01:00:5e:7f:ff:fa"
	  ],
	  "protocolsfound": [
	    "NBNS",
	    "RTMP",
	    "DHCPv6",
	    "TLSv1",
	    "DHCP",
	    "ICMP",
	    "SSH",
	    "OCSP",
	    "TCP",
	    "MDNS",
	    "TLSv1.2",
	    "SSLv2",
	    "PGSQL",
	    "ARP",
	    "ICMPv6",
	    "SSDP",
	    "DNS",
	    "LLC",
	    "TLSv1.3"
	  ],
	  "wellknownports": [
	    "80",
	    "67",
	    "443",
	    "22",
	    "547",
	    "53",
	    "137"
	  ],
	  "registeredports": [
	    "37026",
	    "46671",
	    "46944",
	    "1935",
	    "42440",
	    "42526",
	    "40110",
	    "35364",
	    "34742",
	    "44793",
	    "48748",
	    "38674",
	    "37317",
	    "38352",
	    "37826",
	    "47926",
	    "38530",
	    "44602",
	    "46764",
	    "38100",
	    "37563",
	    "38532",
	    "35293",
	    "48906",
	    "49066",
	    "47280",
	    "1900",
	    "41822",
	    "47668",
	    "35557"
	  ]
	}

## rawnumbers

### Request

`curl https://{domain}/api/rawnumbers.php?apikey=47d16be1c459&database=packetstream`

### Response
	{
	  "code": 200,
	  "packetcount": 198990,
	  "datasourcecount": 3,
	  "externalipcount": 75,
	  "maccount": 23,
	  "multicastcount": 139,
	  "protocolcount": 19
	}
