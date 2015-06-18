# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
	config.vm.box = "deb/jessie-amd64"
	
	config.push.define "local-exec" do |push|
		push.inline = <<-SCRIPT
			ssh deltastep.org "cd /var/www/deltastep.org/app; git pull"
		SCRIPT
	end
end
