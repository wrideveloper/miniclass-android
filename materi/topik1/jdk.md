# Installing JDK/OpenJdk

## OpenJDK 

- Buka terminal kamu : 
    - Tambah repository OpenJDK 
    ```zsh
        sudo add-apt-repository ppa:openjdk-r/ppa
    ```
    - Update System Package kamu and install OpenJDK 8 
    ```zsh
        sudo apt-get update
        sudo apt-get install openjdk-8-jdk
    ```
    - Pastikan java kamu terinstall
    ```zsh
        java -version
    ```
    - akan keluar
    ```zsh
        openjdk version "1.8.0_72-internal"
        OpenJDK Runtime Environment (build 1.8.0_72-internal-b05)
        OpenJDK 64-Bit Server VM (build 25.72-b05, mixed mode)
    ```

## Oracle JDK
- Linux
    - Buka terminal kamu : 
    - Tambah repository Oracle 
    ```zsh
         sudo add-apt-repository ppa:webupd8team/java
    ```
    - Update System Package kamu and install Oracle JDK 8
    ```zsh
        sudo apt update; sudo apt install oracle-java8-installer
    ```
    - Pastikan java kamu terinstall
    ```zsh
        java -version
    ```
- Windows
    - Ikuti Cara Ini [Cara Install JDK](https://www.tutorialpedia.net/cara-install-java-di-windows-10-dan-linux/)

- Mac
    - Download [JDK](http://www.oracle.com/technetwork/java/javase/downloads/jdk10-downloads-4416644.html)
    - Buka File .pkg yang udah kalian download
    - Buka Package icon untuk memulai instalasi
    - Klik jika ada tulisan next
    - Lalu close jika sudah ada tulisan close
