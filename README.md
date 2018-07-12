ip netns add demons
CNI_COMMAND=DEL CNI_NETNS=/var/run/netns/demons CNI_IFNAME=demoeth0 CNI_PATH=/opt/cni/bin ./ptp
