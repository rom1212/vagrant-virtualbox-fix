# vagrant-virtualbox-fix
Fix the issue that vagrant 1.8.1 cannot find virtualbox 5.1.x.

This is based on https://askubuntu.com/questions/867115/vagrant-unable-to-locate-virtualbox

All you need to do is:
```
git clone https://github.com/romans1212notes/vagrant-virtualbox-fix.git
cd vagrant-virtualbox-fix
sudo cp usr/share/vagrant/plugins/providers/virtualbox/driver/meta.rb /usr/share/vagrant/plugins/providers/virtualbox/driver/
sudo cp usr/share/vagrant/plugins/providers/virtualbox/driver/version_5_1.rb /usr/share/vagrant/plugins/providers/virtualbox/driver/
sudo cp usr/share/vagrant/plugins/providers/virtualbox/plugin.rb /usr/share/vagrant/plugins/providers/virtualbox/
```

