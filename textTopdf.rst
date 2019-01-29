vim file.txt -c "hardcopy > fileName.ps | q"; ps2pdf fileName.ps

enscript sample.txt -o - | ps2pdf14 - sample.pdf
