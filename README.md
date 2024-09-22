<<<<<<< HEAD
# external-enum-workflow
=======
external-enum-workflow
>>>>>>> 9715bb6 (adding some addtional cmds and starting a basic config file)
tools and some usage examples for external footprint enumeration workflows

`export enum-config.sh`

## amass
<<<<<<< HEAD

`amass enum -active -d $ROOTDOMAIN -brute -w $SUBDOMAIN_WL -dir amass4owasp -config /root/amass/config.yaml -o amass_results_owasp.txt`

# TODO
Amass <br>
Nuclei <br>
ZAP <br>
Dirb <br>
nikto?<br>
Nmap<br>
subjack<br>
OpenVAS/GreenBone<br>

# Vulnerability Management 
[Faraday](https://github.com/infobyte/faraday)

=======
`amass enum -active -d $ROOTDOMAIN -brute -w $SUBDOMAIN_WL -dir amass4owasp -config /root/amass/config.yaml -o amass_results_owasp.txt`

## nmap
### ping scan 
`nmap -v -iL domains.txt nmap -sn -oN ping_scan.txt`

## subjack
`~/./go/bin/subjack -w domains.txt -a -c ~/workspace/subjack/fingerprints.json -o subjack.txt`

## gobust
`gobuster dir -u $ROOTDOMAIN -w /Users/matt/workspace/wordlists/wordlists/discovery/directory_list_1.0.txt -v -o gobuster_output.txt`

## wpscan
`wpscan --url $ROOTDOMAIN --api-token $WPSCAN -o wpscan-results.txt --verbose`

## nuclei

# TODO
[x]Amass <br>
[]Nuclei <br>
[x]ZAP <br>
[x]gobuster <br>
[]nikto?<br>
[x]Nmap<br>
[x]subjack<br>
[]OpenVAS/GreenBone<br>
[x]whatRuns<br>
[x]wpscan<br>
[]whatweb<br>

# Code Base

## semgrep
semgrep --config=auto . > ../semgrep.output.txt
semgrep --config=auto . --json --json-val=semgrep.output.json

## Trufflehog
trufflehog filesystem --directory=$WORKSPACE

# Vulnerability Management 
[][Faraday](https://github.com/infobyte/faraday)

# Manual Web App Testing
[]Account Creation <br>
[]XSS (xss buster)<br>
[]SQLi (sqlmap)<br>
[]IDOR <br>
[]Session Handling - logout<br>
[]Sensitive Info Change<br>
[]Redirects?<br>
>>>>>>> 9715bb6 (adding some addtional cmds and starting a basic config file)
