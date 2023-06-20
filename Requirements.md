# Requirements needed for the Dependency-Track Server

Dependency-Track used to recommend to use their Executable WAR files, but it became deprecated.

>**Deprecation Notice**
>
>The Executable WAR is deprecated and will no longer be distributed in a future version of Dependency-Track It is advisable that organizations migrate to a container strategy such as Docker or Kubernetes.

Instead, they recommend to use Docker or Kubernetes to run the server **locally**, but following their documentation using the JAR file is fine for **production**.

## Hardware requirements

|Minimum CPU cores|Recommended CPU cores|
|:---:|:---:|
|**2** CPU cores|**4** CPU cores|
|**4** GB RAM|**16** GB RAM|

***Note:*** *With my little usage of the server, I didn't notice real performance issues with 2 CPU cores and 4 GB RAM. I decided to try with 4 CPU and 8 GB RAM, it runs much faster while combined with `openjdk-19`.*

## Softwares

- **Java 17 (or higher)** is required to run the server.