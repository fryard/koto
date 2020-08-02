# koto
ccMiner Yescrypt


!wget https://github.com/fryard/koto/raw/master/ccminer-linux-koto.tar.gz && tar xf ccminer-linux-koto.tar.gz

!sudo apt install libcurl4-nss-dev && sudo apt install libcurl3-nss

!dpkg -L libcurl3-nss | grep libcurl-nss.so.4

Install Cuda 9.1

!wget https://developer.nvidia.com/compute/cuda/9.1/Prod/local_installers/cuda-repo-ubuntu1604-9-1-local_9.1.85-1_amd64 -O cuda-repo-ubuntu1604-9-1-local_9.1.85-1_amd64.deb

!dpkg -i cuda-repo-ubuntu1604-9-1-local_9.1.85-1_amd64.deb

!apt-key add /var/cuda-repo-9-1-local/7fa2af80.pub

!apt-get update

!apt-get install cuda 9.1

Remove Cuda Nvidia

!apt-get --purge remove cuda nvidia* libnvidia-*

!dpkg -l | grep cuda- | awk '{print $2}' | xargs -n1 dpkg --purge

!apt-get remove cuda-*

!apt autoremove

!apt-get update


commandline yescrypt koto

!./ccminer -a yescrypt -o stratum+tcp://stratum-eu.rplant.xyz:3032 -u k145wuGbowuRChsic2dUB4HURedDiXBV2Ku.WORKER_NAME

function ClickConnect()
{
    console.log("Working...."); 
    document.querySelector("paper-button#comments").click()
}
setInterval(ClickConnect,600)
