admin.conf: ssh-config
	scp -F ssh-config master:/etc/kubernetes/admin.conf .

ssh-config: 
	vagrant up
	vagrant ssh-config > ssh-config

k8s-base.box: k8s-base.rb Makefile
	rm -f $@
	VAGRANT_VAGRANTFILE=$< vagrant destroy -f
	VAGRANT_VAGRANTFILE=$< vagrant up
	VAGRANT_VAGRANTFILE=$< vagrant package --output $@

clean:
	vagrant destroy -f
	rm -fv admin.conf ssh-config
