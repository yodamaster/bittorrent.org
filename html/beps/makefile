
# Be sure to commit changes to .rst files before building the html and then recommit with the updated html.
# Otherwise, the generated .html will have the svn revision number of the previous change rather than the
# current changes.

BEPS= \
	bep_0000.html \
	bep_0001.html \
	bep_0002.html \
	bep_0003.html \
	bep_0004.html \
	bep_0005.html \
	bep_0006.html \
	bep_0007.html \
	bep_0008.html \
	bep_0009.html \
	bep_0010.html \
	bep_0012.html \
	bep_0015.html \
	bep_0016.html \
	bep_0017.html \
	bep_0018.html \
	bep_0019.html \
	bep_0020.html \
	bep_0021.html \
	bep_0022.html \
	bep_0023.html \
	bep_0024.html \
	bep_0025.html \
	bep_0026.html \
	bep_0027.html \
	bep_0028.html \
	bep_0029.html \
	bep_0030.html \
	bep_0031.html \
	bep_0032.html \
	bep_0033.html \
	bep_0034.html \
	bep_0035.html \
	bep_0036.html \
	bep_0037.html \
	bep_0038.html \
	bep_0039.html \
	bep_0040.html \
	bep_1000.html \

all:	$(BEPS) 

%.html:%.rst_post
	rst2html-2.6.py --template=template.txt --pep-base-url=http://www.bittorrent.org/beps/ --cloak-email-addresses --link-stylesheet --stylesheet=../css/bep.css --no-toc-backlinks $? >$@ --traceback

%.rst_post: %.rst
	python postprocess.py $? > $@ 

#%.html:%.rst
#	rstpep2html.py --template=template.txt --cloak-email-addresses --link-stylesheet --stylesheet=../css/bep.css --no-toc-backlinks $? >$@ --traceback



