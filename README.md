What is Rustscan?

Rustscan, developed in Rust language, is a scanning tool that works with IPv6 support and uses less memory. It also provides up to three times faster scanning speed than Nmap.

Installation (for Linux)

It is important to note that before using RustScan, you must have Nmap installed on your system. Many Linux distributions, such as Kali Linux, come with Nmap by default, but for other distributions you may need to install Nmap separately.

We download the .deb extension package from https://github.com/arifsafa/Rustscan-Tool. (rustscan_1.8.0_amd64.deb)
Open terminal.
Go to the directory where the downloaded file is located with the cd command. For example, if the file is in the Downloads folder:
cd ~/Downloads
4. Type the following command and press Enter:

sudo dpkg -i rustscan_1.8.0_amd64.deb
Once the installation is complete, type rustscan in the terminal and press Enter. If the installation is successful, Rustscan's version information will be displayed.

5. Scan:

To scan a single IP address:
rustscan 192.168.1.100
* To scan the IP address range:
rustscan 192.168.1.0/24
* To scan a specific port range:
rustscan -p 80-443 192.168.1.100
Additional Parameters:

-s: Scanning for a specific service (e.g. -s ssh)
-t: Set scan time (e.g. -t 10m)
-v: To get verbose output (level 1–3)
-o: Save the results to a file (e.g. -o scan_result.txt)
Things to Consider When Using Rustscan:

Excessive packet load may cause the scanned system to IP block you. Therefore, you can restrict the time and package parameters.
Rustscan is a newer tool compared to Nmap and may not have some advanced nmap features.
