ROOT_DIR := $(dir $(realpath $(lastword $(MAKEFILE_LIST))))

test-encode1:
	gcc -o bccbt bccbt.c
	./bccbt tests/test_file1 "" "" "" 0
	python3 bytearray.py
	gzip lvls
	rm bccbt bitcodes
test-encode2:
	gcc -o bccbt bccbt.c
	./bccbt tests/test_file2 "" "" "" 0
	python3 bytearray.py
	gzip lvls
	rm bccbt bitcodes
test-encode3:
	gcc -o bccbt bccbt.c
	./bccbt tests/test_file3 "" "" "" 0
	python3 bytearray.py
	gzip lvls
	rm bccbt bitcodes
test-1MBencode:
	gcc -o bccbt bccbt.c
	./bccbt battlearena/1MB.txt "" "" "" 0
	python3 bytearray.py
	gzip lvls
	rm bccbt bitcodes
test-5MBencode:
	gcc -o bccbt bccbt.c
	./bccbt battlearena/5MB.txt "" "" "" 0
	python3 bytearray.py
	gzip lvls
	rm bccbt bitcodes	
test-10MBencode:
	gcc -o bccbt bccbt.c
	./bccbt battlearena/10MB.txt "" "" "" 0
	python3 bytearray.py
	gzip lvls
	rm bccbt bitcodes	
test-20MBencode:
	gcc -o bccbt bccbt.c
	./bccbt battlearena/20MB.txt "" "" "" 0
	python3 bytearray.py
	gzip lvls
	rm bccbt bitcodes	
test-40MBencode:
	gcc -o bccbt bccbt.c
	./bccbt battlearena/40MB.txt "" "" "" 0
	python3 bytearray.py
	gzip lvls
	rm bccbt bitcodes	
test-80MBencode:
	gcc -o bccbt bccbt.c
	./bccbt battlearena/80MB.txt "" "" "" 0
	python3 bytearray.py
	gzip lvls
	rm bccbt bitcodes	
test-100MBencode:
	gcc -o bccbt bccbt.c
	./bccbt battlearena/100MB.txt "" "" "" 0
	python3 bytearray.py
	gzip lvls
	rm bccbt bitcodes	
test-decode:
	gzip -d lvls.gz
	python3 bitpull.py
	gcc -o bccbt bccbt.c
	./bccbt "" bitcodes lvls freqs 1
	rm bitcodes lvls freqs binaryfile bccbt
