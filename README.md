ip netns add demons
CNI_COMMAND=DEL CNI_NETNS=/var/run/netns/demons CNI_IFNAME=demoeth0 CNI_PATH=/opt/cni/bin ./ptp

watch -d -n1 'ip netns exec demons ifconfig;ip netns exec demons route -n'
watch -n 1 'ifconfig; route -n'
