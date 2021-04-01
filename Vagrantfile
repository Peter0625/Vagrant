host_list = [
  {
  :name => "host1",
  :box => "centos/7"
  },
  {
  :name => "host2",
  :box => "ubuntu/trusty64"
  },
  {
  :name => "host3",
  :box => "generic/centos8"
  },
]

Vagrant.configure("2") do |config|
  host_list.each do |item|
    config.vm.define item[:name] do |host|
      host.vm.box = item[:box]
    end
  end
  #config.vm.box = "ubuntu/trusty64"
end
