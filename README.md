# 283_2

-For each member in your team, provide 1 paragraph detailing what parts of the lab that member implemented / researched. (You may skip this question if you are doing the lab by yourself).

-Describe in detail the steps you used to complete the assignment. Consider your reader to be someone skilled in software development but otherwise unfamiliar with the assignment. Good answers to this question will be recipes that someone can follow to reproduce your development steps.
Individual assignment by Tingjia;

1. Use the ubuntu enviornemnt for previous assignment and clone linux kernel from https://github.com/torvalds/linux.git.
2. nstall libs that needed for building linux kernel.
3. uname -a to check the version of kernel.
4. cp /boot/config-5.8.0-50-generic ./.config
5. make oldconfig for defalut config
6. Building kernel with make -j 4 modules && make -j 4 && sudo make modules_install && sudo make install
7. config KVM
8. sudo apt install qemu-kvm libvirt-clients libvirt-daemon-system bridge-utils virt-manager
9. Change and test the modified kernel
10.Emulate cpuid instruction with CPUID packed installed in KVM(sudo apt-get install cpuid)

-does the number of exits increase at a stable rate? Or are there more exits performed during certain VM operations? Approximately how many exits does a full VM boot entail?

No, the number of exits do not increase at a stable rate. There are more exits performed during certain VM operations. A full VM boot entail around 420000 exits.
