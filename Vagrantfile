# -*- mode: ruby -*-
# vi: set ft=ruby :

boxes = [
  {:name => "IE8-Win7", :atlas => "modernIE/w7-ie8"},
  {:name => "IE9-Win7", :atlas => "modernIE/w7-ie9"},
  {:name => "IE10-Win7", :atlas => "modernIE/w7-ie10"},
  {:name => "IE11-Win7", :atlas => "modernIE/w10-edge"},
  {:name => "IE10-Win8", :atlas => "modernIE/w8-ie10"},
  {:name => "IE11-Win8.1", :atlas => "modernIE/w8.1-ie11"},
  {:name => "Edge-Win10", :atlas => "modernIE/w10-edge"}
]

Vagrant.configure(2) do |config|
  boxes.each do |box|
    config.vm.define box[:name] do |machine|
      machine.vm.box = box[:atlas]
    end
  end
end
