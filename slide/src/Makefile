.PHONY: live build clean

live:
	@echo "Previewing main slides..."
	-@reveal-md main.md -w --scripts https://cdn.tonycrane.cc/heti/heti.js,heti_worker.js --template template.html || true

build:
	@echo "Building main slides..."
	@reveal-md main.md --scripts https://cdn.tonycrane.cc/heti/heti.js,heti_worker.js --template template.html --static ../site --assets-dir assets
	@rm ../site/main.html

clean:
	@echo "Cleaning up..."
	rm -rf ../site/
