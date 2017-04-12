export IMGDIR=~/images
export IMGNAME=img1.jpg
run-example:
	docker run --rm -v ${IMGDIR}:/images maoqide/pytesser tesseract /images/${IMGNAME} stdout
