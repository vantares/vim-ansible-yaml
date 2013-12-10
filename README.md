# vim-ansible-yaml

Adds additional syntax highlighting and fixes indentation for Ansible's dialect of YAML.

Ansible YAML files are detected based on the presence of a
[structure following Ansible's Playbook Best Practices](http://www.ansibleworks.com/docs/playbooks_best_practices.html#directory-layout).

## Install

### Using [Vundle](https://github.com/gmarik/vundle)

1. Add the following to your `.vimrc` where other bundles are located:
       
		Bundle 'chase/vim-ansible-yaml'

2. Run from command line:

		$ vim +BundleInstall

### Using [pathogen](https://github.com/tpope/vim-pathogen)

1. Check out the repository into your bundle path:

        $ cd ~/.vim/bundle
        $ git clone git://github.com/chase/vim-ansible-yaml.git

### Normal

1. Check out the repository and copy the following to `.vim/` directory or any
   other run time path, keeping their directory structure intact:

		ftdetect/ansible.vim
		syntax/ansible.vim
		syntax/include/jinja.vim
		syntax/include/yaml.vim
		indent/ansible.vim

### TODO

* Add support for Jinja highlighting on conditionals like `when` and `changed_when`
* Fix highlighting of numbers and `-` mid-string