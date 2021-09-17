# Preparando Ambiente Linux/Java
Passo a passo para instalação do Ubuntu, VMWare e utilização do terminal para preparação do ambiente para programação em Java.

### VMWare Workstation Player 15
<https://www.vmware.com/go/getplayer-win/>

### Ubunto 20.04 LTS
https://ubuntu.ltsbrasil.net/ubuntu-releases/20.04-desktop-amd64.iso

## Instalando o Java 10

- sudo add-apt-repository ppa: linuxuprising/java
- sudo apt update
- sudo apt instal oracle-java10-installer

- java --version

## Ferramentas de build

### Gradle
https://gradle.org

- versão 4.7

- mkdir /opt/gradle
- cd Global\ Labs\ Academy
- unzip -d /opt/gradle gradle-4.7-bin.zip
- ls /opt/gradle/gradle-4.7
- export PATH=$PATH:/opt/gradle/gradle-4.7/bin

- sudo apt purge gradle //oldversions

- gradle -v

### Maven

<p>https://maven.apache.org<br>
versão 3.5.3</p>

- unzip -d /opt/maven apache-maven-3.5.3-bin.zip
- ls /opt/maven/apache-maven-3.5.3
- sudo apt purge maven //old versions
- export PATH=$PATH:/opt/maven/apache-maven-3.5.3/bin

- mvn -v

### Wrappers

https://github.com/takari/maven-wrapper
https://docs.gradle.org/current/userguide/gradle_wrapper.html

- gradle wrapper
- ./gradlew -v
- mvn -N io.takari:maven:wrapper
- ./mvn -v

