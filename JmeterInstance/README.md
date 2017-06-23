Configuring Jmeter Instance
============================

Follow these steps to configure Jmeter instance

## Prerequisites

1. The script uses "unzip" command. Therefore please make sure it is installed.

`sudo apt install unzip`

The "install-java.sh" script will not download the Java distribution. You need to [download JDK] from Oracle.

It is required to have all Java distributions in a single directory.

For example, if you want to install Java 7, following files should be downloaded and moved to a single directory.

 - jdk-7u80-linux-x64.tar.gz
 - jdk-7u80-linux-x64-demos.tar.gz
 - UnlimitedJCEPolicyJDK7.zip

Similarly for Java 8, following are the files required

 - jdk-8u131-linux-x64.tar.gz
 - jdk-8u131-linux-x64.tar.gz
 - jce_policy-8.zip

The Java Demos and Java Cryptography Extension (JCE) Unlimited Strength Jurisdiction Policy files are optional.

Note: This folder contains "jdk-8u131-linux-x64.tar.gz" in "software/java" folder. Please update relevant files accordingly.

2. Add instance hostname in to /etc/hosts

3. Add server key in to a folder (Ex: ~/key) and give permission as "chmod 600 keyFile"

4. Edit config file with respective IPs and hosts. Give file path to key file.

5. Edit run_all script with ip of EI Server

6. Edit ESB_Perf.jmx with ip of EI

7. Jmeter should be downloaded and update path to it in script.

Note: Script refer path as "~/software/"

8. Edit esb-perf-execution.sh file with respective hosts

9. Edit esb-perf-execution.sh product variable as you need (wso2ei-6.1.1, wso2esb-5.0.0)

## Run Scripts

1. Move all files in this folder in to home location of instance. 

2. Run configure_instance.sh

3. Run run_all.sh
