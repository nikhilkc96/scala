# scala
Scala is a general-purpose programming language providing support for functional programming and a strong static type system. Designed to be concise, many of Scala's design decisions aimed to address criticisms of Java

# sbt and scala install steps 

echo "deb https://dl.bintray.com/sbt/debian /" | sudo tee -a /etc/apt/sources.list.d/sbt.list
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 2EE0EA64E40A89B84B2DF73499E82A75642AC823
sudo apt-get update
sudo apt-get install sbt

# the following command will take several minutes. it will finally start a sbt shell.
sbt

# exit the shell by typing exit at the prompt, i.e.
exit

-- not needed----------

sudo apt-get remove --purge openjdk* java-common default-jdk
sudo apt-get remove --purge sbt
sudo apt-get autoremove --purge

# Check weather you successfully removed all related packages by:

sudo update-alternatives --config java

# The system shall prompt you there is no Java available to config, otherwise this workaround fails.

# Then reinstall required packages:

sudo apt-get install openjdk-8-jdk sbt

# In ~/.bashrc, change JAVA_HOME as below:

export JAVA_HOME=/usr/lib/jvm/java-1.8.0-openjdk-amd64

# quit the terminal and restart another terminal.

# Go to project directory and run sbt as
sbt

# exit sbt shell by typing exit, i.e. type exit at prompt sbt:student>

# getting scala
sudo apt-get install scala



