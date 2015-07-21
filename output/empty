LANG=en_US.UTF-8 
2 LC_ALL=en_US.UTF-8 
3 
 
4 .PHONY: docs deploy all clean 
5 
 
6 all: deploy 
7 
 
8 docs: 
9 	$(MAKE) -C docs 
10 	$(MAKE) -C assets 
11 
 
12 deploy: docs 
13 	$(MAKE) -C docs deploy 
14 	$(MAKE) -C assets deploy 
15 
 
16 clean: 
17 	$(MAKE) -C docs clean  
18 	$(MAKE) -C assets clean 
19 	find output/ -mindepth 1 -maxdepth 1 -exec rm -r "{}" "+" 
