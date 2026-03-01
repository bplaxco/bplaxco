workflow.svg: workflow.d2
	d2 workflow.d2 $@ 

.PHONY: watch
watch:
	while true; do inotifywait -e modify workflow.d2; make workflow.svg; done
