#!/bin/bash
sudo sysctl -w vm.overcommit_memory=1 &&
alias sail='[ -f sail ] && sh sail || sh vendor/bin/sail' &&
sail up

