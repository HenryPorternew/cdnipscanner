# cdnipscanner

config.ini is the settings file for cdnipscanner

    IPRange: File path of CDN IPs to check in CIDR format.
    Result: File path to save the result. Three formats are supported: .txt, .csv, .json.
    IPVersion: IP version of the IPRange file. Two formats are supported: ipv4, ipv6.
    ScanOrder: How IPs are scanned. Two methods are supported: sorted, random.
    ScanProtocol: Scan protocol. Two protocols are supported: https, http.
    SNIDomain: Domain or website to check IPs against. This should be behind the same CDN.
    HTTPHost: HTTP host for custom checks. If empty, SNIDomain will be used.
    HTTPPath: HTTP path for custom checks.
    PortNumber: Port number for custom checks. If empty, the default port for http (80) or https (443) will be used.
    ReturnCode: HTTP return code when accessing ScanProtocol://SNIDomain/HTTPPath:PortNumber. You can check the return code from the app menu.
    ThreadNumber: Number of checks to run simultaneously.
    ThreadInterval: Delay between threads starting.
    IPCount: Number of IPs to load from the IPRange file.
    ResultCount: Number of live IPs to find.
    Timeout: Timeout for each IP check if not responding.
    MaxPing: Maximum ping of live IPs to be saved in the result.
